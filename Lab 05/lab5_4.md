# SharePoint

## Task 1: Configuring a SharePoint knowledge source 작업 1: SharePoint 지식 소스 구성

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

## Task 2: Test the SharePoint knowledge source 작업 2: SharePoint 지식 소스 테스트

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


