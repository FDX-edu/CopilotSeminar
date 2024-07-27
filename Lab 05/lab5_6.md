# AI general knowledge AI 일반 지식

지식 소스 외에도 AI 일반 지식을 사용하여 고객의 질문에 대한 정보를 찾아
제공할 수 있습니다. 일반 지식을 사용하면 고객의 모든 질문을 다루지 못할
수 있는 여러 주제를 수동으로 작성할 필요가 없습니다. 이 기능을 통해
코파일럿이 지식 소스의 데이터를 기반으로 하지 않고도 자체 지식을
사용하여 질문에 답변할 수 있습니다. 이는 ChatGPT에게 질문하는 것과
유사합니다.

### Task 1: Configure the use of AI general knowledge 작업 1: AI 일반 지식 사용 구성

1.  From the navigation, go to the **Overview** tab.

탐색에서 개요 탭으로 이동합니다.

2.  In the **Knowledge** area, enable **Allow the AI to use its own
    general knowledge**.

지식 영역에서 \"AI가 자체 일반 지식을 사용하도록 허용\"을 활성화합니다.

### Task 2: Test the use of AI general knowledge 작업 2: AI 일반 지식 사용 테스트

1.  Launch the **Test** pane

테스트 창을 엽니다.

2.  Ask a question that neither matches an existing or a configured
    knowledge source.

> 기존 주제나 구성된 지식 소스와 일치하지 않는 질문을 합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Can you list the planets from closest to farthest    |    |
|    | Op | from the sun?                                        |    |
|    | en |                                                      |    |
|    | q  | 태양에서 가장 가까운 행성부터 먼 순서대로 나열할 수  |    |
|    | uo | 있나요?                                              |    |
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

> ![A screenshot of a cellphone Description automatically
> generated](./output/lab5.docx/media/image19.png){width="2.519695975503062in"
> height="3.0106397637795275in"}

## The conversational boosting topic and the generative answer node

대화 증진 주제와 생성적 응답 노드

기본 내장된 자연어 이해 모델을 사용하면 주제를 트리거하지 않는 모든
사용자 발화가 대화 증진 주제로 이동하며, 답변이 식별되지 않으면 폴백으로
이동합니다. 다른 주제와 마찬가지로 대화 증진 주제의 논리를 시나리오에
맞게 구성할 수 있습니다.

### Task 1: Access the Conversational boosting topic 작업 1: 대화 증진 주제 접근

11. From the navigation, go to the **Topics** tab.

탐색에서 주제 탭으로 이동합니다.

12. Select the **System** topics area.

> 시스템 주제 영역을 선택합니다.

13. Select the **Conversational boosting** topic.

대화 증진 주제를 선택합니다.

![A screenshot of a computer Description automatically
generated](./output/lab5.docx/media/image20.png){width="7.329847987751531in"
height="3.6158147419072617in"}

### Task 2: Review the generative answers node 작업 2: 생성적 응답 노드 검토

1.  In the **Conversational boosting** topic, go to the **Create
    generative answers** node **properties**

대화 증진 주제에서 생성적 응답 노드 속성으로 이동합니다.

2.  With the **Search only selected sources**, see that you hand-pick
    the **knowledge sources** that should be used when entering that
    specific node.

선택한 소스만 검색하도록 설정하면 특정 노드에 들어갈 때 사용해야 하는
지식 소스를 직접 선택할 수 있습니다.

3.  For example, select **all** but the SharePoint knowledge sources (at
    it's currently the slowest one).

> 예를 들어, 현재 가장 느린 SharePoint 지식 소스를 제외한 모든 소스를
> 선택합니다.
>
> ![A screenshot of a computer Description automatically
> generated](./output/lab5.docx/media/image21.png){width="2.7783344269466315in"
> height="3.902463910761155in"}

4.  You can also choose to **disable** **AI to use its own general
    knowledge**, and you can also set **additional custom
    instructions**. The **Content moderation** setting is the level of
    controls you apply to avoid the copilot from hallucinating (i.e.,
    coming up with a wrong answer to a question, for example by
    misinterpreting or overinterpreting grounding data).

AI가 자체 일반 지식을 사용하지 않도록 설정할 수도 있으며, 추가 맞춤형
지시 사항을 설정할 수도 있습니다. 콘텐츠 중재 설정은 코파일럿이 잘못된
답변을 생성하는 것을 방지하기 위해 적용할 제어 수준입니다(예: 데이터를
잘못 해석하거나 과도하게 해석하여 질문에 대한 잘못된 답변을 생성하는
경우).

> ![A screenshot of a chat box Description automatically
> generated](./output/lab5.docx/media/image22.png){width="2.726288276465442in"
> height="4.391369203849519in"}

5.  **Save**

+------+---------------------------------------------------------------+
| ![Li | **Pro tip:** You may disregard the authentication warning as  |
| ghts | this won't apply to the tests done in this lab                |
| On   |                                                               |
| out  | 프로 팁:이 실습에서 수행한 테스트에는 적용되지 않으므로 인증  |
| line | 경고를 무시할 수 있습니다.                                    |
| ](./ |                                                               |
| outp | ![](./ou                                                      |
| ut/l | tput/lab5.docx/media/image23.png){width="3.056790244969379in" |
| ab5. | height="1.2089555993000876in"}                                |
| docx |                                                               |
| /med |                                                               |
| ia/i |                                                               |
| mage |                                                               |
| 6.sv |                                                               |
| g){w |                                                               |
| idth |                                                               |
| ="0. |                                                               |
| 4724 |                                                               |
| 4094 |                                                               |
| 4881 |                                                               |
| 8897 |                                                               |
| 6in" |                                                               |
| hei  |                                                               |
| ght= |                                                               |
| "0.4 |                                                               |
| 7244 |                                                               |
| 0944 |                                                               |
| 8818 |                                                               |
| 8976 |                                                               |
| in"} |                                                               |
+======+===============================================================+
+------+---------------------------------------------------------------+
