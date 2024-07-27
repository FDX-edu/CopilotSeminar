# AI Builder prompts AI Builder 프롬프트

프롬프트를 LLM(Large Language Model)에게 주는 작업이나 목표로
생각하십시오. 프롬프트 빌더를 사용하면 맞춤형 프롬프트를 만들고
테스트하며 저장할 수 있습니다. 또한 런타임 시 동적 컨텍스트 데이터를
제공하는 입력 변수를 사용할 수 있습니다. 이러한 프롬프트를 다른 사람들과
공유하고 Power Automate, Power Apps 또는 Copilot Studio에서 사용할 수
있습니다. 예를 들어, 회사 이메일에서 작업 항목을 선택하는 프롬프트를
만들어 이메일 처리 자동화를 구축하는 Power Automate 플로우에서 사용할 수
있습니다.

프롬프트 빌더는 메이커가 자연어를 사용하여 특정 비즈니스 요구에 맞는
맞춤형 프롬프트를 고안할 수 있도록 합니다. 이러한 프롬프트는 콘텐츠
요약, 데이터 분류, 엔티티 추출, 언어 번역, 감정 평가 또는 불만에 대한
응답 작성 등 다양한 작업이나 비즈니스 시나리오에 사용할 수 있습니다

프롬프트를 플로우에 통합하여 지능형 자동화를 구축할 수 있습니다.
메이커는 자연어 프롬프트를 설명하여 애플리케이션의 고급 생성 AI 기능을
구축할 수 있습니다. 이러한 프롬프트를 사용하여 맞춤형 Copilot을
확장함으로써 일상적인 비즈니스 운영을 간소화하고 효율성을 높일 수
있습니다.

맞춤형 프롬프트를 사용하면 메이커는 GPT 모델이 특정 방식으로 작동하거나
특정 작업을 수행하도록 지시할 수 있습니다. 프롬프트를 신중하게
작성함으로써 특정 비즈니스 요구에 맞는 응답을 생성할 수 있습니다. 이를
통해 GPT 모델을 다양한 작업을 수행할 수 있는 유연한 도구로 변환할 수
있습니다.

## Task 1: 생성 AI 오케스트레이션 비활성화

1.  설정으로 이동하여 생성 AI 옵션을 선택하십시오.

2.  \"Copilot이 응답하는 방식을 어떻게 결정해야 합니까?\"에서 클래식을 선택한 후 저장하십시오.

## Task 2: 프롬프트 생성

1.  주제로 이동하여 \"티켓 상태 확인\"을 엽니다.

2. 적응형 카드가 포함된 마지막 메시지 뒤에 (+) 버튼으로 다른 노드를 추가합니다.
작업 호출을 선택하고 프롬프트 생성을 선택합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2007/media/image2.png" >

3.  이름을 정합니다. Ticket customer communication

4.  입력 추가: Ticket Details

5.  프롬프트에서 아래 지침을 복사하여 붙여넣기합니다.

    ```
    Based on the ticket details, write a personalized, apologetic, message to the person impacted.
    You can summarize the issue to show you understand it.
    Show empathy and suggest ways to mitigate the situation based on the ticket details.
    Have a positive attitude, and use emojis when applicable.
    Don't include hashtags.
    The text should be a single paragraph.

    ## Ticket details
    ```

    ```
    티켓 세부 정보를 바탕으로 영향을 받은 사람에게 개인화된 사과 메시지를 작성합니다.
    문제를 요약하여 이해한다는 것을 보여줄 수 있습니다.
    공감을 표시하고 티켓 세부 정보를 바탕으로 상황을 완화할 방법을 제안합니다.
    긍정적인 태도를 갖고 해당되는 경우 이모티콘을 사용합니다.
    해시태그를 포함하지 마십시오.
    텍스트는 단일 문단이어야 합니다.
    
    ## Ticket details
    ```


6.  Ticket details 아래에 삽입 버튼을 사용하여 세부 정보 입력을 선택하십시오.

7.  설정에서 모델 GPT-4 (미리보기)를 선택하십시오.

8.  랩 3에서 ServiceNow 샘플 JSON 페이로드를 입력 샘플 데이터에 붙여넣고 프롬프트 테스트를 선택하여 프롬프트를 테스트하십시오.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2007/media/image5.png" >

9.  맞춤형 프롬프트 저장을 선택하십시오.

10. 세부 정보 입력에 SNTicketInfo 변수를 선택하십시오.

11. 생성된 출력물을 위한 변수를 생성하십시오: PersonalizedMessage

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2007/media/image6.png" >

12. 메시지 노드를 추가하고 PersonalizedMessage.text 변수를 삽입하십시오.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2007/media/image7.png" >

13. **Save**

14. **Test** 

    ```
    What's the latest on ticket INC0007001, please?
    ```
    ```
    티켓 INC0007001에 대한 최신 상태는 무엇인가요?
    ```

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2007/media/image8.png" >

# Summary 요약

랩 07 '생성 AI 오케스트레이션을 사용하여 커넥터와 상호 작용하기'를 완료해 주셔서 감사합니다. 다음 작업을 성공적으로 완료하셨습니다.

- Copilot Studio에서 맞춤형 프롬프트 생성 
- 입력을 전달하고 출력물을 최종 사용자에게 제공하는 답변으로 사용