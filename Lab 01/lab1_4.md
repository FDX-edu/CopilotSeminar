# 연습 4: 첫 번째 주제 만들기

## Task 1: Create a new topic manually 작업 1: 새 주제 수동으로 만들기

첫 번째 작업에서는 다음 단계를 따라 새 주제를 수동으로 만듭니다:

1.  Microsoft Copilot Studio의 왼쪽 메뉴에서 Topic을 선택합니다.

2.  화면 상단의 **Add a topic** 드롭다운에서 **From blank**에서 옵션을 선택합니다.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image19.png">

3.  주제 제목을 \"untitled\"에서 \"Check Order Status\"로 클릭하여 이름을
바꿉니다.

4.  주제 트리거 아래에서 구문을 선택하고 편집을 선택합니다.

5.  다음 구문을 붙여넣고 Enter를 누릅니다.

```
order status
track my order
where is my package
check order status
has my order shipped
```

```
주문 상태
내 주문 추적
내 패키지는 어디에 있습니까?
주문 상태 확인
내 주문이 배송되었나요?
```

6.  오른쪽 상단의 세부 사항 버튼을 선택하여 주제 세부 사항 창을 엽니다.

여기에서 구성된 주제 이름(작성자가 보는 것)과 다른 표시 이름(최종
사용자가 볼 수 있는 것)을 설정할 수 있습니다.

**Pro tips :** 표시 이름: 중의성 발생 시 사용됩니다(예: 여러 주제가 사용자 발화와 일치할 때, \"다음 중 어느 것을 의미하셨나요\...\"  질문에서 두세 개의 인식된 주제 중 선택하도록 사용자에게  요청).                              
 생성 AI 오케스트레이션 사용 시: 주제 트리거를 위한 내장 자연어 이해 대신 사용되며, 표시 이름은 모델 표시 이름으로 불리며, 모델 설명과 함께 의도 감지 과정의 일부로 사용됩니다.  세부 사항 창: 주제 입력 및 출력 변수를 구성할 수 있는 곳입니다. 이는 다른 주제에서 주제를 호출할 때나 생성 AI  오케스트레이션이 켜져 있을 때 유용합니다. 이 경우 대형 언어 모델을 사용하여 필요한 변수를 슬롯 채우기하고, 사용자가  누락된 입력을 자동으로 요청합니다.   

7.  저장을 선택합니다.

## Task 2: Review the topic user interface 작업 2: 주제 사용자 인터페이스 검토

이제 첫 번째 주제를 만들었으므로(트리거 구문 외에는 콘텐츠 없음), 작성
사용자 인터페이스(UI)를 탐색하여 친숙해질 수 있습니다. 

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image20.png">

1.  **주제 제목**: 현재 편집 중인 주제의 이름으로, 주제 페이지에 표시됩니다.

2.  **생산성 바**: 노드(메시지, 질문 등)를 위한 도구(잘라내기, 복사,
붙여넣기, 삭제 등)에 접근할 수 있는 곳입니다.

3. **코파일럿, 코멘트, 변수, 주제 검사기, 세부 사항, 분석, 코드 편집기 열기
및 기본값으로 재설정 버튼:** 이 영역에는 다음이 포함됩니다:

**코파일럿:** 자연어 설명을 사용하여 주제를 만들고 업데이트하는 데
도움이 됩니다.

**코멘트:** 작성자가 노드에 코멘트를 남기고 협력할 수 있는 곳입니다.

**변수 메뉴:** 주제 수준 및 전역 변수를 확인하고, 테스트 탭에서 실행 시
변수 값을 볼 수 있는 곳입니다.

**주제 검사기:** 언제든지 작성 캔버스에서 실행하여 플랫폼에서 감지할 수
있는 오류를 확인할 수 있습니다(해결되지 않으면 봇 게시를 방지).

**세부 사항 버튼:** 주제 속성에 접근할 수 있는 곳입니다.

4.  **더 보기:**

**분석:** 주제 사용 메트릭을 보여줍니다.

**코드 편집기 열기:** 사용자 인터페이스를 코드 없는/저코드 환경에서
개발자가 직접 편집할 수 있는 기본 YAML 구성의 프로코드 보기로
전환합니다. 일부 시스템 주제의 경우, 기본값으로 재설정 옵션이 있어 주제
콘텐츠를 원래 상태로 되돌릴 수 있습니다.

5.  **저장 버튼:** 주제 변경 사항을 저장합니다.

6.  **주제 세부 사항 메뉴:** 작성자가 주제 이름, 표시 이름, 설명 및
상태(활성/비활성)를 업데이트할 수 있는 곳입니다. 생성 AI
오케스트레이션이 활성화된 경우, 표시 이름이 모델 표시 이름으로 대체되며
모델 설명이 추가로 사용 가능합니다. 입력과 출력을 구성할 수 있으며, 생성
AI를 오케스트레이터로 사용할 때 자동으로 슬롯을 채울 수 있습니다.

7.  **트리거 전환 버튼:** 모든 주제의 트리거 노드에 있으며, 기본적으로
새로운 주제는 구문 트리거(또는 생성 AI 오케스트레이션이 활성화된 경우,
코파일럿에 의해 트리거됨)를 갖지만, 메시지 수신, 이벤트 수신, 활동 수신,
대화 업데이트 수신, 호출 수신, 리디렉션 및 비활동으로 전환할 수
있습니다.

8.  **새 노드 추가:** 새 노드 추가 버튼을 사용하여 주제에 활동을 추가할 수
있습니다. 예를 들어, 메시지 보내기, 질문하기, 조건 추가 등을 통해 대화
논리를 구축할 수 있습니다.

9. **작성 캔버스 제어:** 작성 캔버스가 광범위한 주제에 대해 커질 수
있으므로 이 제어를 사용하여 탐색할 수 있습니다. 포함된 제어에는 캔버스
맵, 줌, 핸드, 선택 및 리셋이 있습니다.

## Task 3: Add content to your topic 작업 3: 주제에 콘텐츠 추가

이 연습은 주제에 많은 양의 콘텐츠를 추가하는 방법을 다루지는 않습니다.
대신, 하나의 질문 노드, 메시지 노드 및 주제 리디렉션을 추가하는 단계를
제공하여 Microsoft Copilot Studio에서 주제를 생성하고 테스트하고
게시하는 전체 프로세스를 익힐 수 있습니다. 이 모듈의 게시 데모
연습에서는 Microsoft Copilot Studio의 작성 기능에 대해 더 깊이 있게
검토합니다.

이 연습의 다음 섹션에서는 Microsoft Copilot Studio의 핵심 구성 요소를
이해하고 주제를 만드는 데 필요한 기본 지식을 다룹니다.

### Fundamental knowledge: Question node 기본 지식: 질문 노드

코파일럿 작성자로서 사용자의 응답을 기대하고 해당 정보에 기반하여 작업을
수행하려는 경우 질문 노드를 사용해야 합니다. 사용자 응답은 변수에
저장되며, 질문 노드는 엔터티와 슬롯 채우기 기능도 사용할 수 있습니다. 이
개념은 이 연습의 뒷부분에서 다룹니다.

질문 노드는 메시지 노드가 하는 많은 기능을 사용합니다. 예를 들어 리치
텍스트, 음성 작성 및 이미지, 비디오, 적응형 카드와 같은 리치 텍스트 응답
유형을 사용할 수 있습니다.

1.  이전 작업에서 열어둔 주제에서 캔버스의 기존 노드 아래에 있는 + 버튼을
선택한 다음 질문하기를 선택하여 새로운 질문 노드를 추가합니다.

2.  \"주문과 관련하여 무엇을 하고 싶으신가요?\"를 입력하고 식별 값이
\"사용자의 전체 응답\"으로 설정되어 있는지 확인합니다. 이 노드는 주제가
트리거된 후 사용자가 무엇을 원하는지 묻는 질문을 합니다. 게시 데모
연습에서는 엔터티와 슬롯 채우기를 사용하는 작업을 확장합니다.

3.  기본적으로 사용자 응답은 Var1이라는 변수에 저장됩니다. 변수 이름을 예를
들어 OrderRequest로 변경하려면 변수 이름을 클릭할 수 있습니다.

**Pro tips:**  변수를 항상 적절하게 이름을 지정하는 것이 모범 사례입니다.  이렇게 하면 논리에서 참조할 때 명확하게 식별할 수 있으며, 테스트를 수행하고 실행 시 변수 값을 확인할 때 명확성을 추가합니다. 고객 및 파트너는 일관성과 유지 관리 용이성을 위해 변수의 명명 규칙을 정의하고 따를 수 있습니다.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image21.png">

**Pro tips :** 
•	질문 동작은 속성 및 질문 동작을 클릭하여 사용자 지정할 수 있습니다. 여기에서 질문을 건너뛸 수 있는지,  사용자에게 질문을 다시 요청해야 하는 횟수  , 유효성 검사 규칙,  사용자가  예상대로 답변하지 않을 경우 어떻게 해야 하는지 정의할 수 있습니다.
•	또한 사용자가  질문에 답변하지 않고 다른 주제로 이동할 수 있는지 여부를 정의할 수  있으며, 중단 시 허용되는 주제 목록을 정의할 수 있습니다. 
•	사용자가 처음에 예상되는 내용을 이해하지 못하는 경우 재시도 프롬프트를 정의하는 것이 가장 좋습니다. 그런 다음 사용자가 질문에 적절하게 대답할 수 있도록 도와줄 때 훨씬 더 명확하게 설명해도 됩니다.


### Fundamental knowledge: Message node 기본 지식: 메시지 노드

메시지 노드는 사용자에게 메시지를 표시하는 데 사용할 수 있습니다. 이
메시지는 대화 주제에 따라 간단할 수 있습니다. 질문 노드와는 달리 메시지
노드는 사용자의 응답을 기대하거나 저장하지 않습니다. 메시지 노드에는
리치 텍스트 옵션도 있어 텍스트로 표시하거나 카드, 이미지, 비디오 및
적응형 카드와 같은 고급 옵션을 사용할 수 있습니다.

**Pro tips :**   코파일럿을 더 자연스럽고 인간적으로 들리게 하기 위해 메시지 변형을 구성할 수 있습니다. 이렇게 하면 코파일럿이 동일한  메시지를 반복하지 않고 구성된 메시지 중 하나를 보내게 됩니다.

메시지 노드 내에서 변수를 사용할 수 있어 사용자에게 표시되는 텍스트
본문이 저장된 데이터에 따라 동적일 수 있습니다. 이 기능을 통해 메시지를
더 개인화할 수 있습니다(예: \"안녕하세요 {System.User.FirstName}, 주문
세부 정보를 가져오겠습니다. 잠시만 기다려 주세요.\"). 변수는 데이터
자동화 또는 계산을 수행하는 데 사용할 수도 있습니다. 나중에 연습에서
변수를 더 깊이 다룹니다. 마지막으로 Power Fx 공식을 추가하여 더 동적인
콘텐츠를 만들 수 있습니다.

1.  질문 노드 아래의 + 버튼을 선택하여 다른 노드를 추가합니다. 그런 다음
메시지 보내기를 선택합니다. 고객의 질문에 감사하는 메시지를
입력합니다(예: \"질문해 주셔서 감사합니다!\").**\
**

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image22.png">

2.  이 데모 시나리오에서 고객의 대화를 종료합니다. 작성 캔버스 내의 메시지
노드 아래에서 + 버튼을 선택합니다. 주제 관리 옵션 위로 마우스를 가져간
다음 다른 주제로 이동을 선택하고 대화 종료를 선택합니다. 이는 대화
세션을 종료하는 전용 주제로 리디렉션되어 질문이 해결되었는지 확인하고
고객 만족도 설문조사를 작성하도록 제안합니다.\

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image23.png">

** Pro tip :** 개별 대화 경로를 대화 종료 주제로 끝내는 것이 모범 사례입니다. 이를 통해 최종 사용자는 질문이 해결되었는지  확인할 수 있습니다. 사용자가 확인하면 고객 만족도(CSAT) 설문조사가 표시됩니다. 해결률 및 CSAT 점수는 모두 코파일럿    분석에 표시됩니다.  

3.  그런 다음 화면 오른쪽 상단에서 저장 버튼을 선택합니다.

4.  테스트 창을 사용하여 봇이 예상대로 작동하는지 확인합니다. 새로운
테스트를 하기 전에 새로고침을 꼭 하세요.

```
I\'d like to check the status of my order please.
```
```
주문 상태를 확인하고 싶습니다.
```

**Pro tip :** 트리거 구문은 사용자가 말할 수 있는 모든 발화를   정확하게 일치시킬 필요는 없습니다.      

## Task 4: 코파일럿을 사용하여 Topic 만들기

Microsoft Copilot Studio에서 주제를 만드는 작업이 이전보다 더
쉬워졌습니다. 이제 주제가 해야 할 일을 자연어로 설명하여 Microsoft
Copilot Studio에서 주제를 만들 수 있습니다. 설명으로부터 만들기 기능을
사용하여 수동 단계의 일부를 줄여 자동으로 주제를 생성할 수 있습니다. 이
작업에서는 Copilot을 사용하여 주제를 얼마나 간단하고 빠르게 만들 수
있는지 학습합니다.

1.  화면 왼쪽의 탐색 창에서 주제를 선택합니다.

2.  만들기 드롭다운을 선택하고 주제를 선택한 다음 Copilot으로 설명에서
만들기를 선택합니다. 주제의 이름을 입력하고 설명을 입력하라는 새 창이
나타납니다.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image24.png">

3.  주제 이름 필드에 \"지원 티켓\"을 입력합니다.

4. \"설명을 입력하세요\" 공간에 주제의 목적을 설명하는 내용을 입력합니다.

```
Create a support ticket, including a title, severity (high / medium / low), description and an email address to send update notifications to. Define variables following this naming pattern: Topic.TicketTitle.
```
```
제목, 심각도(높음/중간/낮음), 설명 및 업데이트 알림을 보낼 이메일 주소를 포함한 지원 티켓을 만듭니다. Topic.TicketTitle이라는 명명 패턴에 따라 변수를 정의합니다.
```

5.  생성을 선택합니다.

<img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image25.png">

> Copilot은 트리거 구문, 질문 노드, 엔터티 선택, 변수 이름 지정 및
> 메시지 노드 확인을 포함한 주제를 생성합니다.

6.  작성 캔버스 상단의 Copilot 버튼을 선택합니다(이미 Copilot 패널이 열려
있지 않은 경우). Copilot 패널의 \"무엇을 하고 싶으신가요?\" 필드에 추가
지침을 입력한 다음 업데이트를 선택합니다.
```
Before the last message, ask a question to find out the user's preferred contact method, choosing from email, phone or SMS.
```

```
마지막 메시지를 보내기 전에 질문을 하여 이메일, 전화 또는 SMS 중에서 선택하여 사용자가 선호하는 연락 방법을 알아보세요.
```

 <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image26.png">

 Copilot은 고객에게 연락 방법을 묻고 선택을 변수에 저장하는 질문 노드를
 자동으로 추가합니다.

 <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image27.png">

**참고 :** 아래 오류가 발생하면 이 단계를 건너뛸 수 있습니다. 
 <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image28.png">


Microsoft Copilot Studio의 Copilot 기능은 작성 시간을 대폭 단축하여
자연어를 사용해 새 주제를 만들고 편집할 수 있습니다. 또한 Copilot 패널은
생성된 업데이트를 보여주고 주제에서 업데이트할 수 있는 제안을
제공합니다.

7.  새 주제를 저장합니다.

8.   <img src="https://github.com/FDX-edu/240819_CopilotEdu_test/raw/main/Lab%2001/media/image29.png">
테스트 창을 사용하여 봇이 예상대로 작동하는지 확인합니다. 새 대화를
시작하고 이전 대화를 다시 시작하지 않으려면 새로고침 아이콘을 사용하는
것을 주저하지 마세요.

```
I have an issue with my laptop and need to log a support ticket
```
```
노트북에 문제가 있어 지원 티켓을 기록해야 합니다.
```

