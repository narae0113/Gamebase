## Game > Gamebase > エラーコード

## Client SDK

| Category        | Platform           | Error                                    | Error Code | Description                                    |
| --------------- | ------------------ | ---------------------------------------- | ---------- | ---------------------------------------- |
| Common          | Android, UNITY<br/>IOS | NOT_INITIALIZED<br/>TCGB\_ERROR\_NOT\_INITIALIZED | 1          | Gamebaseが初期化されていません。                |
|                 | Android, UNITY<br/>IOS | NOT\_LOGGED\_IN<br/>TCGB\_ERROR\_NOT\_LOGGED\_IN | 2          | ログインが必要です。                            |
|                 | Android, UNITY<br/>IOS | INVALID_PARAMETER<br/>TCGB\_ERROR\_INVALID\_PARAMETER | 3          | 正しくないパラメーターです。                           |
|                 | Android, UNITY<br/>IOS | INVALID\_JSON\_FORMAT<br/>TCGB\_ERROR\_INVALID\_JSON\_FORMAT | 4          | JSON形式のエラーです。                         |
|                 | Android, UNITY<br/>IOS | USER_PERMISSION<br/>TCGB\_ERROR\_USER\_PERMISSION | 5          | 権限がありません。                               |
|                 | Android, UNITY<br/>IOS | INVALID\_MEMBER<br/>TCGB\_ERROR\_INVALID\_MEMBER  | 6          | 正しくない会員に対するリクエストです。                              |
|                 | Android, UNITY<br/>IOS | BANNED\_MEMBER<br/>TCGB\_ERROR\_BANNED\_MEMBER   | 7         | 利用制限対象の会員です。                                |
|                 | Android, UNITY<br/>IOS | NOT_SUPPORTED<br/>TCGB\_ERROR\_NOT\_SUPPORTED | 10         | この機能には対応しておりません。                         |
|                 | UNITY<br/>IOS      | NOT\_SUPPORTED\_ANDROID<br/>TCGB\_ERROR\_NOT\_SUPPORTED\_ANDROID | 11         | この機能はAndroidには対応しておりません。               |
|                 | UNITY<br/>IOS      | NOT\_SUPPORTED\_IOS<br/>TCGB\_ERROR\_NOT\_SUPPORTED\_IOS | 12         | この機能はiOSには対応しておりません。                   |
|                 | UNITY              | NOT\_SUPPORTED\_UNITY\_EDITOR            | 13         | この機能はEditorには対応しておりません。                |
|                 | UNITY              | NOT\_SUPPORTED\_UNITY\_STANDALONE        | 14         | この機能はStandaloneには対応しておりません。            |
|                 | UNITY              | NOT\_SUPPORTED\_UNITY\_WEBGL             | 15         | この機能はWebGLには対応しておりません。                 |
|                 | Android            | ANDROID\_ACTIVITY\_DESTROYED             | 31         | Activityが強制終了しました。                       |
|                 | Android            | ANDROID\_ACTIVEAPP\_NOT\_CALLED          | 32         | activeApp APIが呼び出されませんでした。                 |
|                 | IOS                | IOS_GAMECENTER_DENIED                    | 51         | Gamecenterログインが拒否されました。                 |
| Network(Socket) | Android, UNITY<br/>IOS | SOCKET\_RESPONSE\_TIMEOUT<br/>TCGB\_ERROR\_SOCKET\_RESPONSE\_TIMEOUT | 101        | ネットワーク状態が不安定なため、レスポンスがありません。                |
|                 | Android, UNITY<br/>IOS | SOCKET_ERROR<br/>TCGB\_ERROR\_SOCKET\_ERROR | 110        | ソケットエラーです。                                  |
|                 | Android, UNITY<br/>IOS | UNKNOWN_ERROR<br/>TCGB\_ERROR\_UNKNOWN\_ERROR | 999        | ソケットの不明なエラーです。                           |
| Launching       | Android, UNITY<br/>IOS | LAUNCHING\_SERVER\_ERROR<br/>TCGB\_ERROR\_LAUNCHING\_SERVER\_ERROR | 2001       | 起動サーバーエラーです。                           |
|                 | Android, UNITY<br/>IOS | LAUNCHING\_NOT\_EXIST\_CLIENT\_ID<br/>TCGB\_ERROR\_LAUNCHING\_NOT\_EXIST\_CLIENT\_ID | 2002       | クライアントIDがありません。                   |
|                 | Android, UNITY<br/>IOS | LAUNCHING\_UNREGISTERED\_APP<br/>TCGB\_ERROR\_LAUNCHING\_UNREGISTERED\_APP | 2003       | 登録されていないアプリです。                       |
|                 | Android, UNITY<br/>IOS | LAUNCHING\_UNREGISTERED\_CLIENT<br/>TCGB\_ERROR\_LAUNCHING\_UNREGISTERED\_CLIENT | 2004       | 登録されていないクライアント(バージョン)です。          |
| Auth            | Android, UNITY<br/>IOS | AUTH\_USER\_CANCELED<br/>TCGB\_ERROR\_AUTH\_USER\_CANCELED | 3001       | ログインがキャンセルされました。                           |
|                 | Android, UNITY<br/>IOS | AUTH\_NOT\_SUPPORTED\_PROVIDER<br/>TCGB\_ERROR\_AUTH\_NOT\_SUPPORTED\_PROVIDER | 3002       | この認証方式には対応しておりません。                      |
|                 | Android, UNITY<br/>IOS | AUTH\_NOT\_EXIST\_MEMBER<br/>TCGB\_ERROR\_AUTH\_NOT\_EXIST\_MEMBER | 3003       | 退会されているか、存在しない会員です。                    |
|                 | Android, UNITY<br/>IOS | AUTH\_EXTERNAL\_LIBRARY\_ERROR<br/>TCGB\_ERROR\_AUTH\_EXTERNAL\_LIBRARY\_ERROR | 3009       | 外部認証ライブラリーエラーです。                     |
|                 | Android, UNITY<br/>IOS | AUTH_ALREADY_IN_PROGRESS_ERROR<br/>TCGB_ERROR_AUTH_ALREADY_IN_PROGRESS_ERROR | 3010       | 移行認証プロセスが完了しませんでした。                 |
|                 | Android, UNITY<br/>IOS | AUTH\_TRANSFERKEY\_EXPIRED<br/>TCGB\_ERROR\_AUTH\_TRANSFERKEY\_EXPIRED | 3031       | TransferKeyの有効期限が切れました。  |
|                 | Android, UNITY<br/>IOS | AUTH\_TRANSFERKEY\_CONSUMED<br/>TCGB\_ERROR\_AUTH\_TRANSFERKEY\_CONSUMED| 3032       | TransferKeyはすでに使われています。 |
|                 | Android, UNITY<br/>IOS | AUTH\_TRANSFERKEY\_NOT\_EXIST<br/>TCGB\_ERROR\_AUTH\_TRANSFERKEY\_NOT\_EXIST | 3033       | TransferKeyが有効ではありません。 |
| Auth (Login)    | Android, UNITY<br/>IOS | AUTH\_TOKEN\_LOGIN\_FAILED<br/>TCGB\_ERROR\_AUTH\_TOKEN\_LOGIN\_FAILED | 3101       |トークンログインに失敗しました。                        |
|                 | Android, UNITY<br/>IOS | AUTH\_TOKEN\_LOGIN\_INVALID\_TOKEN\_INFO<br/>TCGB\_ERROR\_AUTH\_TOKEN\_LOGIN\_INVALID\_TOKEN\_INFO | 3102       |トークン情報が有効ではありません。                       |
|                 | Android, UNITY<br/>IOS | AUTH\_TOKEN\_LOGIN\_INVALID\_LAST\_LOGGED\_IN\_IDP<br/>TCGB\_ERROR\_AUTH\_TOKEN\_LOGIN\_INVALID\_LAST\_LOGGED\_IN\_IDP | 3103       | 最近ログインしたIdPの情報がありません。                  |
| IdP Login       | Android, UNITY<br/>IOS | AUTH\_IDP\_LOGIN\_FAILED<br/>TCGB\_ERROR\_AUTH\_IDP\_LOGIN\_FAILED | 3201       | IdPログインに失敗しました。                       |
|                 | Android, UNITY<br/>IOS | AUTH\_IDP\_LOGIN\_INVALID\_IDP\_INFO<br/>TCGB\_ERROR\_AUTH\_IDP\_LOGIN\_INVALID\_IDP\_INFO | 3202       | IdP情報が有効ではありません(Consoleに該当するIdP情報がありません)。 |
| Add Mapping     | Android, UNITY<br/>IOS | AUTH\_ADD\_MAPPING\_FAILED<br/>TCGB\_ERROR\_AUTH\_ADD\_MAPPING\_FAILED | 3301       | マッピング追加に失敗しました。                         |
|                 | Android, UNITY<br/>IOS | AUTH\_ADD\_MAPPING\_ALREADY\_MAPPED\_TO\_OTHER\_MEMBER<br/>TCGB\_ERROR\_AUTH\_ADD\_MAPPING\_ALREADY\_MAPPED\_TO\_OTHER\_MEMBER | 3302       | 既に他のメンバーにマッピングされています。                      |
|                 | Android, UNITY<br/>IOS | AUTH\_ADD\_MAPPING\_ALREADY\_HAS\_SAME\_IDP<br/>TCGB\_ERROR\_AUTH\_ADD\_MAPPING\_ALREADY\_HAS\_SAME\_IDP | 3303       | 既に同じIdPにマッピングされています。                     |
|                 | Android, UNITY<br/>IOS | AUTH\_ADD\_MAPPING\_INVALID\_IDP\_INFO<br/>TCGB\_ERROR\_AUTH\_ADD\_MAPPING\_INVALID\_IDP\_INFO | 3304       | IdP情報が有効でありません(Consoleに該当するIdPの情報がありません)。|
|                 | Android, UNITY<br/>IOS | AUTH_ADD_MAPPING_CANNOT_ADD_GUEST_IDP<br/>TCGB_ERROR_AUTH_ADD_MAPPING_CANNOT_ADD_GUEST_IDP | 3305       | Guest IdPではAddMappingができません。 |
| Remove Mapping  | Android, UNITY<br/>IOS | AUTH\_REMOVE\_MAPPING\_FAILED<br/>TCGB\_ERROR\_AUTH\_REMOVE\_MAPPING\_FAILED | 3401       | マッピング削除に失敗しました。                         |
|                 | Android, UNITY<br/>IOS | AUTH\_REMOVE\_MAPPING\_LAST\_MAPPED\_IDP<br/>TCGB\_ERROR\_AUTH\_REMOVE\_MAPPING\_LAST\_MAPPED\_IDP | 3402       | 最後にマッピングされたIdPは削除することができません。              |
|                 | Android, UNITY<br/>IOS | AUTH\_REMOVE\_MAPPING\_LOGGED\_IN\_IDP<br/>TCGB\_ERROR\_AUTH\_REMOVE\_MAPPING\_LOGGED\_IN\_IDP | 3403       | 現在ログイン中のIdPです。                    |
| Logout          | Android, UNITY<br/>IOS | AUTH\_LOGOUT\_FAILED<br/>TCGB\_ERROR\_AUTH\_LOGOUT\_FAILED | 3501       | ログアウトに失敗しました。                          |
| Withdrawal      | Android, UNITY<br/>IOS | AUTH\_WITHDRAW\_FAILED<br/>TCGB\_ERROR\_AUTH\_WITHDRAW\_FAILED | 3601       | 退会に失敗しました。                            |
| Not Playable    | Android, UNITY<br/>IOS | AUTH\_NOT\_PLAYABLE<br/>TCGB\_ERROR\_AUTH\_NOT\_PLAYABLE | 3701       | プレイできない状態です(メンテナンスまたはサービス終了など)。       |
| Auth(Unknown)   | Android, UNITY<br/>IOS | AUTH\_UNKNOWN\_ERROR<br/>TCGB\_ERROR\_AUTH\_UNKNOWN\_ERROR | 3999       | 不明なエラーです(定義されていないエラー)。          |
| Purchase        | Android, UNITY<br/>IOS | PURCHASE\_NOT\_INITIALIZED<br/>TCGB\_ERROR\_PURCHASE\_NOT\_INITIALIZED | 4001       | Gamebase PurchaseAdapterが初期化されていませんでした。  |
|                 | Android, UNITY<br/>IOS | PURCHASE\_USER\_CANCELED<br/>TCGB\_ERROR\_PURCHASE\_USER\_CANCELED | 4002       | 購入がキャンセルされました。                            |
|                 | Android, UNITY<br/>IOS | PURCHASE\_NOT\_FINISHED\_PREVIOUS\_PURCHASING<br/>TCGB\_ERROR\_PURCHASE\_NOT\_FINISHED\_PREVIOUS\_PURCHASING | 4003       | 前回の購入が完了していません。                      |
|                 | Android, UNITY<br/>IOS | PURCHASE\_NOT\_ENOUGH\_CASH<br/>TCGB\_ERROR\_PURCHASE\_NOT\_ENOUGH\_CASH | 4004       | 該当するストアのcashが足りないため決済することができません。           |
|                 | Android, UNITY<br/>IOS | PURCHASE\_NOT\_SUPPORTED\_MARKET<br/>TCGB\_ERROR\_PURCHASE\_NOT\_SUPPORTED\_MARKET | 4010       | このストアには対応しておりません。                        |
|                 | Android, UNITY<br/>IOS | PURCHASE\_EXTERNAL\_LIBRARY\_ERROR<br/>TCGB\_ERROR\_PURCHASE\_EXTERNAL\_LIBRARY\_ERROR | 4201       | 外部IAPライブラリーのエラーです。                    |
|                 | Android, UNITY<br/>IOS | PURCHASE\_UNKNOWN\_ERROR<br/>TCGB\_ERROR\_PURCHASE\_UNKNOWN\_ERROR | 4999       | 不明な購入エラーです。                         |
| Push            | Android, UNITY<br/>IOS | PUSH\_EXTERNAL\_LIBRARY\_ERROR<br/>TCGB\_ERROR\_PUSH\_EXTERNAL\_LIBRARY\_ERROR | 5101       | 外部ライブラリーのエラーです。                        |
|                 | Android, UNITY<br/>IOS | PUSH\_ALREADY\_IN\_PROGRESS\_ERROR<br/>TCGB\_ERROR\_PUSH\_ALREADY\_IN\_PROGRESS\_ERROR | 5102       | 前回のPush APIの呼び出しが完了していません。             |
|                 | Android, UNITY<br/>IOS | PUSH\_UNKNOWN\_ERROR<br/>TCGB\_ERROR\_PUSH\_UNKNOWN\_ERROR | 5999       | 不明なPushエラーです(定義されていないPushエラー)。     |
| UI              | Android, UNITY<br/>IOS | UI\_UNKNOWN\_ERROR<br/>TCGB\_ERROR\_UI\_UNKNOWN\_ERROR | 6999       | 不明なエラーです(定義されていないエラー)。           |
| Server          | Android, UNITY<br/>IOS | SERVER\_INTERNAL\_ERROR<br/>TCGB\_ERROR\_SERVER\_INTERNAL\_ERROR | 8001       | サーバー内部エラー                                 |
|                 | Android, UNITY<br/>IOS | SERVER\_REMOTE\_SYSTEM\_ERROR<br/>TCGB\_ERROR\_SERVER\_REMOTE\_SYSTEM\_ERROR | 8002       | サーバーで外部連携中にエラーが発生しました。                       |
|                 | Android, UNITY<br/>IOS | SERVER\_UNKNOWN\_ERROR<br/>TCGB\_ERROR\_SERVER\_UNKNOWN\_ERROR | 8999       | サーバーで不明なエラーが発生しました。                          |

<br/>
<br/>


## Server
| Module  | Error Code            | Description                              |
| ------- | --------------------- | ---------------------------------------- |
| Common  | -4000001<br/>-4000006 | 正しくないパラメータータイプでのAPI呼び出し <br/>例) パラメーターはintタイプで宣言されているが、stringタイプのデータでAPIが呼び出されている |
|         | -4000002<br/>-4000004 | 必須パラメーターが抜けていたり、値がないとき                  |
|         | -4000003              | Request bodyに定義されていない値が転送された場合          |
|         | -4000005              | 必須パラメーターが抜けていたり、適切でない値で呼び出されたとき          |
|         | -4010001              | 正しくないアプリIDが呼び出されたとき                            |
|         | -4010002              | 正しくないアプリキーが呼び出されたとき                             |
|         | -4010003              | 認証されていないクライアントから認証が必要なAPIを呼び出した場合      |
|         | -4010004              | 正しくないシークレットキー(secret key)が呼び出されたとき                |
|         | -4060001              | HTTPのヘッダーにContent-Typeを間違って設定したとき             |
|         | -4060002              | 使用していない(depreated) APIバージョンを呼び出し                     |
|         | -4060003              | サポートされていないAPIバージョンを呼び出したか、無効なURIで呼び出した時 |
|         | -4090001 ~ 4          |内部DB関連のエラー                              |
|         | -4150001              | 正しくない形式のJSONデータを転送                      |
|         | -5000001 ~ 15         |内部システムエラー                                |
| Gateway | -4010202              | 正しくないアプリIDが呼び出されたとき                            |
|         | -4010203              | 有効でないアクセストークン                           |
|         | -4010204              | 利用停止/退会/アカウント流出など、有効でないユーザー            |
|         | -4040201              | 呼び出したAPIに対し、TOASTサービスが有効になっていないとき <br/>例) Leaderboardサービスを使用していない状態でGamebaseを通じてLeaderboardAPIを呼び出したとき、<br/>またはGamebaseそのものが有効になっていない場合 |
|         | -4040202              | 定義されていないAPIを呼び出した場合                   |
|         | -4120201              | 一部提供されるSANDBOXシステムから実際の環境サーバーアドレスでAPI呼び出し(または反対に呼び出し) <br/>- 該当エラー発生時は、サーバー呼び出しアドレスを確認する必要がある |
|         | -5000201 ~ 7          | Gateway内部システムエラー                        |
| Member  | -4000402              |ユーザーIDを間違って入力したとき                        |
|         | -4000403              | 正しくない会員をリクエストしたとき                         |
|         | -4000404              | 正しくないAuthをリクエストしたとき |
|         | -4000409              | 端末移行のために発行されたTransferAccount情報を同じ端末で使用 |
|         | -4040401              | 退会されているか、存在しない会員をリクエストしたとき                |
|         | -4040403              | 存在しないTransferAccountに対するリクエストの時 |
|         | -4100402              | 이미 사용된 TransferAccount 요청일 때  |
|         | -4100403              | 유효 기간이 만료된 TransferAccount 의 요청일 때  |
|         | -4100401              | 既に退会した会員をリクエストしたとき                      |
|         | -4220401              |ユーザーAuthデータが正常でないとき                 |
| IdP     | -4000901              | Block 된 게임 유저가 TransferAccount 검증 요청한 경우 |
|         | -4000920              | 내부에서 PASSWORD 암호화시 오류 발생. 계속 발생시 고객센터를 통해 문의 필요 |
|         | -4000921 ～ 2          | TransferAccount発行時、内部エラー発生。繰り返し発生する場合はサポートへ問い合わせ必要 |
|         | -4000923              | マニュアル(MANUAL)方式でPASSWORDを変更しようとする時、現在のPASSWORDと同じ文字列を入力 |
|         | -4000924              | Internal error. If this problem persists, please contact Customer Center. |
|         | -4000925              | マニュアル(MANUAL)方式でIDを変更しようとする時、現在使用中のIDを入力 |
|         | -4000927              | TransferAccountの有効性を検証時、 PASSWORDが間違っていた時 |
|         | -4040920              | TransferAccountの有効性を検証時、IDが存在しない時 |
|         | -5110920              | TransferAccount発行システムエラー。繰り返し発生する場合はサポートへ問い合わせ必要 |
| Coupon  | -100003               | 無効なクーポンコードをリクエストした場合                 |
|         | -100004               | リクエストにより手動ですでに終了処理したクーポンコード  |
|         | -100005               | すでに使用されたクーポン                              |
|         | -100006 ～ 10          | クーポン使用期間ではない場合                     |
|         | -100011               | クーポンを使用できる制限数を超過した場合        |
|         | -999999               | クーポンシステム内部エラー。繰り返し発生する場合はサポートへ問い合わせ必要 |
| IAP     | 5000                  | CONSUME FAILED                                 |
|         | 5018                  | すでに消費を行った決済                      |
|         | 1100                  | 必須パラメータが省略、または無効なパラメータを伝達      |
|         | 9999                  | UNKNOWN ERROR                                  |
