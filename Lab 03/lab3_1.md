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

## 작업 2: Power Automate 클라우드 흐름 만들기 

1.  아래 스크린샷과 같이 **Question** 노드 아래의 **(+)** 새 노드 버튼을
    **클릭하고** Call an action(액션 호출)을 **선택한 다음 Basic
    actions(기본 액션**) 아래에서 **Create a flow(플로우 생성**)를
    클릭합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image7.png">

2.  그러면 새 브라우저 창에서 **Power Automate**가 열리고 아래
    스크린샷과 같이 Copilot Studio와 상호 작용하기 위한 새 Power
    Automate 클라우드 흐름에 대한 스캐폴딩 사전 및 사후 작업이
    포함됩니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image8.png">

 **전문가 팁:** 오른쪽 상단 모서리에 있는 Power Automate에서 **New Designer**이 활성화 되었는지 확인하세요.


3.  When Copilot Studio calls a flow trigger(Copilot Studio가 흐름
    트리거를 호출할 때**)를 클릭하고** 왼쪽 창에서 **Add an input(입력
    추가)을 클릭합니다.**
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image11.png">

4.  Text **형식의** 입력을 **추가하고** TicketNumber라고 합니다.
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image12.png">

5.  트리거와 방금 추가한 작업 사이에 **있는 작업 추가 를** 클릭합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image13.png">

     **참고**: 다음 단계에서 ServiceNow 환경이 활성화되지 않고 연결을 제대로 설정할 수 없는 경우(일반적으로 레코드 유형이 8단계에서 인시던트를 옵션으로 포함하는 목록을 반환하지 않는 경우) 11단계로 건너뜁니다.

6.  검색 창에서 ServiceNow List Records를 검색 하고 List Records**를
    선택합니다.**

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image14.png">

7.  ServiceNow **에 대한 연결을 만듭니다**.연결의 이름을 고유한
    항목(예: ServiceNow - {Your User Name})  으로 지정합니다.인스턴스를 https://dev261120.service-now.com 로
    설정 하고, 사용자 이름을 **CopilotStudioServiceAccount**로 설정 하고,  암호를 **다음으로** 설정합니다.

    ```
    asdfjasldfja;ldkfj;adfadf
    ```

     그런 다음 **새로 만들기를 선택합니다.**

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image15.png">

8.  이제 **Record Type(레코드 유형**)에서 Incident(인시던트)를
    선택합니다 (목록에서 Incident(인시던트를 더 쉽게 찾을 수 있도록
    검색할 수 있음)).
    Advanced parameters(고급 매개변수**)에서** Show all(모두 표시**)을
    선택합니다**.
    시스템 참조 표시(Display System References**)를** 예(Yes)로 설정하여
    실제 값을 표시합니다.

     Exclude Reference 링크를 **yes**로 둡니다.\
     쿼리**에** numberCONTAINS를 입력하고 동적 콘텐츠(⚡아이콘)에서
     TicketNumber 입력을 .
     **numberCONTAINS**와 **참조하는** 변수 **사이에** 공백이 없는지
     확인합니다.또는 Query **필드에** 아래를 붙여넣을 수도 있습니다.

    ```
    numberCONTAINS@{triggerBody()?['text']}
    ```

    제한을 1로 설정합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image16.png">

9.  클라우드 흐름에서 **Power Virtual Agents에 값 반환 작업을** 클릭하고
    **텍스트** 유형의 **출력을 추가하고** SNTicketInfo라고 부릅니다**.**

10. 출력 **값**의 경우 수식 버튼 **fx** 를 사용하여 List Records
    본문에서 결과 배열의 첫 번째로 반환된 레코드의 문자열 버전을
    가져옵니다.
    아래 수식을 붙여넣고 추가를 선택합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image17.png">

    ```
    string(first(outputs('List_Records')?['body/result']))
    ```
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image18.png">

11. **선택적 단계(ServiceNow가 작동하지 않는 경우):** 출력 **값**에 아래
    하드코딩된 페이로드를 붙여넣습니다. 이는 ServiceNow가 일반적으로
    반환하는 내용의 예를 나타냅니다.

    ```
    "parent": "",
        "made_sla": "true",
        "caused_by": "",
        "watch_list": "",
        "upon_reject": "Cancel all future Tasks",
        "sys_updated_on": "2018-12-12 23:18:55",
        "child_incidents": "0",
        "hold_reason": "",
        "origin_table": "",
        "task_effective_number": "INC0009005",
        "approval_history": "",
        "number": "INC0009005",
        "resolved_by": "",
        "sys_updated_by": "admin",
        "opened_by": "System Administrator",
        "user_input": "",
        "sys_created_on": "2018-08-31 21:35:45",
        "sys_domain": "global",
        "state": "New",
        "route_reason": "",
        "sys_created_by": "admin",
        "knowledge": "false",
        "order": "",
        "calendar_stc": "",
        "closed_at": "",
        "cmdb_ci": "",
        "delivery_plan": "",
        "contract": "",
        "impact": "1 - High",
        "active": "true",
        "work_notes_list": "",
        "business_service": "",
        "business_impact": "",
        "priority": "1 - Critical",
        "sys_domain_path": "/",
        "rfc": "",
        "time_worked": "",
        "expected_start": "",
        "opened_at": "2018-08-31 21:35:21",
        "business_duration": "",
        "group_list": "",
        "work_end": "",
        "caller_id": "David Miller",
        "reopened_time": "",
        "resolved_at": "",
        "approval_set": "",
        "subcategory": "Email",
        "work_notes": "2018-12-12 23:18:42 - System Administrator (Work notes)\nupdated the priority to high based on the criticality of the Incident.\n\n",
        "universal_request": "",
        "short_description": "Email server is down.",
        "correlation_display": "",
        "delivery_task": "",
        "work_start": "",
        "assignment_group": "",
        "additional_assignee_list": "",
        "business_stc": "",
        "cause": "",
        "description": "Unable to send or receive emails.",
        "origin_id": "",
        "calendar_duration": "",
        "close_notes": "",
        "notify": "Do Not Notify",
        "service_offering": "",
        "sys_class_name": "Incident",
        "closed_by": "",
        "follow_up": "",
        "parent_incident": "",
        "sys_id": "ed92e8d173d023002728660c4cf6a7bc",
        "reopened_by": "",
        "incident_state": "New",
        "urgency": "1 - High",
        "problem_id": "",
        "company": "",
        "reassignment_count": "0",
        "activity_due": "2018-12-13 01:18:55",
        "assigned_to": "",
        "severity": "3 - Low",
        "comments": "",
        "approval": "Not Yet Requested",
        "sla_due": "UNKNOWN",
        "comments_and_work_notes": "2018-12-12 23:18:42 - System Administrator (Work notes)\nupdated the priority to high based on the criticality of the Incident.\n\n",
        "due_date": "",
        "sys_mod_count": "3",
        "reopen_count": "0",
        "sys_tags": "",
        "escalation": "Normal",
        "upon_approval": "Proceed to Next Task",
        "correlation_id": "",
        "location": "",
        "category": "Software"
    }
    
    ```

12. 구름 흐름이 거의 완료되었습니다. 모범 사례로 이동하기 전에 **이름을
    바꿔**야 하므로 Copilot Studio와 관리자가 쉽게 찾을 수 있습니다.
    아래 스크린샷과 같이 템플릿 **제목**을 클릭하고 이름을 Get Ticket
    Status {YourUserName}으로 바꿉니다.

13. 게시를 **클릭하고** 아래 스크린샷과 같이 녹색 배너가 표시될 때까지
    잠시 기다립니다.

     **전문가 팁:** 게시 버튼이 보이지 않으면 저장을 선택하세요.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image19.png">

    Power Automate에서 작업을 완료했습니다. 이제 Copilot Studio로 다시 전환해 보겠습니다.

## 작업 3: Copilot Studio에서 Power Automate 클라우드 흐름 호출

1.  Copilot Studio에서 기존 주제를 열고 아래와 같이 흐름의 맨 아래로
    돌아갑니다. **작업 호출을 클릭하면** 기본 작업 탭 **아래의 목록에
    새로운 Power Automate 클라우드 흐름이 표시됩니다** . 목록에서 **티켓
    상태 받기** 흐름을 선택합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image20.png">

    **전문가 팁:** 생성한 클라우드 흐름이 보이지 않으면 주제를 저장하고 페이지를 새로 고쳐 다시 시도하세요.

2.  티켓 상태 받기 **플로를 선택하면 새** 작업 **노드가 자동으로
    추가되는** 것을 볼 수 있습니다.흐름에 입력이 필요한 경우 값을 선택하도록 요청합니다.
    이전 단계에서 만든 흐름에는 **TicketNumber** 입력이 필요하므로
    사용자로부터 값이 저장된 변수(랩 이전 단계의 **TicketNumber**)를
    선택하여 이 입력을 Power Automate 작업에 추가해야 합니다.

3.  Enter or select 값을 **선택하고 이 랩의 이전 단계에서 만든**
    TicketNumber **변수를 선택합니다** . 이제 Power Automate 흐름에
    연결되고 Power Automate의 결과를 **SNTicketInfo** 변수에 출력합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image21.png">

    **전문가 팁**
    • 통합에서 대기 시간이 예상되는 경우 작업 속성으로 이동하여 대기 시간 메시지를 추가합니다
      (예: 이 세부 정보를 가져오고 있습니다. 잠시만요...)
    • Power Automate에서 클라우드 흐름을 호출하고 실행하는 추가 대기 시간을 피하기 위해 Microsoft Copilot Studio에서 직접 HTTP 요청 및 커넥터를 사용하는 것을 고려하세요.

4.  ServiceNow**는 인시던트의 전체 세부 정보를 기술** 적인 JSON 형식으로
    반환**하므로** Copilot Studio가 스키마를 기반으로 콘텐츠를 완전히
    이해할 수 있도록 구문 분석해야 합니다.\
    이렇게 하려면 **변수 관리를 선택한** 다음, **값 구문 분석을
    선택합니다**.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image22.png">

     JSON을 구문 분석하려면 ServiceNow의 Rest API 탐색기를 사용하여 본문의
     구조를 가져오거나 샘플 페이로드에서 스키마를 가져올 수 있습니다.
     실습을 위해 아래에 샘플 ServiceNow 데이터를 제공하고 있습니다.
    
    아래 텍스트를 복사하는 데 어려움이 있으면 Lab 파일의 Misc 폴더로 이동하여 ServiceNow Sample JSON Payload.txt를 엽니다.

    ```
    "parent": "",
        "made_sla": "true",
        "caused_by": "",
        "watch_list": "",
        "upon_reject": "Cancel all future Tasks",
        "sys_updated_on": "2018-12-12 23:18:55",
        "child_incidents": "0",
        "hold_reason": "",
        "origin_table": "",
        "task_effective_number": "INC0009005",
        "approval_history": "",
        "number": "INC0009005",
        "resolved_by": "",
        "sys_updated_by": "admin",
        "opened_by": "System Administrator",
        "user_input": "",
        "sys_created_on": "2018-08-31 21:35:45",
        "sys_domain": "global",
        "state": "New",
        "route_reason": "",
        "sys_created_by": "admin",
        "knowledge": "false",
        "order": "",
        "calendar_stc": "",
        "closed_at": "",
        "cmdb_ci": "",
        "delivery_plan": "",
        "contract": "",
        "impact": "1 - High",
        "active": "true",
        "work_notes_list": "",
        "business_service": "",
        "business_impact": "",
        "priority": "1 - Critical",
        "sys_domain_path": "/",
        "rfc": "",
        "time_worked": "",
        "expected_start": "",
        "opened_at": "2018-08-31 21:35:21",
        "business_duration": "",
        "group_list": "",
        "work_end": "",
        "caller_id": "David Miller",
        "reopened_time": "",
        "resolved_at": "",
        "approval_set": "",
        "subcategory": "Email",
        "work_notes": "2018-12-12 23:18:42 - System Administrator (Work notes)\nupdated the priority to high based on the criticality of the Incident.\n\n",
        "universal_request": "",
        "short_description": "Email server is down.",
        "correlation_display": "",
        "delivery_task": "",
        "work_start": "",
        "assignment_group": "",
        "additional_assignee_list": "",
        "business_stc": "",
        "cause": "",
        "description": "Unable to send or receive emails.",
        "origin_id": "",
        "calendar_duration": "",
        "close_notes": "",
        "notify": "Do Not Notify",
        "service_offering": "",
        "sys_class_name": "Incident",
        "closed_by": "",
        "follow_up": "",
        "parent_incident": "",
        "sys_id": "ed92e8d173d023002728660c4cf6a7bc",
        "reopened_by": "",
        "incident_state": "New",
        "urgency": "1 - High",
        "problem_id": "",
        "company": "",
        "reassignment_count": "0",
        "activity_due": "2018-12-13 01:18:55",
        "assigned_to": "",
        "severity": "3 - Low",
        "comments": "",
        "approval": "Not Yet Requested",
        "sla_due": "UNKNOWN",
        "comments_and_work_notes": "2018-12-12 23:18:42 - System Administrator (Work notes)\nupdated the priority to high based on the criticality of the Incident.\n\n",
        "due_date": "",
        "sys_mod_count": "3",
        "reopen_count": "0",
        "sys_tags": "",
        "escalation": "Normal",
        "upon_approval": "Proceed to Next Task",
        "correlation_id": "",
        "location": "",
        "category": "Software"
    }
    ```

5.  이제 Power Automate 흐름 작업에서 **SNTicketInfo** 변수를 선택하여
    구문 분석할 값을 선택해야 합니다.

6.  다음으로 **데이터 유형을** 샘플 데이터에서**로 선택합니다**\
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image23.png">

7.  이제 샘플 JSON에서 스키마 가져오기 를 선택하고 **확인을** 선택한
    **후 위 단계에서 제공된 JSON 샘플에 붙여넣** 습니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image24.png">


8.  그런 다음 나중에 사용자를 위해 구문 분석된 레코드를 저장할 변수를
    설정합니다.
    SNTicketInfoParsed라는 변수를 만듭니다. 해당 유형은 스키마(레코드)에
    따라 자동으로 설정됩니다.

9.  이제 응답을 추가하여 부조종사 사용자에게 티켓의 상태를 알려주는
    형식화된 응답을 제공합니다. **(+)**를 클릭하여 새 노드를 추가하고
    **메시지 보내기를 선택합니다**.
    **명령 모음을 사용하거나 텍스트를 \*\*로 둘러싸서 주요 정보를** 굵게
    표시합니다.

    ```
    The status of ticket {Topic.TicketNumber}
    ({Topic.SNTicketInfoParsed.short_description}) is {Topic.SNTicketInfoParsed.state}
    ```
    Copilot Studio와 일부 채널은 간단한 서식을 위한 Markdown을 지원합니다.
    
    **전문가 팁:** Copilot Studio와 일부 채널은 간단한 서식을 위한 Markdown을 지원합니다.
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image25.png">
    
    위의 샘플 JSON을 보고 어떤 데이터가 어떤 값으로 반환되는지 확인할 수
    있지만, 아래는 메시지를 구조화하는 데 도움이 되도록 나중에 조회할 티켓의
    스크린샷입니다.
    
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image26.png">

10. 대화를 종료하려면 **주제 관리를** **선택하고 다른 주제로 이동하여**
    대화 종료를 **선택합니다**.

11. **주제를 저장하고** 부조종사를 테스트하십시오.
    
    ```
    What is the status of my ticket INC0007001?
    ```
    
    ```
    내 항공권의 티켓 INC0007001의 상태는 어떤가요?
    ```

12. 항공권 번호의 상태를 확인하십시오**INC0007001**

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image27.png">
    
    Power Automate 클라우드 흐름과 Microsoft Copilot Studio에서 이 흐름을
    사용하여 외부 서비스의 실시간 데이터를 사용자에게 제공하는 새 토픽을
    성공적으로 만들었습니다!

## 작업 4: 적응형 카드에 ServiceNow 티켓 정보 표시

1.  티켓 상태 확인 **주제로** 이동합니다.

2.  **메시지에 대한 문자 메시지 변수를** 삭제합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image28.png">

3.  추가**,** 적응형 카드를 **선택합니다.**

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image29.png">

4.  JSON 편집에서 **수식**으로 **전환** 하여 적응형 카드를 동적으로
    만들고 Power Fx 언어로 작성할 수 있습니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image30.png">

5.  **ServiceNow 티켓 정보에 대한 참조가 이미 포함되어 있는 아래의 Power
    Fx 수식을** 붙여넣습니다

    아래 텍스트를 복사하는 데 어려움이 있으면 Lab 파일의 Misc 폴더로 이동하여 ServiceNow Adaptive Card Power Fx.txt를 엽니다.

    ```
    {
      type: "AdaptiveCard",
      version: "1.5",
      body: [
        {
          type: "ColumnSet",
          columns: [
            {
              type: "Column",
              width: "auto",
              items: [
                {
                  type: "Image",
                  url: "https://www.servicenow.com/community/s/legacyfs/online/avatars_servicenow/1f66cb9fdb3ee3c0107d5583ca961942.jpg",
                  size: "Small",
                  style: "Person"
                }
              ]
            },
            {
              type: "Column",
              width: "stretch",
              items: [
                {
                  type: "TextBlock",
                  text: Topic.SNTicketInfoParsed.short_description,
                  weight: "Bolder",
                  size: "Large",
                  wrap: true,
                  color: "Attention",
                  horizontalAlignment: "Left"
                }
              ],
              verticalContentAlignment: "Center",
              horizontalAlignment: "Center"
            }
          ]
        },
        {
          type: "TextBlock",
          text: Topic.SNTicketInfoParsed.description,
          weight: "Lighter",
          wrap: true
        },
        {
          type: "FactSet",
          facts: [
            {
              title: "Number:",
              value: Topic.SNTicketInfoParsed.number
            },
            {
              title: "State:",
              value: Topic.SNTicketInfoParsed.state
            },
            {
              title: "Priority:",
              value: Topic.SNTicketInfoParsed.priority
            },
            {
              title: "Impact:",
              value: Topic.SNTicketInfoParsed.impact
            },
            {
              title: "Urgency:",
              value: Topic.SNTicketInfoParsed.urgency
            },
            {
              title: "Category:",
              value: Topic.SNTicketInfoParsed.category
            },
            {
              title: "Subcategory:",
              value: Topic.SNTicketInfoParsed.subcategory
            },
            {
              title: "Caller ID:",
              value: Topic.SNTicketInfoParsed.caller_id
            },
            {
              title: "Opened By:",
              value: Topic.SNTicketInfoParsed.opened_by
            },
            {
              title: "Opened At:",
              value: Topic.SNTicketInfoParsed.opened_at
            }
          ],
          spacing: "Small"
        },
        {
          type: "TextBlock",
          text: "Comments and notes:",
          weight: "Bolder",
          size: "Medium",
          wrap: true
        },
        {
          type: "TextBlock",
          text: Topic.SNTicketInfoParsed.comments_and_work_notes,
          wrap: true,
          size: "Small"
        }
      ],
      actions: [
        {
          type: "Action.OpenUrl",
          title: "Update Ticket",
          url: "https://dev204932.service-now.com/nav_to.do?uri=incident.do?sys_id=" & Topic.SNTicketInfoParsed.sys_id & "%26sysparm_view=ess"
        }
      ],
      '$schema': "http://adaptivecards.io/schemas/adaptive-card.json"
    }
    
    ```

6.  **저장을** 클릭합니다.


7.  부조종사를 테스트하십시오.

    ```
    What's the latest on ticket INC0007001, please?
    ```
    ```
    티켓 INC0007001에 대한 최신 정보는 무엇입니까?    
    ```
      
    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2003/media/image31.png">

# 요약

 랩 03 \'부조종사에서 Power Automate 클라우드 흐름 빌드 및 호출\'을
 완료해 주셔서 감사합니다. 다음을 성공적으로 수행했습니다.

-   새 Power Automate 클라우드 흐름을 만들었습니다.
-   Power Automate 클라우드 흐름을 토픽에 호출했습니다.
-   입력 및 출력 변수 설정
-   Copilot Studio에서 사용자에게 동적 데이터를 다시 표시했습니다.
