### Dataverse 

#### Task 1: Configuring the Dataverse knowledge source 작업 1: Dataverse 지식 소스 구성

The Dataverse knowledge source allows users to make natural language
queries over structured data, stored in Dataverse tables.

Dataverse 지식 소스를 사용하면 Dataverse 테이블에 저장된 구조화된
데이터에 대해 자연어 쿼리를 할 수 있습니다.

1.  Navigate to the **Knowledge** tab of your copilot and select **Add
    knowledge**.

코파일럿의 지식 탭으로 이동하여 지식 추가를 선택합니다.

2.  Select **Dataverse**, and search Account and select the **Account**
    table and click **Next**

Dataverse를 선택하고 \'Account\' 테이블을 검색하여 선택한 후 다음을
클릭합니다.

3.  Check the table contains data, and click **Next**.

테이블에 데이터가 포함되어 있는지 확인하고 다음을 클릭합니다.

4.  To improve the understanding of questions about specific attributes
    of the table, in **Synonyms**, select **Edit**.\
    In this example, for **Address 1**, add Address as a **Synonym**,
    with Complete address of the account as the **Description**. Then
    select **Back**.

특정 테이블 속성에 대한 질문을 이해하기 위해 동의어에서 편집을
선택합니다. 예를 들어, \'Address 1\'에 대해 동의어로 \'Address\'를
추가하고 설명에 \'Complete address of the account\'를 입력합니다. 그런
다음 뒤로를 선택합니다.

> ![](./output/lab5.docx/media/image12.png){width="6.522742782152231in"
> height="4.245418853893264in"}

5.  To improve the understanding of user questions about accounts, in
    **Glossary**, select **Edit**.\
    In this example, add Customer as a **Term**, with Customer is a
    synonym for account as the **Description**. Then select **Next**,
    then **Back**.

계정에 대한 사용자 질문 이해를 개선하기 위해 용어집에서 편집을
선택합니다. 예를 들어, \'Customer\'를 용어로 추가하고 설명에 \'Customer
is a synonym for account\'를 입력합니다. 그런 다음 다음을 선택한 후
뒤로를 선택합니다.

> ![](./output/lab5.docx/media/image13.png){width="6.45645997375328in"
> height="2.2170188101487316in"}

6.  Keep the default values **Knowledge** **name** and **Knowledge**
    **description**.

기본값인 \'Knowledge name\'과 \'Knowledge description\'을 유지합니다.

7.  Click **Add**.

추가를 클릭합니다.

1.  Because **Dataverse** is an internal data source, end-users have to
    be logged in. So go to **Settings**, **Security**,
    **Authentication**, choose **Authenticate with Microsoft**, then
    **Save**.

Dataverse는 내부 데이터 소스이므로 최종 사용자는 로그인해야 합니다.
설정으로 이동하여 보안 인증을 선택한 후 \'Microsoft로 인증\'을 선택하고
저장합니다.

+------+---------------------------------------------------------------+
| ![Li | **Pro tip:** This data source requires authentication because |
| ghts | any search is done in the context of the connected end-user.  |
| On   | So, only records the end-user has at least read access to are |
| out  | returned and summarized.                                      |
| line |                                                               |
| ](./ | 프로 팁:                                                      |
| outp |                                                               |
| ut/l | 이 데이터 소스는 연결된 최종 사용자의 맥락에서 검색이         |
| ab5. | 수행되므로 인증이 필요합니다. 따라서 최종 사용자가 읽기       |
| docx | 권한을 가진 레코드만 반환되고 요약됩니다.                     |
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

#### Task 2: Test the Dataverse knowledge source 작업 2: Dataverse 지식 소스 테스트

5.  Launch the **Test** pane

테스트 창을 엽니다.

6.  **Ask** these 2 below questions, one after the other.

아래 두 질문을 연속으로 합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | What customers are located in Redmond? List them in  |    |
|    | Op | a table with their name and address.                 |    |
|    | en |                                                      |    |
|    | q  | 레드먼드(Redmond)에 위치한 고객은 누구인가요? 이름과 |    |
|    | uo | 주소를 표로 나열해 주세요.                           |    |
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

+----+----+------------------------------------------------------+----+
|    | ![ | Thanks. Who\'s the primary contact at city power and |    |
|    | Op | light?                                               |    |
|    | en |                                                      |    |
|    | q  | 감사합니다. City Power and Light의 주요 연락처는     |    |
|    | uo | 누구인가요?                                          |    |
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

> ![](./output/lab5.docx/media/image14.png){width="2.8642596237970253in"
> height="6.527128171478565in"}

### SharePoint

#### Task 1: Configuring a SharePoint knowledge source 작업 1: SharePoint 지식 소스 구성

2.  Navigate to the **Knowledge** tab of your copilot and select **Add
    knowledge**.

코파일럿의 지식 탭으로 이동하여 지식 추가를 선택합니다.

3.  Select **SharePoint and OneDrive**, and use this URL:
    copilotstudiotraining.sharepoint.com/.\
    Give it a description "Answer

SharePoint 및 OneDrive를 선택하고 다음 URL을 사용합니다: 설명에
\'Answer\'를 입력합니다.

4.  Because **SharePoint and OneDrive** is an internal data source,
    end-users have to be authenticated. If it's not the case, go to
    **Settings**, **Security**, **Authentication**, choose
    **Authenticate with Microsoft**, then **Save**

SharePoint 및 OneDrive는 내부 데이터 소스이므로 최종 사용자는 인증해야
합니다. 인증되지 않은 경우 설정으로 이동하여 보안 인증을 선택한 후
\'Microsoft로 인증\'을 선택하고 저장합니다..

+------+---------------------------------------------------------------+
| ![Li | **Pro tip:** This data source requires authentication because |
| ghts | any search is done in the context of the connected end-user.  |
| On   | So, only documents and pages the end-user has at least read   |
| out  | access to are returned and summarized.                        |
| line |                                                               |
| ](./ | **프로 팁:**                                                  |
| outp |                                                               |
| ut/l | 이 데이터 소스는 연결된 최종 사용자의 맥락에서 검색이         |
| ab5. | 수행되므로 인증이 필요합니다. 따라서 최종 사용자가 읽기       |
| docx | 권한을 가진 문서와 페이지만 반환되고 요약됩니다.              |
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

#### Task 2: Test the SharePoint knowledge source 작업 2: SharePoint 지식 소스 테스트

1.  Launch the **Test** pane

테스트 창을 엽니다.

2.  Ask a question that doesn't match an existing topic to trigger the
    **Conversational boosting** topic.

기존 주제와 일치하지 않는 질문을 하여 대화 증진 주제를 트리거합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | What is the Northwind Standard plan?                 |    |
|    | Op |                                                      |    |
|    | en | 북풍 표준 계획이 무엇인가요?                         |    |
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

Notice that it generates an answer and includes **citations** to ground
its answer on and offer the user the option to navigate to the
**sources** that were used to generate this answer

생성된 응답에는 참조가 포함되어 있으며, 사용자가 이 답변을 생성하는 데
사용된 소스로 이동할 수 있는 옵션을 제공합니다.

> ![A screenshot of a phone Description automatically
> generated](./output/lab5.docx/media/image15.png){width="2.8440780839895012in"
> height="3.121362642169729in"}

## Custom instructions  맞춤형 지시 사항

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

### 작업 1: 생성 AI 오케스트레이션을 위한 맞춤형 지시 사항 구성

 

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

### Task 2: Configure custom instructions for classic orchestration

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

### Task 3: Test custom instructions 작업 3: 맞춤형 지시 사항 테스트

 

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

 

## AI general knowledge AI 일반 지식

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
