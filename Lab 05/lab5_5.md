# Custom instructions  맞춤형 지시 사항

프롬프트 수정을 통해 생성적 응답 및 지식 소스의 기능을 확장하여 맞춤형
지시 사항을 추가할 수 있습니다. 맞춤형 지시 사항을 사용할 때는 프롬프트
엔지니어링에 대한 모범 사례를 따르는 것이 중요합니다. 다음은 이 기능을
최대한 활용하기 위한 몇 가지 팁입니다:

-   **구체적으로:** 맞춤형 지시 사항은 명확하고 구체적이어야 하며,
    코파일럿이 무엇을 해야 할지 정확히 이해할 수 있어야 합니다.
    모호하거나 애매한 언어는 혼동이나 잘못된 응답을 유발할 수 있습니다.

-   **예제 사용:** 예제를 제공하여 지시 사항을 설명하고 코파일럿이
    기대하는 바를 이해하도록 돕습니다. 예제는 코파일럿이 정확하고 관련성
    있는 응답을 생성하는 데 도움이 됩니다.

-   **간단하게 유지:** 맞춤형 지시 사항에 너무 많은 세부 정보나 복잡한
    논리를 추가하지 마십시오. 지시 사항을 간단하고 명확하게 유지하여
    코파일럿이 효과적으로 처리할 수 있도록 합니다.

-   **대안 제공:** 코파일럿이 할당된 작업을 완료할 수 없을 때를 대비한
    대안을 제공하십시오. 예를 들어, 사용자가 질문할 때 \"답변이 없으면
    \'찾을 수 없음\'으로 응답\"과 같은 대안을 포함할 수 있습니다. 이러한
    대안은 코파일럿이 잘못된 응답을 생성하는 것을 방지하는 데 도움이
    됩니다.

-   **테스트 및 개선:** 맞춤형 지시 사항이 의도한 대로 작동하는지 철저히
    테스트하는 것이 중요합니다. 필요에 따라 조정하여 코파일럿의 응답
    정확성과 효과를 향상시킵니다.

## 작업 1: 생성 AI 오케스트레이션을 위한 맞춤형 지시 사항 구성

 

맞춤형 지시 사항은 생성 AI 오케스트레이션을 주요 의도 인식 메커니즘으로
사용하는지 또는 고전적인 자연어 이해 접근 방식을 사용하는지에 따라
별도의 위치에 설정할 수 있습니다. 생성 AI 오케스트레이션이 활성화된 경우
지시 사항은 코파일럿 수준에서 설정해야 합니다.

1.  Let's first make sure Generative AI orchestration is enabled. From
    the navigation, go to **Settings** tab.

먼저 생성 AI 오케스트레이션이 활성화되어 있는지 확인합니다. 탐색에서
설정 탭으로 이동합니다.

2.  Navigate to the **Generative AI** menu.

생성 AI 메뉴로 이동합니다.

3.  In **How should your copilot decide how to respond?,** select
    **Generative (preview)**.

\"Copilot이 응답하는 방식을 어떻게 결정해야 합니까?\"에서 \"Generative
(미리보기)\"를 선택합니다.

4.  **Save** and **Close** the settings.

설정을 저장하고 닫습니다.

5.  From the navigation, go to the **Overview** tab.

> 탐색에서 개요 탭으로 이동합니다.

6.  In the **Details** area, select **Edit**.

세부 정보 영역에서 편집을 선택합니다.

7.  Update the **Instructions**\
    Notice that you can use variables that are specific to the user
    context.

지시 사항을 업데이트합니다. 사용자 맥락에 특정한 변수를 사용할 수 있음을
주목하십시오.

+----+----+------------------------------------------------------+----+
|    | ![ | Talk like a pirate and use pirate expressions.       |    |
|    | Op |                                                      |    |
|    | en | Use emojis in your responses.                        |    |
|    | q  |                                                      |    |
|    | uo | Answer in less than 50 words.                        |    |
|    | ta |                                                      |    |
|    | ti | Refuse to answer questions that are not about        |    |
|    | on | Microsoft products.                                  |    |
|    | ma |                                                      |    |
|    | rk | 해적처럼 말하고 해적 표현을 사용하십시오.            |    |
|    | ou |                                                      |    |
|    | tl | 응답에 이모지를 사용하십시오.                        |    |
|    | in |                                                      |    |
|    | e] | 50단어 이내로 답변하십시오.                          |    |
|    | (. |                                                      |    |
|    | /o | Microsoft 제품에 관한 질문이 아닌 경우 답변을        |    |
|    | ut | 거부하십시오.                                        |    |
|    | pu |                                                      |    |
|    | t/ |                                                      |    |
|    | la |                                                      |    |
|    | b5 |                                                      |    |
|    | .d |                                                      |    |
|    | oc |                                                      |    |
|    | x/ |                                                      |    |
|    | me |                                                      |    |
|    | di |                                                      |    |
|    | a/ |                                                      |    |
|    | im |                                                      |    |
|    | ag |                                                      |    |
|    | e8 |                                                      |    |
|    | .s |                                                      |    |
|    | vg |                                                      |    |
|    | ){ |                                                      |    |
|    | wi |                                                      |    |
|    | dt |                                                      |    |
|    | h= |                                                      |    |
|    | "0 |                                                      |    |
|    | .4 |                                                      |    |
|    | 69 |                                                      |    |
|    | 73 |                                                      |    |
|    | 64 |                                                      |    |
|    | 39 |                                                      |    |
|    | 19 |                                                      |    |
|    | 51 |                                                      |    |
|    | 00 |                                                      |    |
|    | 6i |                                                      |    |
|    | n" |                                                      |    |
|    | he |                                                      |    |
|    | ig |                                                      |    |
|    | ht |                                                      |    |
|    | =" |                                                      |    |
|    | 0. |                                                      |    |
|    | 38 |                                                      |    |
|    | 02 |                                                      |    |
|    | 24 |                                                      |    |
|    | 19 |                                                      |    |
|    | 07 |                                                      |    |
|    | 26 |                                                      |    |
|    | 15 |                                                      |    |
|    | 92 |                                                      |    |
|    | in |                                                      |    |
|    | "} |                                                      |    |
+====+====+======================================================+====+
+----+----+------------------------------------------------------+----+

8.  **Save**

저장합니다.

![A screenshot of a computer Description automatically
generated](./output/lab5.docx/media/image16.png){width="4.96261154855643in"
height="2.857592957130359in"}

## Task 2: Configure custom instructions for classic orchestration

작업 2: 고전적 오케스트레이션을 위한 맞춤형 지시 사항 구성

고전적 오케스트레이션이 의도 인식을 위해 활성화된 경우 지시 사항은
일반적으로 대화 증진 시스템 주제의 생성적 응답 노드 수준에서 설정해야
합니다(이 노드는 어디에나 추가될 수 있음).

1.  Let's make sure **Classic** orchestration is enabled. From the
    navigation, go to **Settings** tab.

고전적 오케스트레이션이 활성화되어 있는지 확인합니다. 탐색에서 설정
탭으로 이동합니다.

2.  Navigate to the **Generative AI** menu.

생성 AI 메뉴로 이동합니다.

3.  In **How should your copilot decide how to respond?**, select
    **Classic**.

\"Copilot이 응답하는 방식을 어떻게 결정해야 합니까?\"에서 \"Classic\"을
선택합니다.

4.  **Save** and **Close** the settings.

설정을 저장하고 닫습니다.

5.  From the navigation, go to the **Topics** tab.

탐색에서 주제 탭으로 이동합니다.

6.  Select the **System** topics area.

시스템 주제 영역을 선택합니다.

7.  Select the **Conversational boosting** topic.

> 대화 증진 주제를 선택합니다.

8.  Go to the **Create generative answers** node **properties**

생성적 응답 노드 속성으로 이동합니다.

9.  There is text area where the placeholder text says **Customize your
    prompt with variables and plain language**. Add your custom
    instructions here.

지시 사항을 사용자 지정할 수 있는 텍스트 영역이 있습니다. 여기에 맞춤형
지시 사항을 추가합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Talk like a pirate and use pirate expressions.       |    |
|    | Op |                                                      |    |
|    | en | Use emojis in your responses.                        |    |
|    | q  |                                                      |    |
|    | uo | Answer in less than 50 words.                        |    |
|    | ta |                                                      |    |
|    | ti | 해적처럼 말하고 해적 표현을 사용하십시오.            |    |
|    | on |                                                      |    |
|    | ma | 응답에 이모지를 사용하십시오.                        |    |
|    | rk |                                                      |    |
|    | ou | 50단어 이내로 답변하십시오.                          |    |
|    | tl |                                                      |    |
|    | in |                                                      |    |
|    | e] |                                                      |    |
|    | (. |                                                      |    |
|    | /o |                                                      |    |
|    | ut |                                                      |    |
|    | pu |                                                      |    |
|    | t/ |                                                      |    |
|    | la |                                                      |    |
|    | b5 |                                                      |    |
|    | .d |                                                      |    |
|    | oc |                                                      |    |
|    | x/ |                                                      |    |
|    | me |                                                      |    |
|    | di |                                                      |    |
|    | a/ |                                                      |    |
|    | im |                                                      |    |
|    | ag |                                                      |    |
|    | e8 |                                                      |    |
|    | .s |                                                      |    |
|    | vg |                                                      |    |
|    | ){ |                                                      |    |
|    | wi |                                                      |    |
|    | dt |                                                      |    |
|    | h= |                                                      |    |
|    | "0 |                                                      |    |
|    | .4 |                                                      |    |
|    | 69 |                                                      |    |
|    | 73 |                                                      |    |
|    | 64 |                                                      |    |
|    | 39 |                                                      |    |
|    | 19 |                                                      |    |
|    | 51 |                                                      |    |
|    | 00 |                                                      |    |
|    | 6i |                                                      |    |
|    | n" |                                                      |    |
|    | he |                                                      |    |
|    | ig |                                                      |    |
|    | ht |                                                      |    |
|    | =" |                                                      |    |
|    | 0. |                                                      |    |
|    | 38 |                                                      |    |
|    | 02 |                                                      |    |
|    | 24 |                                                      |    |
|    | 19 |                                                      |    |
|    | 07 |                                                      |    |
|    | 26 |                                                      |    |
|    | 15 |                                                      |    |
|    | 92 |                                                      |    |
|    | in |                                                      |    |
|    | "} |                                                      |    |
+====+====+======================================================+====+
+----+----+------------------------------------------------------+----+

![](./output/lab5.docx/media/image17.png){width="3.0912325021872267in"
height="2.0522167541557303in"}

10. **Save**

저장합니다.

## Task 3: Test custom instructions 작업 3: 맞춤형 지시 사항 테스트

 

1.  Launch the **Test** pan

테스트 창을 엽니다.

2.  Ask a question that doesn't match an existing topic to trigger the
    **Conversational boosting** topic.

기존 주제와 일치하지 않는 질문을 하여 대화 증진 주제를 트리거합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | What is Microsoft Copilot Studio?                    |    |
|    | Op |                                                      |    |
|    | en | Microsoft Copilot Studio란 무엇인가요?               |    |
|    | q  |                                                      |    |
|    | uo |                                                      |    |
|    | ta |                                                      |    |
|    | ti |                                                      |    |
|    | on |                                                      |    |
|    | ma |                                                      |    |
|    | rk |                                                      |    |
|    | ou |                                                      |    |
|    | tl |                                                      |    |
|    | in |                                                      |    |
|    | e] |                                                      |    |
|    | (. |                                                      |    |
|    | /o |                                                      |    |
|    | ut |                                                      |    |
|    | pu |                                                      |    |
|    | t/ |                                                      |    |
|    | la |                                                      |    |
|    | b5 |                                                      |    |
|    | .d |                                                      |    |
|    | oc |                                                      |    |
|    | x/ |                                                      |    |
|    | me |                                                      |    |
|    | di |                                                      |    |
|    | a/ |                                                      |    |
|    | im |                                                      |    |
|    | ag |                                                      |    |
|    | e8 |                                                      |    |
|    | .s |                                                      |    |
|    | vg |                                                      |    |
|    | ){ |                                                      |    |
|    | wi |                                                      |    |
|    | dt |                                                      |    |
|    | h= |                                                      |    |
|    | "0 |                                                      |    |
|    | .4 |                                                      |    |
|    | 69 |                                                      |    |
|    | 73 |                                                      |    |
|    | 64 |                                                      |    |
|    | 39 |                                                      |    |
|    | 19 |                                                      |    |
|    | 51 |                                                      |    |
|    | 00 |                                                      |    |
|    | 6i |                                                      |    |
|    | n" |                                                      |    |
|    | he |                                                      |    |
|    | ig |                                                      |    |
|    | ht |                                                      |    |
|    | =" |                                                      |    |
|    | 0. |                                                      |    |
|    | 38 |                                                      |    |
|    | 02 |                                                      |    |
|    | 24 |                                                      |    |
|    | 19 |                                                      |    |
|    | 07 |                                                      |    |
|    | 26 |                                                      |    |
|    | 15 |                                                      |    |
|    | 92 |                                                      |    |
|    | in |                                                      |    |
|    | "} |                                                      |    |
+====+====+======================================================+====+
+----+----+------------------------------------------------------+----+

> ![A screenshot of a phone Description automatically
> generated](./output/lab5.docx/media/image18.png){width="3.6457830271216096in"
> height="4.956964129483815in"}

 


