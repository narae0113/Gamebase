## Game > Gamebase > Upgrade Guide

## 2.6.0

### Unity

#### Android Limitation

* Android Support Libraryバージョンが28.0.0に上がり、Unity 5、Unity 2017.1、Unity 2017.2ではAndroidのビルドが失敗します。
	* Unity 2017.4未満のバージョンのEditorを使用している場合はUnity 2017.4以上のバージョンをインストールし、「Editor/Data/PlaybackEngines/AndroidPlayer/Tools/gradle/lib」フォルダをコピーして使用中のUnity Editorの同じパスに上書きしてmainTemplate.gradleファイルを下記のように修正してください。

```groovy
// GENERATED BY UNITY. REMOVE THIS COMMENT TO PREVENT OVERWRITING WHEN EXPORTING AGAIN
buildscript {
	repositories {
		jcenter()
        // >>> For download Gradle Android Plugin
        maven {
            url 'https://maven.google.com'
        }
	}

	dependencies {
		//classpath 'com.android.tools.build:gradle:2.1.0'
        // >>> Update Gradle Android Plugin version
        classpath 'com.android.tools.build:gradle:2.3.0'
	}
}
```

#### Firebase Push

* Firebase Cloud Messagingを使用している場合Firebaseコンソールからgoogle-services.jsonファイルをダウンロードし、xmlリソースに変換してプロジェクトに追加しないとPushが正常に動作しません。
    * Gamebase 2.5.0 以前のバージョンではxmlリソースなしてPush動作に問題ありませんでしたが、Gamebase 2.6.0からは必ずxmlリソースが必要です。
* 下のガイドを参考にしてPush設定を行ってください。
    * [\[Game > Gamebase > Android SDK ご利用ガイド > Push > Settings > Firebase\]](./aos-push/#firebase)

#### Standalone

* Removed Japan Purchase
	* 日本決済がFadeOutしました。
	* GamebaseUnitySDK_IAPAdapterを使用している場合は、下記のフォルダを直接削除してください。
        * Asset/Toast/Common
        * Asset/Toast/Core
        * Asset/Toast/IAP
        * Asset/Toast/Standalone

### Android

#### Limitation

* minSdkVersionが15(IceCreamSandwichMR1, 4.0.3)から16(JellyBean, 4.1)に変更されました。
	* OS 4.1未満の端末では正常な動作を保障しないため、プロジェクトのminSdkVersionが15の場合、16に変更してください。

#### Removed APIs

* 削除された関数は次のとおりです。代替関数に変更してください。
    * **Gamebase.getAuthBanInfo()**を削除しました。**Gamebase.getBanInfo()**に変更してください。
    * **Gamebase.getLanguageCode()**を削除しました。**Gamebase.getDeviceLanguageCode()**に変更してください。
    * **new GamebaseConfiguration.Builder(void)**を削除しました。**GamebaseConfiguration.newBuilder()**に変更してください。
    * **new GamebaseConfiguration.Builder.setAppId()**を削除しました。**GamebaseConfiguration.newBuilder()**に変更してください。
    * **new GamebaseConfiguration.Builder.setAppVersion()**を削除しました。**GamebaseConfiguration.newBuilder()**に変更してください。

#### Changed / Deprecated APIs

* Gamebase.activeApp()は自動的に呼び出されるため、今後は呼び出す必要がありません。
* Gamebase.initialize()の引数に必要なGamebaseConfigurationの作成方法が変更されました。
    * **new GamebaseConfiguration.Builder(String, String)**の代わりに**GamebaseConfiguration.newBuilder()**を呼び出してください。
* LaunchingStatus.isPlayable()は今後、呼び出さないでください。
	* [\[Game > Gamebase > Android SDK使用ガイド > 初期化 > Launching Information\]](./aos-initialization/#launching-information)文書を参照してLaunching Status Codeに応じてゲームプレイが可能かどうかを直接決定してください。
* Purchase
    * Store Codeの変更ができないため、**GamebaseConfiguration.newBuilder()**でStore Codeを伝達する必要があります。
        * Gamebase.Purchase.getStoreCode() / Gamebase.Purchase.setStoreCode()は削除される予定です。今後は使用しないでください。
    * Gamebase.Purchase.requestRetryTransaction()は呼び出す必要がありません。
* Push
    * Gamebase Android SDK 2.6.0以上からは、プッシュメッセージを送信する時、Gamebaseコンソールの**プッシュ**タブのメニューから送信する必要があります。
        * Gamebase Android SDK 2.6.0未満の場合、Gamebaseコンソールの**プッシュ(旧)** タブからプッシュを送信する必要があります。
    * GamebaseConfiguration.Builder.setFCMSenderId()は呼び出す必要がありません。
    * GamebaseConfiguration.Builder.setTencentAccessKey(), GamebaseConfiguration.Builder.setTencentAccessId()を呼び出している場合、APIの呼び出しを削除し、build.gradleに次のように宣言する必要があります。

```groovy
android {
    defaultConfig {
        ...
        // >>> For Tencent Push Notification
        manifestPlaceholders = [
            XG_ACCESS_ID : "1234567890",
            XG_ACCESS_KEY : "ABCDEFGHIJKL",
        ]
    }
}
```

### iOS

* No special steps are required.

## 2.4.4

### Unity

* Setting Toolがアップデートされました。
    * フォルダ構造が変更され、以前のバージョンのSettingToolを完全に削除した後、再インストールする必要があります。

## 2.2.2

### Unity

* GamebaseUnitySDKSettingsクラスの**storeCodeAOS**の変数名が **storeCodeAndroid**に変更されました。
    * **storeCodeAOS**を参照してStore Codeを定義するコードやPrefabがある場合は変数の参照に失敗するため、**storeCodeAndroid**変数に変更してください。

## 2.2.0

### Unity

* GamebaseMainActivityのPackage Nameが変更されました。
    * AndroidManifest.xmlのMainActivity宣言を下記のように変更していない場合、クラッシュが発生します。
    * **com.toast.gamebase.activity.GamebaseMainActivity** -> **com.toast.android.gamebase.activity.GamebaseMainActivity**

```xml
<manifest>
    ...
    <application>
    ...
        <activity android:name="com.toast.android.gamebase.activity.GamebaseMainActivity"
            android:launchMode="singleTask"
            android:configChanges="keyboard|keyboardHidden|screenLayout|screenSize|orientation"
            android:label="@string/app_name">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    ...
    </application>
    ...
</manifest>
```

## 2.1.0

### Common

#### Removed APIs

* 使用していないTransferKey機能を削除しました。
	* Guestアカウント移行機能が必要な場合は、Gamebase SDK 2.2.1から追加された[\[Game > Gamebase > Unity SDK使用ガイド > 認証 > TransferAccount\]](./unity-authentication/#transferaccount)機能を利用してください。
	* 