

# 연습 1: 코파일럿 만들기를 위해 로그인하기

> 이 연습에서는 제공된 자격 증명을 사용하여 Microsoft Copilot Studio 작성 환경에 로그인합니다.

## 작업 1: 브라우저 환경 설정

기존에 로그인한 경험과 충돌을 피하기 위해 다음 세 가지 옵션 중 하나를
사용하여 이 실습을 수행할 수 있습니다.

1.  **해당 워크숍에서 사용할 새 작업 프로필 설정**

>**Pro tip:** 작업 환경과 평가판 환경 간에 작업 기록을 
유지하면서 전환하는 가장 좋은 옵션입니다. 나중에 계정을 계속 
사용하려는 경우 이상적입니다. 

2.  Or **게스트로 브라우징**
3.  Or **InPrivate 세션 시작**.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image5.png" width="600">



## 작업 2: Copilot Studio에 로그인하기

1.  aka.ms/CopilotStudioStart로 이동

2. **제공된 사용자 이름을 입력하고 다음을 클릭**

3.  **Sign in 제공된 비밀번호를 입력하고 로그인 클릭**

4.  메시지가 표시되면 로그인 상태를 유지할지 여부를 선택합니다.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image6.png" width="400">

5. Microsoft Copilot Studio에 처음 액세스하면 국가/지역을 선택하라는
메시지가 표시됩니다. 값을 선택하거나 기본 옵션을 그대로 두고 시작하기를
클릭할 수 있습니다.

## 작업 3: 코파일럿 만들기

1.  Microsoft Copilot Studio 홈페이지에서 코파일럿을 설명하여 만듭니다.

```
I want to a copilot for my customer support.
It is an assistant for Contoso customers, helping to answer common questions
and help with common tasks, like checking an order status
```

```
고객 지원을 위한 부조종사를 원합니다.
Contoso 고객을 위한 도우미로, 일반적인 질문에 답변하고 주문 상태 확인과 같은 일반적인 작업을 돕는 데 도움이 됩니다
```

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image9.png" width="800">

2.  부조종사를 추가로 사용자 지정할 수 있는 대화 환경으로 리디렉션됩니다. 설명에 대한 추가 세부 정보를 제공할 수 있으며(거부할 수 있음) 목소리 톤을 입력하라는 메시지도 표시됩니다. 

```
Playful tone, joyful, customer focus, but definitely professional
```
```
장난기 넘치는 어조, 유쾌하고 고객 중심적이지만 확실히 전문적입니다.
```

3.  **공개적으로 접근 가능한** 웹사이트를 정보 소스로 요청받습니다.
```
Information should come from https://learn.microsoft.com/en-us/microsoft-copilot-studio/ and from https://www.microsoft.com/en-us/microsoft-copilot/
```

```
정보는 https://learn.microsoft.com/en-us/microsoft-copilot-studio/ 와 https://www.microsoft.com/en-us/microsoft-copilot/ 에서 가져와야 합니다.
```

4.  코파일럿이 도와주거나 논의하지 않아야 할 주제나 작업도 요청받습니다.

```
We don't want to discuss other brands like Fabrikam. Never provide product comparisons with competitor technologies.
```

```
Fabrikam과 같은 다른 브랜드에 대해 논의하고 싶지는 않습니다. 경쟁사 기술과 제품을 비교하지 마십시오.
```

5.  필요한 정보를 모두 입력하면 \"완료\"를 클릭합니다.

6.  코파일럿을 생성하기 전에 \"\...\" 및 \"고급 설정 편집\" 메뉴로 이동하여
코파일럿 스키마 이름을 업데이트하고(코파일럿 표시 이름과 달리 스키마
이름은 고유해야 하며 나중에 변경할 수 없음), 솔루션(예: \"Copilot Studio
Workshop\")에 저장합니다.

사용자 지정 부조종사의 고유한 이름(표시 이름 및 스키마 이름 모두)을 선택해야 합니다


7. 그런 다음 \"생성\"을 선택할 수 있습니다.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image12.png" width="800">

1.	"Skip to configure(구성으로 건너뛰기)"를 선택하여 대화 생성 환경을 피하도록 선택할 수 있습니다.
2.	"언어 편집" 메뉴에서 부조종사의 기본 언어를 설정할 수 있습니다. 랩의 경우 영어(en-US)를 유지해야 합니다.
3.	항상 자체 솔루션 및 게시자의 컨텍스트에서 copilot를 구성하여 원하는 게시자 접두사로 copilot를 만들고 쉽게 내보내고 다른 환경에 배포할 수 있도록 하는 것이 좋습니다.



