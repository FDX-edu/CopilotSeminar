# Knowledge sources 지식 소스

Microsoft Copilot Studio에서의 지식은 Power Platform, Dynamics 365
데이터 및 외부 시스템의 엔터프라이즈 데이터를 추가하여 코파일럿이 최종
사용자에게 관련 정보와 통찰력을 제공할 수 있게 합니다. 또한 생성적
응답에 지식을 통합할 수 있습니다. 지식을 포함하는 게시된 코파일럿은
구성된 지식 소스를 사용하여 게시된 코파일럿을 보강합니다.

**지원되는 지식 소스**

  |  이름  | 소스 |  설명 |    일반 응답에서  |  인증  |
                                                    지원되는 입력 수 
  -------------- -------- ------------------------- ---------------- -------------
  공개 웹사이트  외부     Bing에서 쿼리 입력을      4개의 공개 URL   없음
                          검색하며 제공된           (예:             
                          웹사이트의 결과만         microsoft.com)   
                          반환합니다.                                

  문서           내부     Dataverse에 업로드된      Dataverse 파일   없음
                          문서를 검색하여 문서      저장 할당량에    
                          내용에서 결과를           의해 제한        
                          반환합니다.                                

  SharePoint     내부     SharePoint URL에 연결하여 4개의 URL        코파일럿
                          GraphSearch를 사용하여                     사용자의
                          결과를 반환합니다.                         Microsoft
                                                                     Entra ID 인증

  OneDrive for   내부     OneDrive URL에 연결하여   4개의 URL        코파일럿
  Business                GraphSearch를 사용하여                     사용자의
                          결과를 반환합니다.                         Microsoft
                                                                     Entra ID 인증

  Dataverse      내부     연결된 Dataverse 환경에   두 개의          코파일럿
                          연결하여 Dataverse에서    Dataverse 지식   사용자의
                          생성적 기술을 사용하여    소스 (지식       Microsoft
                          결과를 반환합니다.        소스당 최대      Entra ID 인증
                                                    15개의 테이블)   

  엔터프라이즈   내부     연결된 Dataverse 환경에   맞춤형           코파일럿
  데이터 via              연결하여 Dataverse에서    코파일럿당 두 개 사용자의
  그래프 연결             생성적 기술을 사용하여                     Microsoft
                          결과를 반환합니다.                         Entra ID 인증
  --------------------------------------------------------------------------------

## Websites 웹사이트

### Task 1: Configure website knowledge sources 작업 1: 웹사이트 지식 소스 구성

1.  Navigate to the **Knowledge** tab of your copilot

코파일럿의 지식 탭으로 이동합니다.

![A screenshot of a computer Description automatically
generated](./output/lab5.docx/media/image3.png){width="6.745556649168854in"
height="1.790336832895888in"}

From previous labs, you may see existing knowledge sources, such as
public websites.

-   <https://learn.microsoft.com/en-us/microsoft-copilot-studio/>

-   <https://www.microsoft.com/en-us/microsoft-copilot/>

이전 실습에서 공개 웹사이트와 같은 기존 지식 소스를 볼 수 있습니다.

-   예: <https://learn.microsoft.com/en-us/microsoft-copilot-studio/>

-   예: <https://www.microsoft.com/en-us/microsoft-copilot/>

2.  Select **Add knowledge**.

지식 추가를 선택합니다.

3.  Consider adding a new **website**, such as
    <https://adoption.microsoft.com/en-us/>.\
    Make sure **each** knowledge source has a good **name** and explicit
    **description** of what it can return.

새로운 웹사이트(예: https://adoption.microsoft.com/en-us/)를 추가합니다.
각 지식 소스에는 반환할 수 있는 내용에 대한 명확한 설명을 제공해야
합니다.

![A screenshot of a computer Description automatically
generated](./output/lab5.docx/media/image4.png){width="4.949708005249343in"
height="2.6408891076115486in"}

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   When using the default built-in natural language          |
| out  |     understanding model, knowledge sources are invoked from   |
| line |     the Create generative answers node. By default, user      |
| ](./ |     sentences that don't trigger a topic will go to the       |
| outp |     Conversational boosting topic, where a generative answers |
| ut/l |     node is pre-configured.                                   |
| ab5. |                                                               |
| docx | <!-- -->                                                      |
| /med |                                                               |
| ia/i | -   When generative AI orchestration is enabled, the large    |
| mage |     language model will look at each knowledge source model   |
| 6.sv |     description to know what data source to use to answer a   |
| g){w |     user query.                                               |
| idth |                                                               |
| ="0. | 프로 팁:                                                      |
| 4724 |                                                               |
| 4094 | 기본 내장된 자연어 이해 모델을 사용할 때 지식 소스는 생성적   |
| 4881 | 응답 노드에서 호출됩니다. 기본적으로 주제를 트리거하지 않는   |
| 8897 | 사용자 문장은 대화 증진 주제로 이동하며, 여기서 생성적 응답   |
| 6in" | 노드가 미리 구성됩니다.                                       |
| hei  |                                                               |
| ght= | 생성 AI 오케스트레이션이 활성화되면 대형 언어 모델이 각 지식  |
| "0.4 | 소스 모델 설명을 참고하여 사용자 쿼리에 사용할 데이터 소스를  |
| 7244 | 결정합니다.                                                   |
| 0944 |                                                               |
| 8818 |                                                               |
| 8976 |                                                               |
| in"} |                                                               |
+======+===============================================================+
+------+---------------------------------------------------------------+

### Task 2: Test website knowledge sources 작업 2: 웹사이트 지식 소스 테스트

1.  Launch the **Test** pane

> 테스트 창을 엽니다.

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

3.  Notice that it generates an answer and includes **citations** to
    ground its answer on and offer the user the option to navigate to
    the **sources** that were used to generate this answer.

생성된 응답에는 참조가 포함되어 있으며, 사용자가 이 답변을 생성하는 데
사용된 소스로 이동할 수 있는 옵션을 제공합니다.

> ![A screenshot of a computer program Description automatically
> generated](./output/lab5.docx/media/image9.png){width="3.3760684601924758in"
> height="4.940278871391076in"}

4.  Ask a **follow up** question.

후속 질문을 합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | What knowledge sources does it support?              |    |
|    | Op |                                                      |    |
|    | en | 지원되는 지식 소스는 무엇인가요?                     |    |
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

> ![A screenshot of a chat Description automatically
> generated](./output/lab5.docx/media/image10.png){width="3.37007874015748in"
> height="3.0056955380577426in"}
>
> Notice that even though the follow up question didn't refer to the
> specific product this question applied to, the generative answers
> features made sure context was preserved and that the follow up
> question was interpreted in context of the previous messages in the
> conversation.
>
> 후속 질문이 특정 제품을 언급하지 않았음에도 불구하고, 생성적 응답
> 기능은 대화의 이전 메시지 맥락을 유지하고 후속 질문을 올바르게
> 해석합니다.

