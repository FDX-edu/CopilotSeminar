![](./output/lab1.docx/media/image2.svg){width="0.9251334208223972in"
height="0.9251334208223972in"} Microsoft Copilot Studio

실습 01: Microsoft Copilot Studio에서 첫 번째 코파일럿 만들기

실습 단계별 안내

2024년 7월

Microsoft Copilot Studio 워크숍

Contents

[Microsoft Copilot Studio
[1](#microsoft-copilot-studio)](#microsoft-copilot-studio)

[이 실습의 목표 [1](#이-실습의-목표)](#이-실습의-목표)

[사전 준비 [1](#사전-준비)](#사전-준비)

[연습 1: 코파일럿 만들기를 위해 로그인하기
[2](#연습-1-코파일럿-만들기를-위해-로그인하기)](#연습-1-코파일럿-만들기를-위해-로그인하기)

[연습 2: 사용자 인터페이스 빠르게 둘러보기
[7](#연습-2-사용자-인터페이스-빠르게-둘러보기)](#연습-2-사용자-인터페이스-빠르게-둘러보기)

[연습 3: 코파일럿 테스트하기
[12](#연습-3-코파일럿-테스트하기)](#연습-3-코파일럿-테스트하기)

[연습 4: 첫 번째 주제 만들기
[16](#연습-4-첫-번째-주제-만들기)](#연습-4-첫-번째-주제-만들기)

[연습 5: 테스트를 위해 데모 웹사이트에 코파일럿 게시하기
[31](#연습-5-테스트를-위해-데모-웹사이트에-코파일럿-게시하기)](#연습-5-테스트를-위해-데모-웹사이트에-코파일럿-게시하기)

[이용 약관 [35](#이용-약관)](#이용-약관)

# Microsoft Copilot Studio 

> 이 실습은 문서 말미의 이용 약관에 따릅니다.

## 이 실습의 목표

+-------------------------------------------------+--------------------+
| 이 실습 후, 다음을 수행할 수 있습니다.          | 이 실습을 완료하는 |
|                                                 | 데                 |
| -   Microsoft Copilot Studio의 통합 작성        |                    |
|     캔버스를 사용하여 새로운 맞춤형 코파일럿을  | 약 40분이          |
|     만듭니다.                                   | 걸립니다.          |
|                                                 |                    |
| -   첫 번째 주제를 만들고, 리치 텍스트 응답을   |                    |
|     포함한 콘텐츠를 주제에 추가합니다.          |                    |
|                                                 |                    |
| -   Microsoft Copilot Studio의 새로운 코파일럿  |                    |
|     기능을 사용하여 AI로 주제를 만듭니다.       |                    |
|                                                 |                    |
| -   Microsoft Copilot Studio에서 봇을           |                    |
|     테스트하는 방법을 학습합니다.               |                    |
|                                                 |                    |
| -   데모 웹사이트에 봇을 게시합니다.            |                    |
+=================================================+====================+
+-------------------------------------------------+--------------------+

## 사전 준비

> 일부 실습은 이전 실습에서 다룬 기능과 작업을 참조합니다. 실습은 대부분
> Microsoft Copilot Studio 평가판에 액세스할 수 있으면 이전 모듈을
> 완료하지 않아도 진행할 수 있도록 설계되었습니다. 그러나 제품의 기능과
> 기능을 제대로 보여주기 위해 특정 모듈을 완료한 후에 일부 실습을
> 시작하는 것이 좋습니다.
>
> Lab 01: Microsoft Copilot Studio에서 첫 번째 코파일럿 만들기에는
> 다음이 필요합니다:

-   인터넷 액세스가 가능한 컴퓨터

-   제공된 Microsoft 테넌트에 로그인할 수 있어야 합니다 (일부 회사는
    사용자가 회사 테넌트에만 연결하도록 강제할 수 있습니다).

## 연습 1: 코파일럿 만들기를 위해 로그인하기

> 이 연습에서는 제공된 자격 증명을 사용하여 Microsoft Copilot Studio
> 작성 환경에 로그인합니다.

### 작업 1: 브라우저 환경 설정

기존에 로그인한 경험과 충돌을 피하기 위해 다음 세 가지 옵션 중 하나를
사용하여 이 실습을 수행할 수 있습니다.

1.  **Set up a new work profile** specific to that workshop

**해당 워크숍에 특정한 새 작업 프로필 설정**

+------+---------------------------------------------------------------+
| ![Li | **Pro tip**: best option to switch between your work and      |
| ghts | trial environments while keeping history of your work. Ideal  |
| On   | if you want to continue using the account later.              |
| out  |                                                               |
| line | **Pro tip:** 작업 환경과 평가판 환경 간에 작업 기록을         |
| ](./ | 유지하면서 전환하는 가장 좋은 옵션입니다. 나중에 계정을 계속  |
| outp | 사용하려는 경우 이상적입니다.                                 |
| ut/l |                                                               |
| ab1. |                                                               |
| docx |                                                               |
| /med |                                                               |
| ia/i |                                                               |
| mage |                                                               |
| 4.sv |                                                               |
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

2.  Or **browse as a guest**.

게스트로 브라우징

3.  Or **start an InPrivate session**.

InPrivate 세션 시작

![](./output/lab1.docx/media/image5.png){width="7.514583333333333in"
height="0.8548611111111111in"}

### 작업 2: Copilot Studio에 로그인하기

1.  Navigate to
    [aka.ms/CopilotStudioStart](https://aka.ms/CopilotStudioStart)

aka.ms/CopilotStudioStart로 이동

2.  Enter the provided user name, click **Next**

**제공된 사용자 이름을 입력하고 다음을 클릭**

3.  Enter the provided password, click

**Sign in 제공된 비밀번호를 입력하고 로그인 클릭**

4.  If prompted, choose whether to **stay signed in**.

계속 로그인할지 묻는 메시지가 나타나면 선택

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image6.png){width="3.1311318897637794in"
height="2.9361056430446193in"}

5.  The first time you access Microsoft Copilot Studio, you'll be
    prompted to choose your country/region. You can choose a value or
    leave the default option and click **Get Started**.

Microsoft Copilot Studio에 처음 액세스하면 국가/지역을 선택하라는
메시지가 표시됩니다. 값을 선택하거나 기본 옵션을 그대로 두고 시작하기를
클릭할 수 있습니다.

### 작업 3: 코파일럿 만들기

1.  From the Microsoft Copilot Studio **Home** page, **describe** your
    copilot to create it.

Microsoft Copilot Studio 홈페이지에서 코파일럿을 설명하여 만듭니다.

+----+----+------------------------------------------------------+----+
|    | ![ | I want to a copilot for my customer support. It is   |    |
|    | Op | an assistant for Contoso customers, helping to       |    |
|    | en | answer common questions and help with common tasks,  |    |
|    | q  | like checking an order status                        |    |
|    | uo |                                                      |    |
|    | ta | 고객 지원을 위한 코파일럿을 만들고 싶습니다. 이는    |    |
|    | ti | Contoso 고객이 일반적인 질문에 답변하고 주문 상태    |    |
|    | on | 확인과 같은 일반적인 작업을 도와주는 도우미입니다.   |    |
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
|    | b1 |                                                      |    |
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

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image9.png){width="7.514583333333333in"
height="3.765277777777778in"}

2.  You will get redirected to a conversational experience to further
    customize your copilot. You can provide further details to the
    description (you can **decline** to do so), and you will also be
    prompted for a **tone of voice**.

대화형 경험으로 리디렉션되어 코파일럿을 사용자 정의할 수 있습니다.
설명에 추가 세부 정보를 제공할 수 있으며, 톤 설정을 요청받습니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Playful tone, joyful, customer focus, but definitely |    |
|    | Op | professional                                         |    |
|    | en |                                                      |    |
|    | q  | 놀랍고 즐거운 고객 중심의 전문적인 톤으로            |    |
|    | uo | 설정합니다.                                          |    |
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
|    | b1 |                                                      |    |
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

3.  You will also get asked for **publicly accessible websites** to get
    information from.

공개적으로 접근 가능한 웹사이트를 정보 소스로 요청받습니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Information should come from                         |    |
|    | Op | https:/                                              |    |
|    | en | /learn.microsoft.com/en-us/microsoft-copilot-studio/ |    |
|    | q  | and from                                             |    |
|    | uo | https://www.microsoft.com/en-us/microsoft-copilot/   |    |
|    | ta |                                                      |    |
|    | ti | 정보는                                               |    |
|    | on | https:/                                              |    |
|    | ma | /learn.microsoft.com/en-us/microsoft-copilot-studio/ |    |
|    | rk | 및                                                   |    |
|    | ou | ht                                                   |    |
|    | tl | tps://www.microsoft.com/en-us/microsoft-copilot/에서 |    |
|    | in | 가져와야 합니다.                                     |    |
|    | e] |                                                      |    |
|    | (. |                                                      |    |
|    | /o |                                                      |    |
|    | ut |                                                      |    |
|    | pu |                                                      |    |
|    | t/ |                                                      |    |
|    | la |                                                      |    |
|    | b1 |                                                      |    |
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

4.  You will also get asked **topics or tasks** the copilot **shouldn't
    help with or talk about**.

코파일럿이 도와주거나 논의하지 않아야 할 주제나 작업도 요청받습니다.

+----+----+------------------------------------------------------+----+
|    | ![ | We don\'t want to discuss other brands like          |    |
|    | Op | Fabrikam. Never provide product comparisons with     |    |
|    | en | competitor technologies.                             |    |
|    | q  |                                                      |    |
|    | uo | 다른 브랜드(Fabrikam 등)에 대한 논의는 원하지        |    |
|    | ta | 않습니다. 경쟁사 기술과의 제품 비교는 절대 제공하지  |    |
|    | ti | 않습니다.                                            |    |
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
|    | b1 |                                                      |    |
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

5.  When prompted, you can answer I'm done

필요한 정보를 모두 입력하면 \"완료\"를 클릭합니다.

6.  Before you create your copilot, go the "**...**" and "**Edit
    advanced settings**" menu to update the copilot **schema name**
    (because contrary to the copilot *display* name, the schema name is
    a technical property that can't be changed afterwards and must be
    unique) and save it a **solution** (e.g. "Copilot Studio Workshop")
    to be able to export it later and inherit from the solution
    publisher prefix).

코파일럿을 생성하기 전에 \"\...\" 및 \"고급 설정 편집\" 메뉴로 이동하여
코파일럿 스키마 이름을 업데이트하고(코파일럿 표시 이름과 달리 스키마
이름은 고유해야 하며 나중에 변경할 수 없음), 솔루션(예: \"Copilot Studio
Workshop\")에 저장합니다.

+------+---------------------------------------------------------------+
| !    | Make sure you pick a unique name for your custom copilot      |
| [War | (both display name and schema name).                          |
| ning |                                                               |
| outl | 사용자 지정 코파일럿의 고유한 이름(표시 이름과 스키마 이름)을 |
| ine] | 선택해야 합니다.                                              |
| (./o |                                                               |
| utpu |                                                               |
| t/la |                                                               |
| b1.d |                                                               |
| ocx/ |                                                               |
| medi |                                                               |
| a/im |                                                               |
| age1 |                                                               |
| 1.sv |                                                               |
| g){w |                                                               |
| idth |                                                               |
| ="0. |                                                               |
| 4393 |                                                               |
| 0664 |                                                               |
| 9168 |                                                               |
| 8538 |                                                               |
| 7in" |                                                               |
| hei  |                                                               |
| ght= |                                                               |
| "0.4 |                                                               |
| 3930 |                                                               |
| 6649 |                                                               |
| 1688 |                                                               |
| 5387 |                                                               |
| in"} |                                                               |
+======+===============================================================+
+------+---------------------------------------------------------------+

7.  You can then choose "**Create**".

그런 다음 \"생성\"을 선택할 수 있습니다.

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image12.png){width="7.514583333333333in"
height="3.765277777777778in"}

+------+---------------------------------------------------------------+
| ![Li | 1.  You can choose to avoid the conversational creation       |
| ghts |     experience by selecting "**Skip to configure**"           |
| On   |                                                               |
| out  | 2.  You can set the copilot's primary language in the "**Edit |
| line |     language**" menu. For the lab, be sure to remain in       |
| ](./ |     English (en-US).                                          |
| outp |                                                               |
| ut/l | 3.  It is a best practice to always configure your copilot in |
| ab1. |     the **context of your own solution** and **publisher**,   |
| docx |     so that the copilot is created with the desired publisher |
| /med |     prefix, and so that you can easily **export it and deploy |
| ia/i |     it to other environments**.                               |
| mage |                                                               |
| 4.sv | 1\. \"구성할 건너뛰기\"를 선택하여 대화형 작성 환경을         |
| g){w | 피하도록 선택할 수 있습니다                                   |
| idth |                                                               |
| ="0. | 2\. \"언어 편집\" 메뉴에서 부조종사의 기본 언어를 설정할 수   |
| 4724 | 있습니다. 실험실의 경우 영어(en-US)로 남아 있어야 합니다.     |
| 4094 |                                                               |
| 4881 | 3\. 항상 자신의 솔루션과 게시자의 맥락에서 코파일럿을         |
| 8897 | 구성하여 원하는 게시자 접두사로 코파일럿을 생성하고 쉽게      |
| 6in" | 내보내고 다른 환경에 배포할 수 있도록 하는 것이 좋습니다.     |
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

## 연습 2: 사용자 인터페이스 빠르게 둘러보기

Microsoft Copilot Studio는 기본부터 고급 코파일럿을 쉽게 만들 수 있도록
도와줍니다. 이 섹션에서는 Microsoft Copilot Studio의 주요 페이지를
검토합니다.

### Main interface 주요 인터페이스

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image13.png){width="7.514583333333333in"
height="3.765277777777778in"}

A.  **Home** -- Displays Microsoft Copilot Studio home page. This is the
    page where you initially landed. You can start creating new copilots
    from here, it contains the list of recent copilots, a list of
    templates to avoid creating new copilots from scratch, as well as
    learning resources.

> **Create** -- This menu gets you to the conversational copilot
> creation experience.\
> **Copilots** -- List of all the copilots your user has access to in
> the environment.\
> **Library** -- List of connectors available for the extension of
> Microsoft 1^st^-party copilots.
>
> **홈:** Microsoft Copilot Studio 홈페이지를 표시합니다. 여기에서 새
> 코파일럿을 만들 수 있으며, 최근 코파일럿 목록, 템플릿 목록, 학습 자료
> 등이 포함되어 있습니다.
>
> **생성:** 대화형 코파일럿 생성 경험으로 이동합니다.
>
> **코파일럿:** 사용자 환경에서 액세스할 수 있는 모든 코파일럿 목록을
> 표시합니다.
>
> **라이브러리:** Microsoft 1st-party 코파일럿 확장을 위한 커넥터 목록을
> 표시합니다.

B.  **Copilots** -- List of available copilots that you can customize
    and quickly navigate to.

> 코파일럿 목록에서 사용 가능한 코파일럿을 커스터마이징하고 빠르게
> 탐색할 수 있습니다.

+------+---------------------------------------------------------------+
| ![Li | **Pro tip**: when you work on a single copilot, you should    |
| ghts | **unpin** **the list of copilots** to get more screen real    |
| On   | estate for your authoring.                                    |
| out  |                                                               |
| line | Pro tip: 단일 코파일럿 작업 시 코파일럿 목록 고정을 해제하여  |
| ](./ | 작성 공간을 더 많이 확보할 수 있습니다.                       |
| outp |                                                               |
| ut/l |                                                               |
| ab1. |                                                               |
| docx |                                                               |
| /med |                                                               |
| ia/i |                                                               |
| mage |                                                               |
| 4.sv |                                                               |
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

C.  **Menu** -- Tabbed navigation between the most useful Copilot Studio
    capabilities.

> 메뉴 -- 가장 유용한 Copilot Studio 기능 간의 탭 탐색
>
> **Overview** -- Description of the copilot, its instructions, and
> quick view of its configuration (knowledge sources, topics, actions,
> publish status, etc.)
>
> **개요:** 코파일럿 설명, 지침 및 구성(지식 소스, 주제, 작업, 게시 상태
> 등)을 빠르게 확인할 수 있습니다.
>
> **Knowledge** -- Where you manage the copilot knowledge sources
> (website, files, etc.)
>
> **지식:** 코파일럿의 지식 소스(웹사이트, 파일 등)를 관리하는 곳입니다.
>
> **Topics** - Where you manage custom and system topics. Topics are the
> core building blocks of a copilot. Topics can be seen as the copilot
> competencies: they define how a conversation dialog plays out. Topics
> are discrete conversation paths that, when used together, allow for
> users to have a conversation that feels natural and flows
> appropriately.
>
> **주제:** 사용자 정의 주제와 시스템 주제를 관리하는 곳입니다. 주제는
> 코파일럿의 핵심 구성 요소로, 대화가 어떻게 진행되는지를 정의합니다.
> 주제는 개별 대화 경로로, 함께 사용하면 자연스럽고 적절하게 흐르는
> 대화를 할 수 있습니다.
>
> **Actions** -- Where you manage action. Actions are pieces of logic
> with inputs and outputs. They leverage Power Platform components such
> as connectors, Power Platform cloud flows, AI Builder custom prompts,
> or Bot Framework skills. Actions are useful to leverage generative AI
> to both prompt the user for the necessary inputs but also to summarize
> the output of the action in the desired format.
>
> **작업:** 작업을 관리하는 곳입니다. 작업은 입력과 출력을 가진 논리
> 조각입니다. 커넥터, Power Platform 클라우드 흐름, AI Builder, 사용자
> 정의 프롬프트 또는 Bot Framework 스킬과 같은 Power Platform 구성
> 요소를 활용합니다. 작업은 생성 AI를 활용하여 필요한 입력을 유도하고
> 원하는 형식으로 작업 출력을 요약하는 데 유용합니다.
>
> **Analytics** -- Where you can view metrics to monitor how well your
> copilot is serving your users and identify ways to improve it.
>
> **분석:** 코파일럿이 사용자에게 얼마나 잘 제공되고 있는지 모니터링하고
> 개선 방법을 식별할 수 있는 메트릭을 확인하는 곳입니다.
>
> **Channels** -- Where you configure how your copilot is being made
> available to your users (e.g. Teams, website, etc.)
>
> **채널:** 사용자에게 코파일럿을 제공하는 방법을 구성하는 곳입니다(예:
> Teams, 웹사이트 등).

D.  **Overview --** Where you can edit the copilot description, its
    generative AI instructions, and also where you can have a quick view
    of its configuration (knowledge sources, topics, actions, publish
    status, etc.)

> **개요 --** Copilot 설명, 생성 AI 설명 및 구성(지식 소스, 주제, 작업,
> 게시 상태 등)을 빠르게 볼 수 있는 편집 가능

E.  **Environment** -- Where you can identify the Power Platform
    environment you're working from. You would typically create and
    author a copilot in a development environment and deploy it to test
    and production environments.

**환경**: 작업 중인 Power Platform 환경을 식별할 수 있는 곳입니다. 보통
개발 환경에서 코파일럿을 만들고 작성한 후 테스트 및 프로덕션 환경에
배포합니다.

F.  **Publish** -- Where you can make the latest version of your copilot
    available to your users. Apart from the test pane, changes are not
    reflected to your end-users as long as you have not published the
    copilot.\
    **Settings** -- Where you can managed your copilot configuration
    (advanced settings, security, language, etc.)

> **게시**: 최신 버전의 코파일럿을 사용자에게 제공할 수 있는 곳입니다.
> 테스트 창 외에는 코파일럿을 게시하지 않으면 변경 사항이 최종
> 사용자에게 반영되지 않습니다.
>
> **설정**: 코파일럿 구성(고급 설정, 보안, 언어 등)을 관리하는 곳입니다.

G.  **Test your copilot** -- The test pane allows you to immediately
    test your copilot and your customizations, even without needing to
    save.

> **코파일럿 테스트**: 테스트 창을 통해 저장할 필요 없이 즉시 코파일럿과
> 사용자 정의를 테스트할 수 있습니다.

### Settings interface 설정 인터페이스

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image14.png){width="7.485681321084864in"
height="5.794444444444444in"}

1.  **Copilot details 코파일럿 세부 사항**-- 코파일럿 표시 이름,
    아이콘을 업데이트하고 고급 설정을 수정하는 곳입니다(예: Azure
    Application Insights 통합 구성).

2.  **AI integration tools AI 통합 도구** Azure AI for Language(의도
    인식 및 엔터티 추출용), Azure OpenAI(지식 소스로서 Azure AI 검색
    인덱스와 결합하여 사용), Bot Framework SDK(기존 Azure AI Bot Service
    봇을 스킬로 호출하기 위해 사용)와 같은 고급 확장 도구 리소스.

3.  **Generative AI** **생성형 AI**-- 주제 트리거링 및 엔터티 추출을
    위한 더 고전적인 자연어 이해 접근 방식을 다중 의도 탐지 및 더 복잡한
    엔터티 추출을 수행하는 대형 언어 모델 기반 접근 방식으로 대체할 수
    있는 곳입니다. 또한, 지식 소스에 대한 콘텐츠 조정 설정을 구성하여
    환각 발생 위험을 줄일 수 있습니다.

4.  **Security 보안 :** 다른 사용자와 코파일럿을 공유(공동 작성)하거나
    보안 그룹과 공유(사용)할 수 있는 곳입니다. 최종 사용자 인증
    설정(인증 유형 및 적용 여부) 및 웹 채널 보안도 구성할 수 있습니다.
    이를 통해 웹 또는 사용자 정의 애플리케이션 배포에 사용되는 Direct
    Line 채널을 더욱 안전하게 할 수 있습니다.

5.  **Entities** **스킬 :** Copilot Studio에는 사용자 발화에서 주요
    정보를 식별하는 데 도움이 되는 많은 사전 구축된 엔터티가 포함되어
    있습니다(예: 도시, 날짜, 번호 등). 이 메뉴에서는 폐쇄형 목록 엔터티
    또는 정규식 엔터티를 정의할 수도 있습니다.

6.  **Skills 스킬 :** Copilot Studio 코파일럿이 호출할 수 있는 외부 Bot
    Framework 스킬을 등록하거나 기존 Azure Service Bot이 Copilot Studio
    코파일럿을 스킬로 사용할 수 있도록 구성하는 곳입니다.

7.  **Languages 언어:**-- 코파일럿을 사용할 수 있는 추가 언어를 구성하고
    지역화할 수 있는 곳입니다.

8.  **Language understanding** **언어 이해** -- Azure Conversational
    Language Understanding(CLU)에서 Azure AI Language로 개발 및 훈련된
    사용자 정의 언어 모델을 구성할 수 있는 곳입니다. 구성된 경우, 이는
    의도 감지를 위한 기본 제공 자연어 이해 모델(NLU)을 효과적으로 대체할
    수 있으며, 엔터티 감지 및 추출도 대체할 수 있습니다.

## 연습 3: 코파일럿 테스트하기

1.  To show the **Test copilot** pane, in the top-right corner of the
    screen, select **Test**.

화면 오른쪽 상단의 테스트를 선택하여 테스트 코파일럿 창을 표시합니다.

![A screenshot of a phone Description automatically
generated](./output/lab1.docx/media/image15.png){width="3.3464566929133857in"
height="5.072926509186352in"}

2.  The **Test copilot** pane shows that a message has already been sent
    to you from the copilot. This message was sent from the
    **Conversation Start** topic, which begins automatically. At the
    **Ask a question or describe what you need** prompt, at the bottom
    of the **Test copilot** pane, enter Hello and then select the
    **Send** button.

테스트 코파일럿 창에는 코파일럿으로부터 이미 메시지가 전송되었음을
보여줍니다. 이 메시지는 자동으로 시작되는 대화 시작 주제에서
전송되었습니다. 테스트 코파일럿 창 하단의 \"질문을 하거나 필요한 것을
설명하세요\" 프롬프트에 \"Hello\"를 입력하고 전송 버튼을 선택합니다.

![A screenshot of a chat Description automatically
generated](./output/lab1.docx/media/image16.png){width="3.3464566929133857in"
height="4.903140857392826in"}

The Copilot will offer a greeting in the **Test Copilot** pane

코파일럿이 테스트 코파일럿 창에서 인사말을 제공합니다.

3.  In the **Test copilot** pane, enter stores near me as the message
    and then select the **Send** button. One of the prebuilt topics
    (*Lesson 2 - A simple topic with a condition and variable*) will be
    triggered in the copilot, and it will ask you what location you\'re
    interested in.

테스트 코파일럿 창에 \"stores near me\"라는 메시지를 입력하고 전송
버튼을 선택합니다. 코파일럿의 사전 구축된 주제 중 하나(연습 2 - 조건과
변수를 가진 간단한 주제)가 트리거되며, 관심 있는 위치를 묻습니다.

4.  In the test chat, select the store location that you want. The
    copilot will respond with specific information based on your
    selection.

테스트 채팅에서 원하는 상점 위치를 선택합니다. 코파일럿은 선택한 위치에
따라 특정 정보를 제공합니다.

![A screenshot of a chat Description automatically
generated](./output/lab1.docx/media/image17.png){width="3.3464566929133857in"
height="4.672415791776028in"}\
\
Now that you\'ve reviewed an existing topic, you can move on to the next
exercise to create a new topic.

이제 기존 주제를 검토했으므로 다음 연습으로 넘어가 새 주제를 만들 수
있습니다.

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   Click on a message in the test pane to get redirected to  |
| out  |     the exact topic and node it was used in.                  |
| line |                                                               |
| ](./ | -   When in a topic, you can access the variables values      |
| outp |     (e.g., the selected store location) in the Variables      |
| ut/l |     menu. Within this menu, the Test tab displays the current |
| ab1. |     value at run time.                                        |
| docx |                                                               |
| /med | **Pro tip:** 테스트 창에서 메시지를 클릭하면 사용된 정확한    |
| ia/i | 주제와 노드로 리디렉션됩니다.                                 |
| mage |                                                               |
| 4.sv | 주제에 있을 때 변수 메뉴에서 변수 값을 확인할 수 있습니다(예: |
| g){w | 선택한 상점 위치). 이 메뉴의 테스트 탭에서 실행 시 현재 값을  |
| idth | 표시합니다.                                                   |
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

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image18.png){width="7.514583333333333in"
height="4.944444444444445in"}

## 연습 4: 첫 번째 주제 만들기

### Task 1: Create a new topic manually 작업 1: 새 주제 수동으로 만들기

첫 번째 작업에서는 다음 단계를 따라 새 주제를 수동으로 만듭니다:

1.  Select **Topics** in the left menu within Microsoft Copilot Studio.

Microsoft Copilot Studio의 왼쪽 메뉴에서 주제를 선택합니다.

2.  From the **Add a topic** drop down at the top of the screen, select
    the **From blank** option.

화면 상단의 주제 추가 드롭다운에서 빈 상태에서 옵션을 선택합니다.

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image19.png){width="5.701832895888014in"
height="1.9506681977252844in"}

3.  Rename your topic title, by clicking on **untitled** and renaming it
    to Check Order Status.

주제 제목을 \"untitled\"에서 \"Check Order Status\"로 클릭하여 이름을
바꿉니다.

4.  Select **Phrases**, under the topic Trigger, and select **Edit**.

주제 트리거 아래에서 구문을 선택하고 편집을 선택합니다.

5.  Paste the following **phrases**, and hit **enter**.

다음 구문을 붙여넣고 Enter를 누릅니다.

+----+----+------------------------------------------------------+----+
|    | ![ | order status                                         |    |
|    | Op |                                                      |    |
|    | en | track my order                                       |    |
|    | q  |                                                      |    |
|    | uo | where is my package                                  |    |
|    | ta |                                                      |    |
|    | ti | check order status                                   |    |
|    | on |                                                      |    |
|    | ma | has my order shipped                                 |    |
|    | rk |                                                      |    |
|    | ou | 주문 상태                                            |    |
|    | tl |                                                      |    |
|    | in | 내 주문 추적                                         |    |
|    | e] |                                                      |    |
|    | (. | 내 소포는 어디에 있나요?                             |    |
|    | /o |                                                      |    |
|    | ut | 주문 상태 확인                                       |    |
|    | pu |                                                      |    |
|    | t/ | 내 주문이 발송되었나요?                              |    |
|    | la |                                                      |    |
|    | b1 |                                                      |    |
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

6.  Select the **Details** button within the top right corner to open
    the **Topic details** pane.\
    This is where you can set a different **Display name** (what the
    end-user may see) from the configured topic **Name** (what the maker
    sees).

오른쪽 상단의 세부 사항 버튼을 선택하여 주제 세부 사항 창을 엽니다.

여기에서 구성된 주제 이름(작성자가 보는 것)과 다른 표시 이름(최종
사용자가 볼 수 있는 것)을 설정할 수 있습니다.

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   The Display name is used in case of disambiguation (for   |
| out  |     example, when multiple topics match a user utterance, the |
| line |     user is prompted to choose between two or three           |
| ](./ |     recognized topics, in a "Did you mean..." question.       |
| outp |                                                               |
| ut/l | -   When generative AI orchestration is used instead of the   |
| ab1. |     built-in natural language understanding for topic         |
| docx |     triggering, the display name is called the Model display  |
| /med |     name and is used in addition to the Model description as  |
| ia/i |     part of the intent detection process.                     |
| mage |                                                               |
| 4.sv | -   The Details pane is also where you can configure topic    |
| g){w |     input and output variables. This is useful when the topic |
| idth |     is invoked by another topic, or when generative AI        |
| ="0. |     orchestration is turned on, effectively using a large     |
| 4724 |     language model to slot fill the necessary variables and   |
| 4094 |     automatically prompting the user for missing inputs.      |
| 4881 |                                                               |
| 8897 | Pro tips:                                                     |
| 6in" |                                                               |
| hei  | 표시 이름: 중의성 발생 시 사용됩니다(예: 여러 주제가 사용자   |
| ght= | 발화와 일치할 때, \"다음 중 어느 것을 의미하셨나요\...\"      |
| "0.4 | 질문에서 두세 개의 인식된 주제 중 선택하도록 사용자에게       |
| 7244 | 요청).                                                        |
| 0944 |                                                               |
| 8818 | 생성 AI 오케스트레이션 사용 시: 주제 트리거를 위한 내장       |
| 8976 | 자연어 이해 대신 사용되며, 표시 이름은 모델 표시 이름으로     |
| in"} | 불리며, 모델 설명과 함께 의도 감지 과정의 일부로 사용됩니다.  |
|      |                                                               |
|      | 세부 사항 창: 주제 입력 및 출력 변수를 구성할 수 있는         |
|      | 곳입니다. 이는 다른 주제에서 주제를 호출할 때나 생성 AI       |
|      | 오케스트레이션이 켜져 있을 때 유용합니다. 이 경우 대형 언어   |
|      | 모델을 사용하여 필요한 변수를 슬롯 채우기하고, 사용자가       |
|      | 누락된 입력을 자동으로 요청합니다.                            |
+======+===============================================================+
+------+---------------------------------------------------------------+

7.  Select **Save**.\
    저장을 선택합니다.

### Task 2: Review the topic user interface 작업 2: 주제 사용자 인터페이스 검토

Now that you created your first topic, albeit without content except
trigger phrases, you can explore the authoring user interface (UI) to
become more familiar with it.

이제 첫 번째 주제를 만들었으므로(트리거 구문 외에는 콘텐츠 없음), 작성
사용자 인터페이스(UI)를 탐색하여 친숙해질 수 있습니다.\
\
![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image20.png){width="7.514583333333333in"
height="4.906944444444444in"}

1.  **Topic title** -- The name of the topic that you\'re currently
    editing, which is visible on the Topics page.

**주제 제목**: 현재 편집 중인 주제의 이름으로, 주제 페이지에 표시됩니다.

2.  **Productivity bar** -- Where you have access to tools, such as cut,
    copy, paste, and delete for the nodes (messages, questions, etc.).

**생산성 바**: 노드(메시지, 질문 등)를 위한 도구(잘라내기, 복사,
붙여넣기, 삭제 등)에 접근할 수 있는 곳입니다.

3.  **Copilot, Comments, Variables, Topic checker, Details, Analytics,
    Open code editor, and Reset to default buttons** -- This area
    includes: Copilot, which helps you create and update topics using
    descriptions in natural language; Comments, where authors can
    collaborate and leave comments on nodes; the Variables menu, to see
    the list of topic-level and global variables, and their runtime
    value in the test tab; Topic checker, which you can run anytime from
    the authoring canvas to check if errors have occurred in your topic
    that the platform can detect (and if left unresolved would prevent
    you from publishing the bot); the Details button to access the topic
    properties.

**코파일럿, 코멘트, 변수, 주제 검사기, 세부 사항, 분석, 코드 편집기 열기
및 기본값으로 재설정 버튼:** 이 영역에는 다음이 포함됩니다:

**코파일럿:** 자연어 설명을 사용하여 주제를 만들고 업데이트하는 데
도움이 됩니다.

**코멘트:** 작성자가 노드에 코멘트를 남기고 협력할 수 있는 곳입니다.

**변수 메뉴:** 주제 수준 및 전역 변수를 확인하고, 테스트 탭에서 실행 시
변수 값을 볼 수 있는 곳입니다.

**주제 검사기:** 언제든지 작성 캔버스에서 실행하여 플랫폼에서 감지할 수
있는 오류를 확인할 수 있습니다(해결되지 않으면 봇 게시를 방지).

**세부 사항 버튼:** 주제 속성에 접근할 수 있는 곳입니다.

4.  **... More** -- Analytics shows topic usage metrics; Open code
    editor switches the user interface from a no-code/low-code
    experience to a pro-code view of the underlying YAML configuration
    of the topic that developers can edit directly. For some system
    topics, a Reset to default option is available to revert the topic
    content to its original state.

**더 보기:**

**분석:** 주제 사용 메트릭을 보여줍니다.

**코드 편집기 열기:** 사용자 인터페이스를 코드 없는/저코드 환경에서
개발자가 직접 편집할 수 있는 기본 YAML 구성의 프로코드 보기로
전환합니다. 일부 시스템 주제의 경우, 기본값으로 재설정 옵션이 있어 주제
콘텐츠를 원래 상태로 되돌릴 수 있습니다.

5.  The **Save** button saves the topic changes.

**저장 버튼:** 주제 변경 사항을 저장합니다.

6.  The **Topic details** menu allows the maker to update the topic
    Name, Display name, Description and Status (active/inactive). When
    generative AI orchestration is enabled, display name is replaced
    with Model display name and Model description becomes available. It
    also allows the configuration of inputs and outputs. The inputs can
    be automatically slot filled when using generative AI as the
    orchestrator.

**주제 세부 사항 메뉴:** 작성자가 주제 이름, 표시 이름, 설명 및
상태(활성/비활성)를 업데이트할 수 있는 곳입니다. 생성 AI
오케스트레이션이 활성화된 경우, 표시 이름이 모델 표시 이름으로 대체되며
모델 설명이 추가로 사용 가능합니다. 입력과 출력을 구성할 수 있으며, 생성
AI를 오케스트레이터로 사용할 때 자동으로 슬롯을 채울 수 있습니다.

7.  The **trigger switcher** button is present at the Trigger node of
    every topic. By default, new topics have the Phrases trigger (or
    Triggered by copilot, when generative AI orchestration is enabled),
    but this can be switched to Message received, Event received,
    Activity received, Conversation update received, Invoke received,
    Redirect and Inactivity.

**트리거 전환 버튼:** 모든 주제의 트리거 노드에 있으며, 기본적으로
새로운 주제는 구문 트리거(또는 생성 AI 오케스트레이션이 활성화된 경우,
코파일럿에 의해 트리거됨)를 갖지만, 메시지 수신, 이벤트 수신, 활동 수신,
대화 업데이트 수신, 호출 수신, 리디렉션 및 비활동으로 전환할 수
있습니다.

8.  **Add a new node** -- the add a new node button allows the maker to
    add activities to a topic, such as send a message, ask a question,
    add a condition, etc., to build the dialog logic.

**새 노드 추가:** 새 노드 추가 버튼을 사용하여 주제에 활동을 추가할 수
있습니다. 예를 들어, 메시지 보내기, 질문하기, 조건 추가 등을 통해 대화
논리를 구축할 수 있습니다.

9.  **Authoring canvas controls** - You can use these controls to
    navigate the authoring canvas, which can become large for extensive
    topics. The included controls are a map of the canvas, zoom, hand,
    selection and reset.

**작성 캔버스 제어:** 작성 캔버스가 광범위한 주제에 대해 커질 수
있으므로 이 제어를 사용하여 탐색할 수 있습니다. 포함된 제어에는 캔버스
맵, 줌, 핸드, 선택 및 리셋이 있습니다.

### Task 3: Add content to your topic 작업 3: 주제에 콘텐츠 추가

This exercise doesn\'t cover how to add a large amount of content to
your topic; rather, it provides the steps to add a single question node,
message node, and topic redirection so that you can become familiar with
the overall process of creating a topic, testing, and publishing in
Microsoft Copilot Studio. The Publish demo exercise in this module
covers a more in-depth review of the authoring capabilities in Microsoft
Copilot Studio.

이 연습은 주제에 많은 양의 콘텐츠를 추가하는 방법을 다루지는 않습니다.
대신, 하나의 질문 노드, 메시지 노드 및 주제 리디렉션을 추가하는 단계를
제공하여 Microsoft Copilot Studio에서 주제를 생성하고 테스트하고
게시하는 전체 프로세스를 익힐 수 있습니다. 이 모듈의 게시 데모
연습에서는 Microsoft Copilot Studio의 작성 기능에 대해 더 깊이 있게
검토합니다.

The next section of this exercise covers foundational knowledge for
understanding the central components of Microsoft Copilot Studio and
creating topics.

이 연습의 다음 섹션에서는 Microsoft Copilot Studio의 핵심 구성 요소를
이해하고 주제를 만드는 데 필요한 기본 지식을 다룹니다.

#### Fundamental knowledge: Question node 기본 지식: 질문 노드

As a copilot author, you should use the Question node when you\'re
expecting a response from the user and you want to do something based on
that information. The user response is stored in a variable, and
question nodes can also use entities and slot filling features, both
concepts that are covered later in this exercise.

코파일럿 작성자로서 사용자의 응답을 기대하고 해당 정보에 기반하여 작업을
수행하려는 경우 질문 노드를 사용해야 합니다. 사용자 응답은 변수에
저장되며, 질문 노드는 엔터티와 슬롯 채우기 기능도 사용할 수 있습니다. 이
개념은 이 연습의 뒷부분에서 다룹니다.

The Question node uses many functions that a Message node does, such as
rich text, speech authoring, and rich text response types such images,
videos, and Adaptive Cards.

질문 노드는 메시지 노드가 하는 많은 기능을 사용합니다. 예를 들어 리치
텍스트, 음성 작성 및 이미지, 비디오, 적응형 카드와 같은 리치 텍스트 응답
유형을 사용할 수 있습니다.

1.  In the topic that you have open from the previous task, select the
    **+ button** below the existing node in the canvas and then select
    **Ask a question** to add a new Question node.

이전 작업에서 열어둔 주제에서 캔버스의 기존 노드 아래에 있는 + 버튼을
선택한 다음 질문하기를 선택하여 새로운 질문 노드를 추가합니다.

2.  Enter What would you like to do with your order? in the field and
    then make sure that the Identify value is set to **User\'s entire
    response**. This node is asking the question after the topic is
    triggered about what the user wants to do. The Publish demo exercise
    extends this task to using entities and slot filling.

\"주문과 관련하여 무엇을 하고 싶으신가요?\"를 입력하고 식별 값이
\"사용자의 전체 응답\"으로 설정되어 있는지 확인합니다. 이 노드는 주제가
트리거된 후 사용자가 무엇을 원하는지 묻는 질문을 합니다. 게시 데모
연습에서는 엔터티와 슬롯 채우기를 사용하는 작업을 확장합니다.

3.  By default, the user response is saved as a variable named **Var1**.
    You can **click on the variable name** to change its name, for
    example to OrderRequest.

기본적으로 사용자 응답은 Var1이라는 변수에 저장됩니다. 변수 이름을 예를
들어 OrderRequest로 변경하려면 변수 이름을 클릭할 수 있습니다.

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   It is a best practice to always properly name variables   |
| out  |     so they can be clearly identified when you reference them |
| line |     in your logic, and it also adds clarity when doing tests  |
| ](./ |     and checking the variable values at runtime.              |
| outp |                                                               |
| ut/l | -   Customers and partners can define and follow naming       |
| ab1. |     conventions for their variables, for consistency and ease |
| docx |     of maintenance.                                           |
| /med |                                                               |
| ia/i | Pro tips:                                                     |
| mage |                                                               |
| 4.sv | 변수를 항상 적절하게 이름을 지정하는 것이 모범 사례입니다.    |
| g){w | 이렇게 하면 논리에서 참조할 때 명확하게 식별할 수 있으며,     |
| idth | 테스트를 수행하고 실행 시 변수 값을 확인할 때 명확성을        |
| ="0. | 추가합니다. 고객 및 파트너는 일관성과 유지 관리 용이성을 위해 |
| 4724 | 변수의 명명 규칙을 정의하고 따를 수 있습니다.                 |
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

![Screens screenshot of a screenshot of a computer Description
automatically
generated](./output/lab1.docx/media/image21.png){width="5.789755030621173in"
height="5.384187445319335in"}

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   Question behavior can be customized by clicking on ...,   |
| out  |     Properties, and Question behavior. From here, you can     |
| line |     define if the question can be skipped, how many time it   |
| ](./ |     should be re-prompted to the user, validation rules, and  |
| outp |     what should happen if the user doesn't answer as          |
| ut/l |     expected.                                                 |
| ab1. |                                                               |
| docx | -   You can also define whether a user can jump to another    |
| /med |     topic without answering the question, and you can define  |
| ia/i |     the list of topics that are allowed in case of            |
| mage |     interruption.                                             |
| 4.sv |                                                               |
| g){w | -   It is a best practice to define retry prompts in case the |
| idth |     user doesn't understand what is expected from them the    |
| ="0. |     first time. It is then OK to be much more explicit with   |
| 4724 |     the user when trying to help them properly answer a       |
| 4094 |     question.                                                 |
| 4881 |                                                               |
| 8897 | Pro tips:                                                     |
| 6in" |                                                               |
| hei  | 질문 행동은 \... 속성 및 질문 행동을 클릭하여 사용자 정의할   |
| ght= | 수 있습니다. 여기서 질문을 건너뛸 수 있는지 여부, 사용자에게  |
| "0.4 | 다시 프롬프트할 횟수, 유효성 검사 규칙 및 사용자가 예상대로   |
| 7244 | 응답하지 않을 경우의 동작을 정의할 수 있습니다. 또한 사용자가 |
| 0944 | 질문에 응답하지 않고 다른 주제로 이동할 수 있는지 여부를      |
| 8818 | 정의할 수 있으며, 중단 시 허용되는 주제 목록을 정의할 수      |
| 8976 | 있습니다. 첫 번째로 사용자가 기대하는 것을 이해하지 못할      |
| in"} | 경우를 대비해 재프롬프트를 정의하는 것이 모범 사례입니다.     |
|      | 그런 다음 질문에 올바르게 응답할 수 있도록 사용자에게 훨씬 더 |
|      | 명확하게 설명하는 것이 좋습니다.                              |
+======+===============================================================+
+------+---------------------------------------------------------------+

#### Fundamental knowledge: Message node 기본 지식: 메시지 노드

You can use the Message node to display a message to the user. This
message can be simple based on the topic of the conversation. In direct
contrast to the Question node, the Message node doesn\'t expect or store
an answer from the user. The Message node also has rich text options
that you can display in text, or advanced options like cards, images,
videos, and Adaptive Cards.

메시지 노드는 사용자에게 메시지를 표시하는 데 사용할 수 있습니다. 이
메시지는 대화 주제에 따라 간단할 수 있습니다. 질문 노드와는 달리 메시지
노드는 사용자의 응답을 기대하거나 저장하지 않습니다. 메시지 노드에는
리치 텍스트 옵션도 있어 텍스트로 표시하거나 카드, 이미지, 비디오 및
적응형 카드와 같은 고급 옵션을 사용할 수 있습니다.

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   To make the copilot sound more natural and human, you can |
| out  |     configure message variations, so that the copilot will    |
| line |     send one of the configured messages, avoiding strict      |
| ](./ |     repletion of the same message.                            |
| outp |                                                               |
| ut/l | Pro tips:                                                     |
| ab1. |                                                               |
| docx | 코파일럿을 더 자연스럽고 인간적으로 들리게 하기 위해 메시지   |
| /med | 변형을 구성할 수 있습니다. 이렇게 하면 코파일럿이 동일한      |
| ia/i | 메시지를 반복하지 않고 구성된 메시지 중 하나를 보내게 됩니다. |
| mage |                                                               |
| 4.sv |                                                               |
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

You can also use variables within message nodes in the body of text
displayed to the user, which is dynamic based on the data stored within
them. This capability allows messages to be more personal, such as
"*Hello {System.User.FirstName}, I can get those order details for you,
one moment**"**.* Variables can also store data to perform automation or
calculations on them. Later exercises cover variables more in depth.
Last, you can also add Power Fx formulas to create even more dynamic
content.

메시지 노드 내에서 변수를 사용할 수 있어 사용자에게 표시되는 텍스트
본문이 저장된 데이터에 따라 동적일 수 있습니다. 이 기능을 통해 메시지를
더 개인화할 수 있습니다(예: \"안녕하세요 {System.User.FirstName}, 주문
세부 정보를 가져오겠습니다. 잠시만 기다려 주세요.\"). 변수는 데이터
자동화 또는 계산을 수행하는 데 사용할 수도 있습니다. 나중에 연습에서
변수를 더 깊이 다룹니다. 마지막으로 Power Fx 공식을 추가하여 더 동적인
콘텐츠를 만들 수 있습니다.

1.  To add another node, select the **+ button** below the Question
    node. Then, select **Send a message**. Enter a message that
    acknowledges the customer\'s question, such as Thank you for your
    question!

질문 노드 아래의 + 버튼을 선택하여 다른 노드를 추가합니다. 그런 다음
메시지 보내기를 선택합니다. 고객의 질문에 감사하는 메시지를
입력합니다(예: \"질문해 주셔서 감사합니다!\").**\
**

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image22.png){width="3.3464566929133857in"
height="4.937711067366579in"}

2.  End the conversation for the customer in this demo scenario. Select
    the **+ button** below the message node within the authoring canvas.
    Hover over the **Topic management** option, and then select **Go to
    another topic** and select **End of conversation**. This will
    redirect to a topic dedicated to ending a chat session, asking of
    the question has been answered and suggesting to fill a customer
    satisfaction survey.

이 데모 시나리오에서 고객의 대화를 종료합니다. 작성 캔버스 내의 메시지
노드 아래에서 + 버튼을 선택합니다. 주제 관리 옵션 위로 마우스를 가져간
다음 다른 주제로 이동을 선택하고 대화 종료를 선택합니다. 이는 대화
세션을 종료하는 전용 주제로 리디렉션되어 질문이 해결되었는지 확인하고
고객 만족도 설문조사를 작성하도록 제안합니다.\
\
![A screenshot of a chat Description automatically
generated](./output/lab1.docx/media/image23.png){width="3.3464566929133857in"
height="3.9254615048118984in"}

+------+---------------------------------------------------------------+
| ![Li | **Pro tip:** It is a best practice to end discrete dialog     |
| ghts | paths with the End of Conversation topic. That way, the       |
| On   | end-user can confirm their question was addressed. When a     |
| out  | user confirms, a customer satisfaction (CSAT) survey is       |
| line | displayed. Resolution rates and CSAT scores are both          |
| ](./ | displayed in the copilot analytics.                           |
| outp |                                                               |
| ut/l | Pro tip: 개별 대화 경로를 대화 종료 주제로 끝내는 것이 모범   |
| ab1. | 사례입니다. 이를 통해 최종 사용자는 질문이 해결되었는지       |
| docx | 확인할 수 있습니다. 사용자가 확인하면 고객 만족도(CSAT)       |
| /med | 설문조사가 표시됩니다. 해결률 및 CSAT 점수는 모두 코파일럿    |
| ia/i | 분석에 표시됩니다.                                            |
| mage |                                                               |
| 4.sv |                                                               |
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

3.  Then, within the top right hand corner of the screen, select the
    **Save** button.

그런 다음 화면 오른쪽 상단에서 저장 버튼을 선택합니다.

4.  Use the **Test** pane to validate that your bot behaves as
    expected.\
    Make sure you **Refresh** before doing a new test.

테스트 창을 사용하여 봇이 예상대로 작동하는지 확인합니다. 새로운
테스트를 하기 전에 새로고침을 꼭 하세요.

+----+----+------------------------------------------------------+----+
|    | ![ | I\'d like to check the status of my order please     |    |
|    | Op |                                                      |    |
|    | en | \"주문 상태를 확인하고 싶습니다\"                    |    |
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
|    | b1 |                                                      |    |
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

+------+---------------------------------------------------------------+
| ![Li | **Pro tip:** Trigger phrases don't need to be an exact match  |
| ghts | of all the utterances a user might say.                       |
| On   |                                                               |
| out  | Pro tip: 트리거 구문은 사용자가 말할 수 있는 모든 발화를      |
| line | 정확하게 일치시킬 필요는 없습니다.                            |
| ](./ |                                                               |
| outp |                                                               |
| ut/l |                                                               |
| ab1. |                                                               |
| docx |                                                               |
| /med |                                                               |
| ia/i |                                                               |
| mage |                                                               |
| 4.sv |                                                               |
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

### Task 4: Use Copilot to create a topic 작업 4: 코파일럿을 사용하여 주제 만들기

Creating topics in Microsoft Copilot Studio is more effortless than
before. Now, you can create a topic in Microsoft Copilot Studio by using
natural language to describe what you want the topic to do. With the
**Create from description with Copilot** feature, you can automatically
build a topic, reducing some manual steps that you experienced from the
first task in this unit. In this task, you\'ll learn how simple and
quick creating a topic with Copilot can be.

Microsoft Copilot Studio에서 주제를 만드는 작업이 이전보다 더
쉬워졌습니다. 이제 주제가 해야 할 일을 자연어로 설명하여 Microsoft
Copilot Studio에서 주제를 만들 수 있습니다. 설명으로부터 만들기 기능을
사용하여 수동 단계의 일부를 줄여 자동으로 주제를 생성할 수 있습니다. 이
작업에서는 Copilot을 사용하여 주제를 얼마나 간단하고 빠르게 만들 수
있는지 학습합니다.

1.  Select **Topics** from the navigation pane to the left of the
    screen.

화면 왼쪽의 탐색 창에서 주제를 선택합니다.

2.  Select the **+ Create** drop down and choose **Topic** and then
    **Create from description with Copilot**. A new window appears,
    asking you to **Name** your topic and enter a description in the
    **Create a topic to...** space.

만들기 드롭다운을 선택하고 주제를 선택한 다음 Copilot으로 설명에서
만들기를 선택합니다. 주제의 이름을 입력하고 설명을 입력하라는 새 창이
나타납니다.\
\
![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image24.png){width="5.708661417322834in"
height="1.7363057742782153in"}

3.  Enter Support Ticket in the **Name** your topic field.

주제 이름 필드에 \"지원 티켓\"을 입력합니다.

4.  In the **Create a topic to** space, enter the description of what
    your topic should do.

\"설명을 입력하세요\" 공간에 주제의 목적을 설명하는 내용을 입력합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Create a support ticket, including a title, severity |    |
|    | Op | (high / medium / low), description and an email      |    |
|    | en | address to send update notifications to. Define      |    |
|    | q  | variables following this naming pattern:             |    |
|    | uo | Topic.TicketTitle.                                   |    |
|    | ta |                                                      |    |
|    | ti | 지원 티켓을 생성합니다. 여기에는 제목,               |    |
|    | on | 심각도(높음/중간/낮음), 설명 및 업데이트 알림을 보낼 |    |
|    | ma | 이메일 주소가 포함됩니다. 이 명명 패턴을 따르는      |    |
|    | rk | 변수를 정의합니다: Topic.TicketTitle.                |    |
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
|    | b1 |                                                      |    |
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

5.  Select **Create**.

생성을 선택합니다.

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image25.png){width="6.653543307086614in"
height="3.6320516185476817in"}

> Copilot creates your topic, including the trigger phrases, question
> nodes, entity selection, variable naming, and message node
> confirmation.
>
> Copilot은 트리거 구문, 질문 노드, 엔터티 선택, 변수 이름 지정 및
> 메시지 노드 확인을 포함한 주제를 생성합니다.

6.  Select the **Copilot** button in the upper part of the authoring
    canvas (if the **Edit with Copilot** panel isn\'t open already).
    Within the **Edit with Copilot** panel, in the field **What do you
    want to do?** Add additional instructions and then, select
    **Update.**

작성 캔버스 상단의 Copilot 버튼을 선택합니다(이미 Copilot 패널이 열려
있지 않은 경우). Copilot 패널의 \"무엇을 하고 싶으신가요?\" 필드에 추가
지침을 입력한 다음 업데이트를 선택합니다.

+----+----+------------------------------------------------------+----+
|    | ![ | Before the last message, ask a question to find out  |    |
|    | Op | the user\'s preferred contact method, choosing from  |    |
|    | en | email, phone or SMS.                                 |    |
|    | q  |                                                      |    |
|    | uo | 마지막 메시지 전에 이메일, 전화 또는 SMS 중에서      |    |
|    | ta | 사용자가 선호하는 연락 방법을 묻는 질문을            |    |
|    | ti | 추가합니다.                                          |    |
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
|    | b1 |                                                      |    |
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

> ![A screenshot of a computer Description automatically
> generated](./output/lab1.docx/media/image26.png){width="4.330708661417323in"
> height="3.0432064741907263in"}
>
> Copilot automatically adds a question node, which both asks the
> customer for their contact method, and stores their choice in a
> variable.
>
> Copilot은 고객에게 연락 방법을 묻고 선택을 변수에 저장하는 질문 노드를
> 자동으로 추가합니다.
>
> ![A screenshot of a phone application Description automatically
> generated](./output/lab1.docx/media/image27.png){width="2.952755905511811in"
> height="4.6684317585301836in"}

+------+---------------------------------------------------------------+
| ![Li | Note: you can skip this step if you run into the below error: |
| ghts |                                                               |
| On   | 참고: 아래 오류가 발생하면 이 단계를 건너뛸 수 있습니다.      |
| out  |                                                               |
| line | ![](./out                                                     |
| ](./ | put/lab1.docx/media/image28.png){width="2.9163024934383204in" |
| outp | height="0.49993766404199474in"}                               |
| ut/l |                                                               |
| ab1. |                                                               |
| docx |                                                               |
| /med |                                                               |
| ia/i |                                                               |
| mage |                                                               |
| 4.sv |                                                               |
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

The Copilot feature in Microsoft Copilot Studio drastically reduces
authoring time, allowing you to create new topics and edit topics by
using natural language. Additionally, the **Edit with Copilot** panel
shows what updates have been created, and it provides suggestions for
what you can update in your topic.

Microsoft Copilot Studio의 Copilot 기능은 작성 시간을 대폭 단축하여
자연어를 사용해 새 주제를 만들고 편집할 수 있습니다. 또한 Copilot 패널은
생성된 업데이트를 보여주고 주제에서 업데이트할 수 있는 제안을
제공합니다.

7.  **Save** your new topic.

새 주제를 저장합니다.

8.  ![](./output/lab1.docx/media/image29.png){width="0.16875in"
    height="0.15694444444444444in"}Use the **Test pane** to validate
    that your bot behaves as expected.\
    Don't hesitate to use the refresh icon to start from a new
    conversation and not resume an old one.

테스트 창을 사용하여 봇이 예상대로 작동하는지 확인합니다. 새 대화를
시작하고 이전 대화를 다시 시작하지 않으려면 새로고침 아이콘을 사용하는
것을 주저하지 마세요.

+----+----+------------------------------------------------------+----+
|    | ![ | I have an issue with my laptop and need to log a     |    |
|    | Op | support ticket                                       |    |
|    | en |                                                      |    |
|    | q  | \"내 노트북에 문제가 있어 지원 티켓을 등록해야       |    |
|    | uo | 합니다\"                                             |    |
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
|    | b1 |                                                      |    |
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

## 연습 5: 테스트를 위해 데모 웹사이트에 코파일럿 게시하기 

### Task 1: Change your copilot authentication 작업 1: 코파일럿 인증 변경하기

이 데모의 목적을 위해 봇을 인증 없이 설정하여 데모 사이트 링크를 가진
모든 사람이 테스트할 수 있도록 합니다. 이를 위해 다음 단계를 따릅니다:

1.  Go to **Settings** in the top-right navigation

오른쪽 상단 탐색에서 설정으로 이동합니다.

2.  Go to **Security**

보안으로 이동합니다.

3.  Select **Authentication**

인증을 선택합니다.

4.  Select **No authentication** in the panel that opens and select
    **Save**

> 열리는 패널에서 인증 안 함을 선택하고 저장을 선택합니다.

5.  Select **Save** in the **Save this configuration?** Panel that opens

열리는 이 구성을 저장하시겠습니까? 패널에서 저장을 선택합니다.

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image30.png){width="4.502120516185477in"
height="2.108559711286089in"}

### Task 2: Publish your copilot 작업 2: 코파일럿 게시하기

Microsoft Copilot Studio provides a demo website so that you can invite
anyone to test your copilot by sending them the URL. This demo website
is useful for gathering feedback to improve your content before you
activate the copilot for your real end-users.

Microsoft Copilot Studio는 데모 웹사이트를 제공하므로 URL을 보내서
누구나 코파일럿을 테스트하도록 초대할 수 있습니다. 이 데모 웹사이트는
코파일럿을 실제 최종 사용자에게 활성화하기 전에 콘텐츠를 개선하기 위한
피드백을 수집하는 데 유용합니다.

1.  In Microsoft Copilot Studio, go to the **Channels** tab

Microsoft Copilot Studio에서 채널 탭으로 이동합니다.

2.  Select **Publish** to push the latest topics updates to the demo
    website. You\'ll need to complete this action before you use the
    demo website the first time and after you make changes to the topics
    that you want people to test on the demo website.

게시를 선택하여 최신 주제 업데이트를 데모 웹사이트에 푸시합니다. 데모
웹사이트를 처음 사용하기 전에 그리고 데모 웹사이트에서 사람들이
테스트하기를 원하는 주제에 변경 사항을 적용한 후 이 작업을 완료해야
합니다.

![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image31.png){width="6.692913385826771in"
height="3.1346073928258966in"}

+------+---------------------------------------------------------------+
| ![Li | **Pro tips:**                                                 |
| ghts |                                                               |
| On   | -   When you\'ve created your real copilot, you\'ll publish   |
| out  |     whenever you want to make updated topics available in     |
| line |     your deployed channels.                                   |
| ](./ |                                                               |
| outp | Pro tips:                                                     |
| ut/l |                                                               |
| ab1. | 실제 코파일럿을 만들었을 때 배포된 채널에서 업데이트된 주제를 |
| docx | 사용할 수 있도록 언제든지 게시할 수 있습니다.                 |
| /med |                                                               |
| ia/i |                                                               |
| mage |                                                               |
| 4.sv |                                                               |
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

-   The publishing process checks for errors in the topics whose Status
    is On.

-   Publication should take only a few minutes.

-   After you\'ve selected the Publish option, a green banner
    notification will show at the top of the screen when publishing is
    complete.

-   게시 프로세스는 상태가 켜짐인 주제의 오류를 확인합니다.

-   게시 선택 후 게시가 완료되면 화면 상단에 녹색 배너 알림이
    표시됩니다.

-   다음 스크린샷에 표시된 데모 웹사이트 링크를 선택합니다.

3.  Select the link for the **demo website**, as shown in the following
    screenshot.

다음 스크린샷에 표시된 데모 웹사이트 링크를 선택합니다.\
\
![A screenshot of a computer Description automatically
generated](./output/lab1.docx/media/image32.png){width="6.6929155730533685in"
height="3.134615048118985in"}

4.  When the demo site window opens, you can interact with the copilot
    by typing at the Type your message prompt or by selecting a starter
    phrase from the provided options.

데모 사이트 창이 열리면 메시지 입력 프롬프트에 입력하거나 제공된
옵션에서 시작 구문을 선택하여 코파일럿과 상호 작용할 수 있습니다.\
\
![A screenshot of a chatbot Description automatically
generated](./output/lab1.docx/media/image33.png){width="6.225893482064742in"
height="3.660971128608924in"}

Congratulations, you\'ve now built and published your first copilot!

축하합니다! 이제 첫 번째 코파일럿을 만들고 게시했습니다!

## 이용 약관

> 이 문서를 전부 또는 일부 사용하는 경우, 다음 약관에 동의하는 것으로
> 간주됩니다:
>
> **[Notice]{.underline} 공지**
>
> Information and views expressed in this document, including (without
> limitation) URL and other Internet Web site references, may change
> without notice. Examples depicted herein, if any, are provided for
> illustration only and are fictitious. No real association or
> connection is intended or should be inferred. This document does not
> provide you with any legal rights to any intellectual property in any
> Microsoft product.
>
> 이 문서에 표현된 정보와 견해(이를 포함하되 이에 국한되지 않는 URL 및
> 기타 인터넷 웹사이트 참조)는 사전 예고 없이 변경될 수 있습니다. 여기에
> 제시된 예시가 있다면, 이는 단지 설명을 위한 것이며 허구입니다. 실제
> 연관성이나 연결은 의도되지 않았으며, 추론해서도 안 됩니다. 이 문서는
> Microsoft 제품의 지적 재산권에 대한 법적 권리를 제공하지 않습니다.

### **[Use Limitations]{.underline} 사용 제한**

> Copying or reproduction, in whole or in part, of this document to any
> other server or location for further reproduction or redistribution is
> expressly prohibited. Microsoft provides you with this document for
> purposes of obtaining your suggestions, comments, input, ideas, or
> know-how, in any form, (\"Feedback\") and to provide you with a
> learning experience. You may use this document only to evaluate its
> content and provide feedback to Microsoft. You may not use this
> document for any other purpose. You may not modify, copy, distribute,
> transmit, display, perform, reproduce, publish, license, create
> derivative works from, transfer, or sell this document or any portion
> thereof. You may copy and use this document for your internal,
> reference purposes only.
>
> 이 문서를 다른 서버나 위치로 복제 또는 재배포하기 위해 전부 또는 일부
> 복사하는 것은 명시적으로 금지되어 있습니다. Microsoft는 이 문서를
> 귀하의 제안, 의견, 아이디어 또는 노하우(\"피드백\")를 얻기 위한
> 목적으로 제공하며 학습 경험을 제공하기 위한 것입니다. 이 문서를
> 평가하고 Microsoft에 피드백을 제공하는 목적 외에는 사용할 수 없습니다.
> 이 문서를 다른 목적으로 사용할 수 없습니다. 이 문서를 수정, 복사,
> 배포, 전송, 표시, 수행, 복제, 출판, 라이선스, 파생 작품 작성, 전송
> 또는 판매할 수 없습니다. 이 문서는 내부 참조 목적으로만 복사 및 사용할
> 수 있습니다.

### **[Feedback]{.underline}** 

> If you give Microsoft any Feedback about this document or the subject
> matter herein (including, without limitation, any technology,
> features, functionality, and/or concepts), you give to Microsoft,
> without charge, the right to use, share, and freely commercialize
> Feedback in any way and for any purpose. You also give third parties,
> without charge, the right to use, or interface with, any Microsoft
> products or services that include the Feedback. You represent and
> warrant that you own or otherwise control all rights to such Feedback
> and that no such Feedback is subject to any third-party rights.
>
> 귀하가 이 문서 또는 여기에 포함된 주제와 관련하여 Microsoft에 제공하는
> 피드백(기술, 기능, 기능 및/또는 개념 포함)에 대해 Microsoft는 무료로
> 해당 피드백을 어떠한 방식으로든 그리고 어떠한 목적으로든 사용, 공유 및
> 상업화할 수 있는 권리를 가집니다. 또한 제3자에게 무료로 해당 피드백이
> 포함된 Microsoft 제품 또는 서비스와 인터페이스할 수 있는 권리를
> 부여합니다. 귀하는 그러한 피드백에 대한 모든 권리를 소유하거나 달리
> 통제하며, 그러한 피드백이 제3자의 권리에 속하지 않는다는 것을 진술하고
> 보증합니다.

### **[DISCLAIMERS]{.underline} 면책 조항**

> CERTAIN SOFTWARE, TECHNOLOGY, PRODUCTS, FEATURES, AND FUNCTIONALITY
> (COLLECTIVELY \"CONCEPTS\"),
>
> INCLUDING POTENTIAL NEW CONCEPTS, REFERENCED IN THIS DOCUMENT ARE IN A
> SIMULATED ENVIRONMENT
>
> WITHOUT COMPLEX SET-UP OR INSTALLATION AND ARE INTENDED FOR FEEDBACK
> AND TRAINING PURPOSES
>
> ONLY. THE CONCEPTS REPRESENTED IN THIS DOCUMENT MAY NOT REPRESENT FULL
> FEATURE CONCEPTS AND MAY
>
> NOT WORK THE WAY A FINAL VERSION MAY WORK. MICROSOFT ALSO MAY NOT
> RELEASE A FINAL VERSION OF SUCH
>
> CONCEPTS. YOUR EXPERIENCE WITH USING SUCH CONCEPTS IN A PHYSICAL
> ENVIRONMENT MAY ALSO BE DIFFERENT.
>
> THIS DOCUMENT, AND THE CONCEPTS AND TRAINING PROVIDED HEREIN, IS
> PROVIDED "AS IS", WITHOUT WARRANTY
>
> OF ANY KIND, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING
> (WITHOUT LIMITATION) THE WARRANTIES OF
>
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, AND
> NONINFRINGEMENT. MICROSOFT DOES NOT
>
> MAKE ANY ASSURANCES OR REPRESENTATIONS WITH REGARD TO THE ACCURACY OF
> THE RESULTS, THE OUTPUT THAT DERIVES FROM USE OF THIS DOCUMENT OR THE
> CONCEPTS, OR THE SUITABILITY OF THE CONCEPTS OR INFORMATION CONTAINED
> IN THIS DOCUMENT FOR ANY PURPOSE.
>
> MICROSOFT COPILOT STUDIO (1) IS NOT INTENDED OR MADE AVAILABLE AS A
> MEDICAL DEVICE FOR THE
>
> DIAGNOSIS OF DISEASE OR OTHER CONDITIONS, OR IN THE CURE, MITIGATION,
> TREATMENT OR PREVENTION OF
>
> DISEASE, OR OTHERWISE TO BE USED AS A COMPONENT OF ANY CLINICAL
> OFFERING OR PRODUCT, AND NO LICENSE
>
> OR RIGHT IS GRANTED TO USE MICROSOFT COPILOT STUDIO FOR SUCH PURPOSES,
> (2) IS NOT DESIGNED OR
>
> INTENDED TO BE A SUBSTITUTE FOR PROFESSIONAL MEDICAL ADVICE,
> DIAGNOSIS, TREATMENT, OR JUDGMENT AND SHOULD NOT BE USED AS A
> SUBSTITUTE FOR, OR TO REPLACE, PROFESSIONAL MEDICAL ADVICE, DIAGNOSIS,
>
> TREATMENT, OR JUDGMENT, AND (3) SHOULD NOT BE USED FOR EMERGENCIES AND
> DOES NOT SUPPORT EMERGENCY
>
> CALLS. ANY CHATBOT YOU CREATE USING MICROSOFT COPILOT STUDIO IS YOUR
> OWN PRODUCT OR SERVICE,
>
> SEPARATE AND APART FROM MICROSOFT COPILOT STUDIO. YOU ARE SOLELY
> RESPONSIBLE FOR THE DESIGN,
>
> DEVELOPMENT, AND IMPLEMENTATION OF YOUR CHATBOT (INCLUDING
> INCORPORATION OF IT INTO ANY PRODUCT
>
> OR SERVICE INTENDED FOR MEDICAL OR CLINICAL USE) AND FOR EXPLICITLY
> PROVIDING END USERS WITH
>
> APPROPRIATE WARNINGS AND DISCLAIMERS PERTAINING TO USE OF YOUR
> CHATBOT. YOU ARE SOLELY RESPONSIBLE
>
> FOR ANY PERSONAL INJURY OR DEATH THAT MAY OCCUR AS A RESULT OF YOUR
> CHATBOT OR YOUR USE OF
>
> MICROSOFT COPILOT STUDIO IN CONNECTION WITH YOUR CHATBOT, INCLUDING
> (WITHOUT LIMITATION) ANY SUCH INJURIES TO END USERS.

이 문서에서 참조된 특정 소프트웨어, 기술, 제품, 기능 및 기능(총칭하여
\"개념\")은 복잡한 설정 또는 설치 없이 시뮬레이션된 환경에서 제공되며
피드백 및 교육 목적으로만 사용됩니다. 이 문서에 제시된 개념은 완전한
기능의 개념을 나타내지 않을 수 있으며, 최종 버전이 작동하는 방식과 다를
수 있습니다. 또한 Microsoft는 이러한 개념의 최종 버전을 출시하지 않을 수
있습니다. 실제 환경에서 이러한 개념을 사용할 때의 경험도 다를 수
있습니다. 이 문서와 이 문서에서 제공되는 개념 및 교육은 명시적이든
묵시적이든 또는 법적이든 상관없이 상품성, 특정 목적에 대한 적합성,
소유권 및 비침해에 대한 보증을 포함하여 어떠한 종류의 보증 없이 \"있는
그대로\" 제공됩니다. Microsoft는 이 문서 또는 개념을 사용한 결과,
출력물의 정확성 또는 이 문서에 포함된 개념이나 정보의 적합성에 대해
어떠한 보증이나 진술도 하지 않습니다.

Microsoft Copilot Studio는 (1) 질병 또는 기타 상태의 진단, 치료, 경감,
치료 또는 예방을 위한 의료 기기로 의도되거나 제공되지 않으며, 임상 제공
또는 제품의 구성 요소로 사용될 수 없으며, 그러한 용도로 Microsoft
Copilot Studio를 사용할 수 있는 라이선스 또는 권리를 부여하지 않습니다.
(2) 전문적인 의료 조언, 진단, 치료 또는 판단을 대체할 의도로 설계되거나
제공되지 않으며, 전문적인 의료 조언, 진단, 치료 또는 판단을 대체하거나
이를 대신하여 사용해서는 안 됩니다. (3) 긴급 상황에 사용되어서는 안
되며, 긴급 호출을 지원하지 않습니다. Microsoft Copilot Studio를 사용하여
만든 모든 챗봇은 Microsoft Copilot Studio와 별개이며 독립적인 귀하의
제품 또는 서비스입니다. 귀하는 챗봇의 설계, 개발 및 구현(이를 의료 또는
임상 용도로 사용하려는 제품 또는 서비스에 통합하는 경우 포함)에 전적으로
책임이 있으며, 최종 사용자에게 챗봇 사용과 관련된 적절한 경고와 면책
조항을 명시적으로 제공할 책임이 있습니다. 귀하의 챗봇 또는 Microsoft
Copilot Studio와 관련하여 귀하의 챗봇 사용으로 인해 발생할 수 있는 모든
개인 상해 또는 사망에 대한 책임은 전적으로 귀하에게 있습니다.
