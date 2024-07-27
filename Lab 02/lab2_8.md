# 코드 보기 및 Power Fx

이제 Microsoft Copilot Studio의 작성 기본 사항에 더 익숙해졌으므로
Copilot 환경을 설정하고 추가로 사용자 지정하는 데 사용할 수 있는 몇 가지
확장 기능을 살펴볼 수 있습니다. 다음 섹션에서는 **전문 개발자를 위한**
코드 보기와 **Power Fx**(Microsoft Power Platform 제작자 및 전문
개발자용)의 두 가지 기능에 대해 설명합니다.

Microsoft Copilot Studio에는 토픽 숨김 코드를 볼 수 있는 기능이
있습니다. 이 기능은 고급 제작자 및 프로 코드 개발자에게 매우 유용하며,
웹 브라우저 내에서 직접 구문을 보고 편집할 수 있으며, 저장하면 구문이
그래픽 작성 캔버스에 즉시 표시됩니다. 결과적으로 여러 작업을 복사하고
편집하는 프로세스가 더 빠르고 쉬워집니다. 일부 특정 작업은 코드 편집기
보기에서만 사용할 수 있습니다.

## 작업 1: 코드 편집기에 액세스

다음 단계에 따라 코드 편집기에 액세스합니다.

1.  이 실습에서 작업한 Check **Order Status(주문 상태 확인**)라는 항목을
    엽니다.

2.  항목의 오른쪽 상단에서 **저장** 아이콘 옆에 있는 확장된(**\...**)
    메뉴를 선택한 다음 **다음 스크린샷과 같이** 코드 편집기 열기를
    선택합니다.
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2002/media/image42.png">


3.  코드 보기(YAML 코드)에서 대화 상자를 볼 수 있는 코드 편집기가
    열립니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2002/media/image43.png">

4.  이 기능을 탐색한 후 오른쪽 위에 있는 **코드 편집기 닫기를**
    선택합니다.

## Microsoft Copilot Studio에서 Power Fx 사용

Power Fx는 Microsoft Copilot Studio에서 사용할 수 있습니다. Power Fx를
사용하면 제작자가 현재 Microsoft Copilot Studio 작성 캔버스 내에서
Microsoft Power Apps 또는 Dataverse의 캔버스 앱에서 수행하는 것과 유사한
기능을 추가할 수 있습니다. Power Fx는 **메시지** 및 **질문** 노드,
**변수 값 설정 노드를 사용할 때 및** 조건**,** 작업**,** 질문 동작
**구성 및** 적응형 카드**와 같은 다른 영역에서** 사용할 수 있습니다. 이
기능을 사용하면 대화형 인터페이스 내에서 고객 및 사용자에게 표시되는
데이터를 보다 효과적으로 제어할 수 있습니다. 또한 Microsoft Copilot
Studio의 런타임에서 일반적인 작업을 수행할 수 있습니다.

다음 작업은 변수 내에서 Power Fx를 사용한 다음 사용자에게 값을 표시하는
기본 시나리오를 살펴봅니다.

## 작업 2: Power Fx를 사용하여 날짜 표시 방법 수정

Power Fx를 사용하여 날짜 표시 방법을 수정하려면 다음 단계를 수행합니다.

1.  이 실습 중에 작업한 **주문 상태 확인 항목을** 엽니다.

2.  \[Check **condition\] 브랜치**에서 **\[Set a variable value**\]
    노드를 추가하고 \[**Create a new variable\]을** 선택합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2002/media/image44.png">

3.  새 변수를 선택하면 **오른쪽에 변수 속성** 창이 열립니다. 변수의
    이름을 OrderDeliveryDate로 변경합니다.
    
    변수 값 설정 **노드**의 **To Value**에서 플라이아웃 메뉴를 선택한
    다음 **Formula**를 선택하여 수식 입력 **패널 을 엽니다** . 필요에
    따라 **수식 입력** 창 의 오른쪽 상단에 있는 **확장** 아이콘을
    선택하여 수식을 입력할 수 있는 영역을 확대하고 아래 항목을 붙여넣을
    수 있습니다.

4.  수식 입력줄에 다음 함수를 입력하고 **다음과 같이** 삽입을
    선택합니다.

    ```
    Text(
        DateAdd(
            Now(),
            2,
            TimeUnit.Days
        ),
        DateTimeFormat.LongDate
    )
    ```

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2002/media/image45.png">


 이 함수는 기술적으로 특정 날짜 및 시간 형식(예: 2024년 5월 31일 오전
 8:00)이 있는 오늘 날짜와 시간을 사용하고 2일을 추가한 다음 긴 날짜
 형식(예: 2024년 5월 31일 금요일)으로 형식을 지정합니다. 이 방법은
 사용자에게 친숙한 간단한 날짜 형식을 표시하거나 날짜를 텍스트 형식의
 문자열로 저장하려는 경우에 중요합니다.

5.  데모를 위해 Check 경로**의 마지막** 메시지를 **업데이트 하여 구성한
    news 변수를 사용할** 수 있습니다.

    ```
    Your order {Topic.OrderNumber} should be delivered by {Topic.OrderDeliveryDate}.
    ```
    ```
    당신의 주문 {Topic.OrderNumber} 이 {Topic.OrderDeliveryDate} 까지 배송될 것입니다.
    ```

6.  **저장을** 클릭합니다.

7.  테스트 창을 열어 Copilot을 테스트하고, 주제를 트리거한 다음, 주제
    프롬프트에 따라 **다음** 스크린샷과 같이 메시지 노드에 도달합니다.

    ```
    Hello, can you please check the status of my order ORD-001342?
    ```
    ```
    안녕하세요. 제 주문 ORD-001342의 상태를 확인해 주시겠습니까?
    ```
  
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2002/media/image46.png">
    
 축하합니다. Microsoft Copilot Studio 통합 저작 기능의 중앙 저작 기능에 대한 모든 랩을 성공적으로 마쳤습니다.
