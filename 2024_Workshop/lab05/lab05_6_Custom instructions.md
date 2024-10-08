# Custom instructions (맞춤형 지시 사항)

프롬프트 수정을 통해 생성적 응답 및 지식 소스의 기능을 확장하여 맞춤형 지시 사항을 추가할 수 있습니다. </br>
맞춤형 지시 사항을 사용할 때는 프롬프트 엔지니어링에 대한 모범 사례를 따르는 것이 중요합니다. </br>
다음은 이 기능을 최대한 활용하기 위한 몇 가지 팁입니다:

-   **구체적으로:** 맞춤형 지시 사항은 명확하고 구체적이어야 하며, 코파일럿이 무엇을 해야 할지 정확히 이해할 수 있어야 합니다.
    모호하거나 애매한 언어는 혼동이나 잘못된 응답을 유발할 수 있습니다.

-   **예제 사용:** 예제를 제공하여 지시 사항을 설명하고 코파일럿이 기대하는 바를 이해하도록 돕습니다. 
    예제는 코파일럿이 정확하고 관련성 있는 응답을 생성하는 데 도움이 됩니다.

-   **간단하게 유지:** 맞춤형 지시 사항에 너무 많은 세부 정보나 복잡한 논리를 추가하지 마십시오. 
    지시 사항을 간단하고 명확하게 유지하여 코파일럿이 효과적으로 처리할 수 있도록 합니다.

-   **대안 제공:** 코파일럿이 할당된 작업을 완료할 수 없을 때를 대비한 대안을 제공하십시오. 
    예를 들어, 사용자가 질문할 때 \"답변이 없으면 \'찾을 수 없음\'으로 응답\"과 같은 대안을 포함할 수 있습니다. 
    이러한 대안은 코파일럿이 잘못된 응답을 생성하는 것을 방지하는 데 도움이 됩니다.

-   **테스트 및 개선:** 맞춤형 지시 사항이 의도한 대로 작동하는지 철저히 테스트하는 것이 중요합니다. 
    필요에 따라 조정하여 코파일럿의 응답 정확성과 효과를 향상시킵니다.

## 작업 1: 생성형 AI 오케스트레이션을 위한 맞춤형 지시 사항 구성

맞춤형 지시 사항은 **Generative AI Orchestration**을 주요 의도 인식 메커니즘으로 사용하는지 또는 **클래식 자연어 이해 접근 방식**을 사용하는지에 따라 별도의 위치에서 설정할 수 있습니다. </br>
**Generative AI Orchestration**이 활성화된 경우 지시 사항은 **코파일럿 수준**에서 설정해야 합니다.

1.  먼저 생성 AI 오케스트레이션이 활성화되어 있는지 확인합니다. 상단 메뉴에서 **Settings** 탭으로 이동합니다.

2.  **Generative AI** 메뉴로 이동합니다.

3.  **\"How should your copilot decide how to respond?\"** 에서 **\"Generative\"** 를 선택합니다.

4.  설정을 저장하고 닫습니다.

5.  상단 메뉴에서 **Overview** 탭으로 이동합니다.

6.  **Details** 영역에서 **Edit**을 선택합니다.

7.  **Instructions**을 업데이트합니다. 사용자 맥락에 특정한 변수를 사용할 수 있음을 주목하십시오.

    ```
    해적처럼 말하고 해적 표현을 사용하세요.
    응답에 이모티콘을 사용하세요.
    50단어 이내로 답변하세요.
    Microsoft 제품과 관련이 없는 질문에는 답변하지 마세요.
    ```

8.  저장합니다.

    <img src="./images/image16.png">

## 작업 2: 클래식 오케스트레이션을 위한 맞춤형 지시 사항 구성

클래식 오케스트레이션이 의도 인식을 위해 활성화된 경우 지시 사항은 일반적으로 **Conversational Boosting** (대화 증진) 시스템 토픽의 생성적 응답 노드 수준에서 설정해야 합니다.
(이 노드는 어디에나 추가될 수 있음).

1. 클래식 오케스트레이션이 활성화되어 있는지 확인합니다. 상단메뉴에서 **Settings** 탭으로 이동합니다.

2. **Generative AI** 메뉴로 이동합니다.

3.  **\"How should your copilot decide how to respond?\"** 에서 **\"Classic\"** 을 선택합니다.

4. **Settings**을 저장하고 닫습니다.

5. 상단메뉴에서 **Topics** 탭으로 이동합니다.

6. **System** Topic 영역을 선택합니다.

7. **Conversational boosting** 토픽을 선택합니다.

8. **Create generative answers** 속성으로 이동합니다.

9.  지시 사항을 사용자 지정할 수 있는 텍스트 영역이 있습니다. 여기에 맞춤형 지시 사항을 추가합니다.

    ```
    해적처럼 말하고 해적 표현을 사용하세요.
    답변에 이모티콘을 사용하세요.
    50단어 이내로 답변하세요.
    ```
    
    <img src="./images/image17.png">

10. 저장합니다.

## Task 3: 맞춤형 지시 사항 테스트

1. **Test** 창을 엽니다.

2. 기존 토픽과 일치하지 않는 질문을 하여 대화 증진 토픽을 트리거합니다.

    ```
    태양에 가장 가까운 행성부터 가장 먼 행성까지 나열해 볼 수 있나요?
    ```

    
    <img src="./images/image18.png" width="400">

 


