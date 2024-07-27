![](./output/lab6.docx/media/image1.png){width="0.9166666666666666in"
height="0.9166666666666666in"} Microsoft Copilot Studio

실습6: 생성형 AI 오케스트레이션을 사용하여 커넥터와 상호작용하기

Hands-on lab step-by-step

July 2024

Microsoft Copilot Studio Workshop

> Contents

[Microsoft Copilot Studio
[1](#microsoft-copilot-studio)](#microsoft-copilot-studio)

[Goals for this lab [1](#goals-for-this-lab)](#goals-for-this-lab)

[Prerequisites
[1](#prerequisites-사전-준비-사항)](#prerequisites-사전-준비-사항)

[Generative AI orchestration
[2](#generative-ai-orchestration-생성형-ai-오케스트레이션)](#generative-ai-orchestration-생성형-ai-오케스트레이션)

[Actions [3](#_Toc171001494)](#_Toc171001494)

[Summary [8](#summary-요약)](#summary-요약)

[Terms of Use [**오류! 책갈피가 정의되어 있지
않습니다.**](#_Toc171001496)](#_Toc171001496)

# Microsoft Copilot Studio 

> This lab is subject to the Terms of Use found at the end of this
> document.

## Goals for this lab 

+-------------------------------------------------+--------------------+
| After this lab you will be able to:             | -   The time to    |
|                                                 |     complete this  |
| -   Understand the basics of plugin actions     |     lab is \[20\]  |
|                                                 |     minutes.       |
| -   Use Copilot Studio to request data from     |                    |
|     another data source using plugin actions in | -   이 실습을      |
|     a basic use case (using the MSN Weather     |     완료하는 데    |
|     Connector) and return the data in a         |     걸리는 시간은  |
|     conversational dialog with a customer or    |     약 20분입니다. |
|     user                                        |                    |
|                                                 |                    |
| -   플러그인 작업의 기본 사항을 이해할 수       |                    |
|     있습니다.                                   |                    |
|                                                 |                    |
| -   Copilot Studio를 사용하여 플러그인 작업을   |                    |
|     통해 다른 데이터 소스에서 데이터를 요청하고 |                    |
|     이를 고객 또는 사용자와의 대화에서 반환할   |                    |
|     수 있습니다(예: MSN Weather Connector       |                    |
|     사용).                                      |                    |
+=================================================+====================+
+-------------------------------------------------+--------------------+

## Prerequisites 사전 준비 사항

> 일부 실습, 특히 후반부 실습은 이전 실습의 기능과 작업을 참조합니다.
> 그러나 대부분의 실습은 Microsoft Copilot Studio 체험판에 접속할 수
> 있는 경우 이전 모듈을 완료하지 않아도 진행할 수 있도록 설계되었습니다.
> 하지만 제품의 기능과 특성을 최대한 활용하려면 특정 모듈을 완료한 후
> 실습을 시작하는 것이 좋습니다.

-   인터넷에 접속할 수 있는 컴퓨터

-   제공된 Microsoft 테넌트에 로그인할 수 있는 권한 (일부 회사는
    사용자가 회사 테넌트에만 접속하도록 제한할 수 있습니다)

