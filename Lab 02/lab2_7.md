# 음성 작성

Microsoft Copilot Studio 내에서 Copilot 제작자는 Message 및 Question
노드에서 SSML(Speech Synthesis Markup Language) 태그를 사용하여 음성
지원 부조종사에 Microsoft Copilot Studio를 사용할 때 동작을 확장할 수
있습니다. 텍스트 작성 및 음성 작성에 Microsoft Copilot Studio를 사용할
수 있습니다. 기본적으로 음성 지원 채널에서는 메시지 노드에 입력된 메시지
텍스트가 텍스트 표시 및 음성에 사용됩니다. 텍스트와 음성에 대해 다른
동작을 제공하여 이 동작을 재정의할 수 있습니다. 예를 들어 문장의 특정
영역이나 이미지 메시지에 더 중점을 두려는 경우 소리 내어 읽을 수 있는
대체 설명을 제공하려는 경우 동작을 재정의할 수 있습니다.

SSML을 사용하는 경우 자연스러운 말처럼 들리도록 텍스트를 합성된 음성으로
변환하는 방법을 설정할 수 있습니다. **Audio**, **Break**, **Emphasis**,
**Prosody**와 같은 SSML 태그를 사용하여 문장이 말하는 방식의 동작을
변경할 수 있습니다.

-   **오디오** - 사전 녹음된 오디오를 추가합니다.
-   **Break** - 단어 사이에 일시 중지 또는 중단을 삽입합니다.
-   **강조** - 단어와 구문에 스트레스 수준을 추가합니다.
-   **운율** - 피치, 윤곽, 범위, 속도 및 볼륨에 대한 변경 사항을 지정합니다.

자세한 내용은 [Speech Synthesis Markup Language](https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/speech-synthesis-markup/)를 참조하세요.

