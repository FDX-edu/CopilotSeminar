## Generative AI orchestration 생성형 AI 오케스트레이션

기본적으로 코파일럿은 사용자의 쿼리와 가장 잘 일치하는 트리거 문구를
가진 주제를 트리거하고 대화 컨텍스트에서 주제 입력을 채워 응답합니다.
생성형 AI를 사용하여 코파일럿이 생성한 질문으로 값을 요청함으로써 대화
컨텍스트뿐만 아니라 주제 입력을 채울 수도 있습니다. 이 동작 및 이를
관리하는 방법에 대해 더 알아보려면 \'주제 입력 및 출력 관리\'를
참조하십시오.

생성형 AI를 사용하여 코파일럿이 응답하는 방식을 결정하면 사용자에게 더
자연스럽고 유동적인 대화를 제공할 수 있습니다. 사용자가 메시지를 보내면
코파일럿은 응답을 준비하기 위해 하나 이상의 작업 또는 주제를 선택합니다.
선택은 여러 요소에 따라 결정됩니다. 가장 중요한 요소는 주제 및 작업의
설명입니다. 다른 요소로는 주제나 작업의 이름, 입력 또는 출력 매개변수,
이름 및 설명 등이 있습니다. 설명은 코파일럿이 사용자의 의도를 작업 및
주제와 더 정확하게 연관시킬 수 있게 합니다.

생성 모드에서 코파일럿은 다중 의도 쿼리를 처리하기 위해 여러 작업 또는
주제를 동시에 선택할 수 있습니다. 작업 및 주제가 선택되면 코파일럿은
실행 순서를 결정하는 계획을 생성합니다.

Copilot Studio에서 생성 모드를 사용하는 코파일럿을 테스트할 때 대화 맵을
열어 계획 실행을 따라갈 수 있습니다.

### Task 1: Enable generative AI orchestration 작업 1: 생성형 AI 오케스트레이션 활성화

1.  Go to **Settings** and to the **Generative AI** options

> 설정으로 이동하여 생성 AI 옵션을 선택합니다.

2.  In **How should your copilot decide how to respond?** select
    **Generative**, then **Save**

> **\"Copilot이 응답하는 방식을 어떻게 결정해야 합니까?\"에서
> \"Generative\"를 선택한 다음 저장합니다.**
>
> ![A screenshot of a computer Description automatically
> generated](./output/lab6.docx/media/image2.png){width="5.534039807524059in"
> height="2.747841207349081in"}[]{#_Toc171001494 .anchor}

## Actions 작업

생성 모드를 활성화하면 코파일럿은 런타임에 사용자의 요청에 가장 적합한
작업 또는 주제를 자동으로 선택할 수 있습니다. 고전 모드에서는 코파일럿이
주제를 사용하여 사용자에게 응답할 수 있습니다. 그러나 주제 내에서 작업을
명시적으로 호출하도록 코파일럿을 설계할 수 있습니다.

작업은 다음 기본 작업 유형 중 하나를 기반으로 합니다:

-   사전 빌드된 커넥터 작업

-   맞춤형 커넥터 작업

-   Power Automate 클라우드 흐름

-   AI Builder 프롬프트

-   Bot Framework 스킬

각 기본 작업은 작업을 수행하기 위해 필요한 입력을 채우기 위해 질문을
생성하도록 생성형 AI를 사용할 수 있게 하는 추가 정보를 가지고 있습니다.
따라서 흐름에서 필요한 입력과 같은 모든 입력을 수집하기 위해 질문 노드를
수동으로 작성할 필요가 없습니다. 입력은 런타임 동안 처리됩니다.

작업은 작업의 결과를 사용하여 사용자의 쿼리에 대한 컨텍스트 응답을
생성할 수 있습니다. 또는 작업에 대한 응답을 명시적으로 작성할 수
있습니다.

### Task 1: Create an action 작업 1: 작업 생성

1.  From the **navigation**, go to the **Actions** tab

> 탐색에서 작업 탭으로 이동합니다.

2.  Select **Add an action**.

> 작업 추가를 선택합니다.

3.  Select the **Get forecast for today** connector.

> 오늘의 예보를 가져오는 커넥터를 선택합니다.
>
> ![A screenshot of a computer Description automatically
> generated](./output/lab6.docx/media/image3.png){width="7.219609580052493in"
> height="3.5614337270341205in"}

4.  Wait for the **connection to get automatically created**.

> 연결이 자동으로 생성될 때까지 기다립니다.

5.  **Scroll down**, in **End user authentication**, choose **Copilot
    author authentication**. That way, the copilot can work without
    using the end-user connection when using the weather connector.
    Instead, the connection the maker has setup will be used. Leave
    other properties from that screen as is.

> 스크롤하여 최종 사용자 인증에서 Copilot 작성자 인증을 선택합니다.
> 이렇게 하면 날씨 커넥터를 사용할 때 최종 사용자 연결을 사용하지 않고
> 코파일럿이 작동할 수 있습니다. 대신 작성자가 설정한 연결이 사용됩니다.
> 다른 속성은 그대로 둡니다.
>
> ![A screenshot of a computer Description automatically
> generated](./output/lab6.docx/media/image4.png){width="5.877786526684164in"
> height="2.3088998250218724in"}

6.  Select **Next**.

> 다음을 선택합니다.

7.  Select **Edit inputs**.

> 입력 편집을 선택합니다.

8.  Leave the **Location** one as is, but for **Units**, choose **Set as
    a value**, in **How will the copilot fill this input?**

> 위치 입력은 그대로 두고, 단위 입력에 대해 \"Copilot이 이 입력을 어떻게
> 채울까요?\"에서 값을 설정하도록 선택합니다.

9.  Choose the **I** value (Imperial)

> I 값을 선택합니다

10. **Save**, and then select **Next**.

> 저장을 선택한 다음 다음을 선택합니다.

11. Review the configuration and select **Finish**.

> 구성을 검토하고 마침을 선택합니다.

### Task 2: Test your action 작업 2: 작업 테스트

1.  Go to the **Test** pane.

> 테스트 창으로 이동합니다.

2.  Ask a **question**

> 질문을 합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | What is the weather?                                 |    |
|    | Op |                                                      |    |
|    | en | 날씨는 어떻습니까?                                   |    |
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
|    | b6 |                                                      |    |
|    | .d |                                                      |    |
|    | oc |                                                      |    |
|    | x/ |                                                      |    |
|    | me |                                                      |    |
|    | di |                                                      |    |
|    | a/ |                                                      |    |
|    | im |                                                      |    |
|    | ag |                                                      |    |
|    | e6 |                                                      |    |
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

3.  In the **Test** pane, click on the **Conversation map** to see how
    the copilot interprets questions and prompts for answers.

> 테스트 창에서 대화 맵을 클릭하여 코파일럿이 질문을 해석하고 응답을
> 준비하는 방법을 확인합니다.
>
> ![A screenshot of a computer Description automatically
> generated](./output/lab6.docx/media/image7.png){width="7.514583333333333in"
> height="3.7069444444444444in"}

4.  Answer with a city

5.  도시 이름으로 응답합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Chicago                                              |    |
|    | Op |                                                      |    |
|    | en | 시카고                                               |    |
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
|    | b6 |                                                      |    |
|    | .d |                                                      |    |
|    | oc |                                                      |    |
|    | x/ |                                                      |    |
|    | me |                                                      |    |
|    | di |                                                      |    |
|    | a/ |                                                      |    |
|    | im |                                                      |    |
|    | ag |                                                      |    |
|    | e6 |                                                      |    |
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

6.  See the copilot **automatically updates the inputs** with the city
    and provides an answer.

코파일럿이 자동으로 입력을 해당 도시로 업데이트하고 응답을 제공하는 것을
확인합니다.

7.  Tell the bot you made a mistake and **change your query**.

봇에게 실수를 알리고 쿼리를 변경합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Wait, I meant the weather for London. Also please    |    |
|    | Op | list every information you have in bullet points,    |    |
|    | en | please.                                              |    |
|    | q  |                                                      |    |
|    | uo | 잠깐만요, 제가 말하려던 도시는 런던입니다. 또한 모든 |    |
|    | ta | 정보를 목록으로 나열해 주세요.                       |    |
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
|    | b6 |                                                      |    |
|    | .d |                                                      |    |
|    | oc |                                                      |    |
|    | x/ |                                                      |    |
|    | me |                                                      |    |
|    | di |                                                      |    |
|    | a/ |                                                      |    |
|    | im |                                                      |    |
|    | ag |                                                      |    |
|    | e6 |                                                      |    |
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

> ![A screenshot of a computer Description automatically
> generated](./output/lab6.docx/media/image8.png){width="6.9445220909886265in"
> height="3.4257327209098865in"}

8.  See how the copilot **updates its query** to the connector, and see
    how it also **reacts to the instruction** to list all information
    available to it.

> 코파일럿이 커넥터에 대한 쿼리를 업데이트하고, 모든 이용 가능한 정보를
> 목록으로 나열하는 지시 사항에 따라 응답하는 것을 확인합니다.

## Summary 요약

실습 6 \'연결기와 상호작용하기 위한 생성형 AI 오케스트레이션 사용\'을
완료해 주셔서 감사합니다. 여러분은 다음 작업을 성공적으로 완료했습니다.

-   Copilot Studio에서 작업 생성

-   Copilot Studio에서 사용자에게 동적 데이터 표시

-   대화 컨텍스트를 활용하여 후속 질문
