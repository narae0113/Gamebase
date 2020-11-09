## Game > Gamebase > 콘솔 사용 가이드 > 고객센터

게임 운영 중 유저에게 인입된 문의를 처리할 수 있으며 그 외 고객센터 페이지를 통해 제공할 수 있는 공지사항, FAQ 등의 설정을 관리할 수 있습니다.
문의 처리시에 유저에게 발송될 이메일 설정 및 자주 쓰이는 답변을 템플릿으로 등록하여 활용하실 수도 있습니다.
> [참고]
> 이 메뉴를 이용하시려면 앱 - 고객센터 설정에서 Gamebase 제공 고객센터 항목을 선택하셔야 합니다.
>

## Inquiry

고객에게 인입된 문의를 처리하거나 조회할 수 있습니다.
그 외에도 고객이 문의를 등록하고자 할 때 필요한 접수 유형 항목을 설정할 수 있으며 문의가 처리되었을 때 유저에게 발송되는 Push 알람에 대한 설정도 가능합니다.

### Search Inquiry

검색 조건에 맞는 고객 문의 내역을 검색합니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_01_202009.png)

**검색 조건**

- **상태**: (필수) 고객 문의의 현재 처리 상태를 선택합니다.
- **접수 유형**: (필수) 고객 문의시 유저가 선택한 접수 유형 항목을 선택합니다. 접수 / 처리 완료 항목이 존재합니다.
- **접수 기간**: (필수)선택한 기간동안 인입된 문의를 조회합니다.
- **유저 ID**: 특정 유저의 문의를 검색하고자 할 경우 해당 유저ID를 입력합니다.

**검색 결과**

- **접수 유형**: 유저가 문의 등록시 선택한 접수 유형 항목
- **문의 제목**: 유저가 문의 등록시 입력한 문의 제목
- **접수일**: 유저의 문의 등록 일시
- **처리일**: 담당자가 인입된 문의를 처리한 일시
- **상태**: 인입된 문의의 현재 처리 상태

#### 1. 접수 유형 관리
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_02_202009.png)

유저가 문의 등록시 선택할 수 있는 접수 유형 항목을 관리할 수 있습니다.
지원하는 언어별로 등록이 가능하며 항목별 최대 글자수는 20자입니다.
표시되는 순서대로 유저에게 목록이 표시되며 해당순서는 드래그앤 드랍을 이용하여 목록 내에서 변경이 가능합니다.
> [참고]
> 지원 언어 선택 현황은 앱 - 고객센터 설정에서 확인할 수 있습니다.

#### 2. 답변 발송 설정
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_05_202009.png)

문의에 대한 처리가 완료되었을 경우 유저에게 Push 메시지를 통해 알림을 발송하고자 할 경우에 해당 기능을 설정할 수 있습니다.
사용하고자 할 경우에 상단에 발송여부를 체크하면 유저에게 처리완료 시 완료 Push알람이 함께 전송됩니다.
글로벌 서비스의 경우 원하는 언어를 추가로 등록하여 발송할 수 있으며 유저의 기기설정에 따라 맞는 언어설정으로 유저에게 푸시 알람이 전송되게 됩니다.
> [참고]
> 1. 이 기능을 사용하려면 TOAST Push 상품이 먼저 활성화되어 있어야 합니다.
> 2. 답변발송 설정의 언어선택의 경우 고객센터에서 지원되는 언어와 무관하게 Gamebase에서 지원되는 모든 언어를 등록할 수 있습니다.

### Inquiry details

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_03_202009.png)
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_04_202009.png)

유저에게 인입된 문의에 대하여 상세내용 확인 및 해당 문의에 대한 처리를 진행할 수 있습니다.

템플릿을 선택할 경우 고객센터 - 답변 템플릿 메뉴에서 설정한 템플릿 내용을 답변에서 바로 사용할 수 있으며 템플릿 내용 외에 Text editor를 이용하여 원하시는 모양대로 답변을 만들어 유저에게 전달할 수 있습니다.
유저 문의 답변시 파일첨부가 필요할 경우 최대 10MB 이내의 파일을 5개까지 첨부하여 유저에게 전달가능합니다.
이후 처리하기가 완료될 경우 문의 인입시 등록된 email을 통해 담당자가 작성한 내용이 유저에게 전달됩니다.
이 때 답변 발송 항목을 통해 문의 처리 완료 시 해당 유저에게 Push알람이 전송되는지에 대한 여부를 확인할 수 있습니다.
> [참고]
> ![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_06_202009.png)
> 로그인된 유저가 문의를 등록했을 경우 해당 유저에 대한 정보를 한 화면에서 조회하여 확인할 수 있습니다.
> 기존 회원 메뉴에서 사용했던 기능과 동일하게 유저정보를 조회할 수 있으므로 유저 문의대응시 필요한 정보를 한화면에서 편리하게 조회하여 사용하실 수 있습니다.

#### 1. 답변 발송 설정
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_05_202009.png)

문의에 대한 처리가 완료되었을 경우 유저에게 Push 메시지를 통해 알림을 발송하고자 할 경우에 해당 기능을 설정할 수 있습니다.
사용하고자 할 경우에 상단에 발송여부를 체크하면 유저에게 처리완료 시 완료 Push알람이 함께 전송됩니다.
글로벌 서비스의 경우 원하는 언어를 추가로 등록하여 발송할 수 있으며 유저의 기기설정에 따라 맞는 언어설정으로 유저에게 푸시 알람이 전송되게 됩니다.
> [참고1]
> 1. 이 기능을 사용하려면 TOAST Push 상품이 먼저 활성화되어 있어야 합니다.
> 2. 답변발송 설정의 언어선택의 경우 고객센터에서 지원되는 언어와 무관하게 Gamebase에서 지원되는 모든 언어를 등록할 수 있습니다.

> [참고2]
> 문의 처리가 완료된 고객 문의를 조회할 경우에는 문의 내역 및 처리 내역을 함께 조회할 수 있으며 처리 당시에 등록한 첨부파일이 있을 경우 해당항목을 클릭하여 다운이 가능합니다.


## FAQ

고객센터 페이지에서 제공되는 FAQ 항목에 대한 관리를 진행할 수 있습니다.

### Search FAQ

등록되어 있는 FAQ 항목에 대하여 검색할 수 있습니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_07_202009.png)

**검색 조건**

- **상태**: (필수) FAQ의 노출 형태를 선택합니다. 노출 / 비노출 항목을 선택할 수 있습니다.
- **유형**: (필수) FAQ의 유형을 선택하여 검색할 수 있습니다. 선택항목은 FAQ 유형 관리에서 등록된 내용을 기준으로 표시됩니다.
- **질문+답변**: 질문 또는 답변에 특정한 키워드를 포함한 FAQ를 검색하고자 할 때 사용합니다. 다른 언어로 등록된 내용을 등록하고자 할 경우에는 검색할 언어를 지정한 후에 검색합니다.

**검색 결과**

- **자주하는 질문**: FAQ가 자주하는 질문란에 들어가있는지에 대한 여부를 표시합니다.
- **유형**: 등록된 FAQ의 분류 유형을 표시합니다.
- **제목**: FAQ의 질문 제목입니다.
- **수정자**: FAQ를 마지막으로 등록 또는 수정한 유저의 정보를 보여줍니다.
- **수정일**: FAQ가 마지막으로 등록 또는 수정된 날짜 정보를 보여줍니다.
- **상태**: FAQ가 현재 표시되고 있는지 여부를 보여줍니다. 노출 중 / 비노출 상태가 있습니다.

#### FAQ 유형 관리
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_09_202009.png)

FAQ 등록 또는 수정시 선택할 수 있는 유형을 관리할 수 있습니다.
지원하는 언어별로 등록이 가능하며 항목별 최대 글자수는 20자입니다.
표시되는 순서대로 표시되며 해당순서는 드래그앤 드랍을 이용하여 목록 내에서 변경이 가능합니다.
> [참고]
> 지원 언어 선택 현황은 앱 - 고객센터 설정에서 확인할 수 있습니다.

### Register or Update FAQ
FAQ를 등록하거나 또는 기존에 등록된 FAQ정보를 수정할 수 있습니다.
등록 또는 수정 시 변경할 수 있는 항목은 모두 동일합니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_08_202009.png)

#### 1. 상태
등록 또는 수정하고자 하는 FAQ의 노출 상태를 선택합니다.
노출 / 비노출 항목이 있으며 고객센터 페이지에서 실제 유저에게 노출할지에 대한 여부를 선택하면 됩니다.

#### 2. 유형
FAQ 유형 관리에서 등록된 유형을 기반으로 등록 또는 수정하고자 하는 FAQ의 유형을 선택합니다.

#### 3. 자주하는 질문
고객센터 페이지에서 자주하는 질문란에 해당 질문을 표시할 지에 대한 여부를 체크합니다.

#### 4. 질문
FAQ 질문 내용을 입력합니다.
> [참고]
> 앱 - 고객센터에서 설정한 지원 언어들은 모두 입력해야 등록이 가능합니다.

####. 5. 답변
FAQ 질문에 대한 답변 내용을 입력합니다.
Text Editor를 통해 원하는 형태로 답변을 입력할 수 있으며 해당형태 그대로 웹페이지에 노출됩니다.
> [참고]
> 앱 - 고객센터에서 설정한 지원 언어들은 모두 입력해야 등록이 가능합니다.

## Notice

고객센터 페이지에서 제공할 공지사항에 대한 관리를 진행할 수 있습니다.

### Search Notice

등록되어 있는 공지사항 목록에 대하여 검색할 수 있습니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_10_202009.png)

**검색 조건**

- **검색 유형**: (필수) 공지사항의 검색 유형을 선택할 수 있습니다. 기본으로 상태가 선택되어 있으며 노출일을 기준으로 검색하고자 할 경우 해당항목을 선택한 후에 동일하게 검색할 수 있습니다.
- **상태**: (필수) 위 검색 유형에서 기본으로 선택되어 있는 항목으로 현재 공지의 노출 상태를 기준으로 검색합니다. 예정 / 노출 중 / 종료 항목을 선택할 수 있습니다.
- **노출일**: 검색 유형에서 노출일 항목을 선택헀을 경우 설정할 수 있으며 선택된 노출일을 기준으로 보여지는 공지사항 목록을 검색하여 볼 수 있습니다.
- **제목+내용**: 제목 또는 내용에 특정한 키워드를 포함한 공지사항을 검색하고자 할 때 사용합니다. 다른 언어로 등록된 내용을 등록하고자 할 경우에는 검색할 언어를 지정한 후에 검색합니다.

**검색 결과**
- **상단 고정**: 해당 공지사항이 상단 고정란에 들어가있는지에 대한 여부를 표시합니다.
- **유형**: 등록된 공지사항의 분류 유형을 표시합니다.
- **제목**: 공지사항의 제목입니다.
- **노출일(UTC+9)**: 공지사항이 노출될 때 실제 노출할 등록일(표시일)을 보여줍니다.
- **노출 기간**: 해당 공지사항의 노출 기간을 표시합니다.
- **상태**: 공지사항의 현재 진행여부 보여줍니다. 예정 / 노출 중 / 종료 상태가 있습니다.

#### 말머리 관리
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_11_202009.png)

공지사항 등록 또는 수정시 선택할 수 있는 말머리를 관리할 수 있습니다.
지원하는 언어별로 등록이 가능하며 항목별 최대 글자수는 20자입니다.
표시되는 순서대로 표시되며 해당순서는 드래그앤 드랍을 이용하여 목록 내에서 변경이 가능합니다.
> [참고]
> 지원 언어 선택 현황은 앱 - 고객센터 설정에서 확인할 수 있습니다.

### Register or Update Notice
새로운 공지사항을 등록하거나 기존에 등록된 공지사항 정보를 수정할 수 있습니다.
등록 또는 수정 시 변경할 수 있는 항목은 모두 동일합니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_15_202009.png)
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_16_202009.png)

#### 1. 노출일
공지사항을 노출하고자 하는 기간을 설정합니다.

#### 2. 표시 시각
공지사항 내용을 표시할 때 실제 유저에게 보여질 날짜를 선택합니다.

#### 3. 말머리
공지사항의 말머리를 선택합니다.

#### 4. 상단 고정
공지사항을 상단에 고정하여 항상 노출될 수 있도록 합니다.

#### 5. 제목
공지사항의 제목을 입력합니다.

#### 6. 내용
공지사항에 대한 내용을 입력합니다.
Text Editor를 통해 원하는 형태로 답변을 입력할 수 있으며 해당형태 그대로 웹페이지에 노출됩니다.
> [참고]
> 앱 - 고객센터에서 설정한 지원 언어들은 모두 입력해야 등록이 가능합니다.

#### 7. 파일 첨부
해당 공지사항에 함께 노출할 파일을 첨부하여 올릴 수 있습니다.
10MB 이내의 파일을 최대 5개까지 첨부가능합니다.
첨부파일들은 공지사항에 함께 노출되며 클릭 시 다운로드가 가능합니다.

## Answer template

고객 문의 처리 시 반복입력을 자주 할 경우 템플릿을 사용하여 처리할 수 있도록 기능을 지원합니다.

### Search Template
현재 등록된 템플릿 리스트를 표시하며, 우측 상단에 검색어를 입력하여 현재 등록된 템플릿을 검색할 수 있습니다.
![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_12_202009.png)

**결과**
- **템플릿명**: 문의 처리시에 템플릿 항목에 노출되어 선택할 수 있는 템플릿명입니다.
- **수정자**: 답변 템플릿을 마지막으로 등록 또는 수정한 유저의 정보를 보여줍니다.
- **수정일**: 답변 템플릿이 마지막으로 등록 또는 수정된 날짜 정보를 보여줍니다.

### Register or Update Template
답변 템플릿을 새롭게 등록하거나 기존에 등록된 답변 템플릿 정보를 수정할 수 있습니다.
등록 또는 수정 시 변경할 수 있는 항목은 모두 동일합니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_13_202009.png)

#### 1. 템플릿명
문의 처리시에 템플릿 선택항목에 노출될 템플릿명을 입력합니다.

#### 2. 내용
문의 처리시 템플릿이 선택되었을 때 채워질 내용을 입력합니다.
Text editor를 이용하여 자유롭게 입력이 가능하며 입력된 내용이 그대로 문의 처리시 템플릿을 선택하면 동일하게 적용됩니다.

## Email Config
문의 처리가 완료되었을 경우 유저에게 발송할 이메일 형식을 설정할 수 있습니다.
최초에 활성화 시켰을 경우 기본 템플릿이 제공되며 이후 Text editor를 통해 원하는 형태로 얼마든지 수정하실 수 있습니다.

테스트 발송 기능이 제공되며 해당 기능을 통해 현재 입력한 템플릿을 이용하여 실제 유저에게 어떤 형태로 전송되는지 미리 확인할 수 있습니다.

![gamebase_ban_01_201812](https://static.toastoven.net/prod_gamebase/Operators_Guide/gamebase_customer_inquiry_14_202009.png)

> [참고]
> 발신 주소에 설정된 이메일이 SPF 레코드가 설정되지 않았을 경우에는 수신거부가 될 가능성이 있으므로 아래 값을 DNS의  TXT레코드에 먼저 등록 후 발신주소에 설정해 주셔야 합니다.
> 추가 값 : v=spf1 include:_spfblocka.toast.com ~all