## 연습 1: 기본 Power Automate 클라우드 흐름 빌드 

 데이터에 연결하면 고객에게 고객 또는 사용자 질문과 관련된 최신 정보와
 통찰력을 제공하므로 회사에 가장 많은 이점을 제공합니다.

 이 연습에서는 새 토픽을 만들고, 간단한 Power Automate 작업을 추가하여
 외부 서비스에서 정보를 검색하고, 해당 데이터를 사용자에게 다시
 표시하는 과정을 살펴봅니다.

## 작업 1: 새 주제 만들기 

1.  이전 실습에서 만든 항목과의 혼동을 피 하려면 **지원 티켓**과 관련된
    항목을 **비활성화합니다**.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image3.png">

2.  Copilot Studio 작성 캔버스의 **주제** 페이지를 **열고 화면 상단의
    주제 추가 드롭다운** 을 클릭하고 **빈 공간에서** 옵션을 선택합니다.
    주제의 이름을 티켓 상태 확인으로 지정합니다.

3.  아래와 같이 사용자가 요청할 수 있는 **몇 가지** 트리거 문구를
    추가합니다

    ```
    What is the status of my ticket INC0008001
    Can you get me information on my ticket status
    Could you check the status of my ticket
    Status update on ticket INC0009005
    What’s happening with my ticket INC1234567
    ```
    ```
    내 항공권의 상태는 어떻게 되나요INC0008001 
    내 항공권 상태에 대한 정보를 얻을 수 있습니까?
    내 티켓의 상태를 확인할 수 있습니까?
    티켓 INC0009005에 대한 상태 업데이트
    내 항공권 INC1234567은 어떻게 되나요?
    ```
                                                

4.  새 **질문** 노드를 만들고 텍스트를 입력합니다 . 물론, 티켓의 상태를
    알려드릴 수 있습니다. 항공권 번호가 어떻게 되나요?

5.  \[Identify**\]에서** \[Create an Entity **of** type Regular
    expression (Regex)**\]을 선택하고 \[**Ticket Number\]라고 하며 다음
    패턴을 사용합니다{7}

6.  Var1 **변수 의 이름을** TicketNumber로 바꿉니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image6.png">

7.  **주제를 저장합니다**.


