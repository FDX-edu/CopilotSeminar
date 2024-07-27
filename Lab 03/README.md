# Lab 3. Copilot에서 Power Automate 클라우드 흐름 빌드 및 호출

## 이 랩의 목표 


 이 실습을 마치면 다음을 수행할 수 있습니다.     
 -   Power Automate의 기본 사항 이해 
 -   Copilot Studio를 사용하여 기본 사용 
     사례(ServiceNow 커넥터 사용)에서 Power 
     Automate를 사용하여 다른 데이터 원본에서 
     데이터를 요청하고 고객 또는 사용자와의 대화 
     상자에서 데이터를 반환합니다  

## 필수 구성 요소

> 일부 실습, 특히 이후 실습에서는 기능 및 이전 작업과 관련하여 이전
> 실습을 참조합니다. 랩은 Microsoft Copilot Studio 평가판에 액세스할 수
> 있도록 설계되었습니다. 이전 모듈을 완료하지 않고도 대부분의 랩에서
> 시작하여 계속 진행할 수 있습니다. 그러나 제품 내에서 사용할 수 있는
> 기능을 보여주는 최상의 환경을 위해서는 일부 실습을 시작하기 전에 특정
> 모듈을 완료하는 것이 좋습니다.
>
> 랩 03 -- 챗봇에 대한 Power Automate 흐름 빌드의 경우 다음이
> 필요합니다.
> - 인터넷에 액세스할 수 있는 컴퓨터. 
> - 제공된 Microsoft 테넌트에 로그인할 수 있어야 합니다(일부 회사에서는
    사용자가 회사 테넌트에만 연결하도록 강제함).

## 기본 지식: Power Automate 이해

> Power Automate는 LOB(기간 업무) 사용자가 애플리케이션 및 서비스 전반에
> 걸쳐 시간이 많이 걸리는 비즈니스 작업 및 프로세스를 자동화하는
> 워크플로를 실용적이고 간단하게 구축할 수 있도록 하는 클라우드 기반
> 서비스입니다.
>
> Power Automate는 Power Apps, Microsoft Dataverse, Dynamics 365 및
> Office 365를 포함하는 강력하고 적응 가능한 비즈니스 애플리케이션
> 플랫폼의 일부입니다. 이 플랫폼을 통해 고객, 파트너 및 ISV 파트너는
> 자신의 회사, 산업, 기능적 역할 또는 특정 지역을 위해 특별히 구축된
> 솔루션을 만들 수 있습니다. 비즈니스 요구 사항을 가장 잘 이해하는
> LOB(기간 업무) 사용자는 이제 데이터 및 프로세스를 쉽게 분석, 구성 및
> 간소화할 수 있습니다. 전문 개발자는 자동화, 분석 및 앱 LOB(기간
> 업무)를 쉽게 확장하여 Functions, App Service 및 Logic Apps와 같은
> Azure 서비스를 활용할 수 있습니다. API 커넥터, 게이트웨이 및 Microsoft
> Dataverse를 사용하면 클라우드 또는 온프레미스에서 이미 사용 중인
> 서비스 또는 데이터에서 더 많은 가치를 얻을 수 있습니다.

다음은 Power Automate로 수행할 수 있는 작업의 몇 가지 예입니다.

-   비즈니스 프로세스를 자동화합니다.
-   기한이 지난 작업에 대한 자동 알림을 보냅니다.
-   일정에 따라 시스템 간에 비즈니스 데이터를 이동합니다.
-   1,000개 이상의 데이터 소스 또는 공개적으로 사용 가능한 API에    연결합니다.
-   Excel에서 데이터를 계산하는 것과 같은 로컬 컴퓨터의 작업을 자동화할    수도 있습니다.

데스크탑에서 마우스 클릭, 키 입력 및 복사 붙여넣기 단계를 기록하는
것만으로도 반복적인 수동 작업을 자동화하면 절약되는 시간을 생각해
보십시오! Power Automate는 자동화에 관한 모든 것입니다.

Microsoft Copilot Studio는 Power Automate와 쉽게 연결되어 사용자의
응답에서 변수를 전달하고, 여러 데이터 원본에서 데이터를 검색하고, 해당
데이터에 대해 복잡한 작업을 수행하고, Microsoft Copilot Studio로
돌아가서 해당 데이터를 사용자와 공유할 수 있습니다. API를 통해 액세스할
수 있는 거의 모든 데이터 소스에서 데이터를 작업하고 검색할 수 있다는
것은 Copilot Studio의 가장 중요한 이점 중 하나입니다.

또는 Microsoft Copilot Studio는 토픽 또는 플러그 인 작업에서 직접 Power
Automate와 동일한 커넥터, HTTP 요청 또는 사용자 지정 커넥터를 직접
사용할 수도 있습니다.

이 Microsoft Copilot Studio 랩의 일부로, Power Automate에 대한 광범위한
소개는 포함되지 않지만 외부 데이터 원본에서 데이터를 검색하고 Copilot
Studio의 대화 환경에서 사용하는 방법에 대한 기본 시나리오를 다룹니다.
Power Automate에 대해 자세히 알아보려면 [Power Automate의 Microsoft
Docs](https://learn.microsoft.com/en-us/power-automate/)를 검토하고
Power Automate가 포함된 Microsoft Power Apps의 일별 자료를 검토할 수도
있습니다.
