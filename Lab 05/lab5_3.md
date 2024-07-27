# Dataverse 

## Task 1: Configuring the Dataverse knowledge source 작업 1: Dataverse 지식 소스 구성

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

## Task 2: Test the Dataverse knowledge source 작업 2: Dataverse 지식 소스 테스트

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


