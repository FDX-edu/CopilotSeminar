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
