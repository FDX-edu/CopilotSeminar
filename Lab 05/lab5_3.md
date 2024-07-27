# Dataverse 

## Task 1: Dataverse 지식 소스 구성

Dataverse 지식 소스를 사용하면 Dataverse 테이블에 저장된 구조화된
데이터에 대해 자연어 쿼리를 할 수 있습니다.

1.  코파일럿의 지식 탭으로 이동하여 지식 추가를 선택합니다.

2.  Dataverse를 선택하고 \'Account\' 테이블을 검색하여 선택한 후 다음을 클릭합니다.

3.  테이블에 데이터가 포함되어 있는지 확인하고 다음을 클릭합니다.

4.  특정 테이블 속성에 대한 질문을 이해하기 위해 동의어에서 편집을 선택합니다. 예를 들어, \'Address 1\'에 대해 동의어로 \'Address\'를 추가하고 설명에 \'Complete address of the account\'를 입력합니다. 그런 다음 뒤로를 선택합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2005/media/image12.png">

5.  계정에 대한 사용자 질문 이해를 개선하기 위해 용어집에서 편집을 선택합니다. 예를 들어, \'Customer\'를 용어로 추가하고 설명에 \'Customer is a synonym for account\'를 입력합니다. 그런 다음 다음을 선택한 후 뒤로를 선택합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2005/media/image13.png">

6.  기본값인 \'Knowledge name\'과 \'Knowledge description\'을 유지합니다.

7.  추가를 클릭합니다.

1.  Dataverse는 내부 데이터 소스이므로 최종 사용자는 로그인해야 합니다. 설정으로 이동하여 보안 인증을 선택한 후 \'Microsoft로 인증\'을 선택하고 저장합니다.

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image4.svg" width="30">**Pro tip:** 이 데이터 소스는 모든 검색이 연결된 최종 사용자의 컨텍스트에서 수행되기 때문에 인증이 필요합니다. 따라서 최종 사용자가 최소한 읽기 액세스 권한이 있는 레코드만 반환되고 요약됩니다.

## Task 2: Dataverse 지식 소스 테스트

5.  테스트 창을 엽니다.

6.  아래 두 질문을 연속으로 합니다.

    ```
    What customers are located in Redmond? List them in a table with their name and address.
    ```

    ```
    레드먼드에 있는 고객은 누구인가요? 이름과 주소와 함께 표에 나열하세요.
    ```


    ```
    Thanks. Who's the primary contact at city power and light?
    ```
    ```
    고맙습니다. City Power and Light의 주요 연락처는 누구입니까?
    ```

    <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2005/media/image14.png" width="400">


