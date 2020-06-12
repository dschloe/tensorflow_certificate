## From rules to data

In these videos you were given an introduction to the concepts and paradigms of Machine Learning and Deep Learning. You saw that the traditional paradigm of expressing rules in a coding language may not always work to solve a problem. As such, scenarios such as Computer Vision are very difficult to solve with rules-based programming. Instead, if we feed a computer with enough data that we describe (or label) as what we want it to recognize, given that computers are really good at processing data and finding patterns that match, then we could potentially ‘train’ a system to solve a problem. We saw a super simple example of that -- fitting numbers to a line. So now let’s go through a notebook and execute the code that trains a neural network to learn how a set of numbers we give it make up a line, so it can then extend the line if we need to.

## Try it for yourself

Ok, now that you’ve seen me do it, why don’t you give it a try for yourself. You can download the workbook [here](https://github.com/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%202%20-%20Lesson%202%20-%20Notebook.ipynb) if you want to try it out for yourself. Or, if you prefer, you can execute it right now in Google Colaboratory [at this link](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%202%20-%20Lesson%202%20-%20Notebook.ipynb).

Now while this might seem very simple, you’ve actually gotten the basics for how neural networks work. As your applications get more complex, you’ll continue to use the same techniques. For now, let’s do a quick test with Multiple Choice Questions to see what you’ve learned.

## Quiz
1. The diagram for traditional programming had Rules and Data In, but what came out?

- [x] Answers
- [ ] Binary
- [ ] Bugs
- [ ] Machine Learning

2. The diagram for Machine Learning had Answers and Data In, but what came out?

- [ ] Binary
- [x] Rules
- [ ] Bugs
- [ ] Models

3. When I tell a computer what the data represents (i.e. this data is for walking, this data is for running), what is that process called?

- [ ] Programming the Data
- [ ] Learning the Data
- [ ] Categorizing the Data
- [x] Labelling the Data

4. What is a Dense?

- [ ] Mass over Volume
- [x] A layer of connected neurons
- [ ] A single neuron
- [ ] A layer of disconnected neurons

5. What does a Loss function do?

- [ ] Figures out if you win or lose
- [ ] Decides to stop training a neural network
- [x] Measures how good the current ‘guess’ is
- [ ] Generates a guess

6. What does the optimizer do?
- [ ] Decides to stop training a neural network
- [ ] Measures how good the current guess is
- [x] Generates a new and improved guess
- [ ] Figures out how to efficiently compile your code

7. What is Convergence?
- [ ] The bad guys in the next ‘Star Wars’ movie
- [x] The process of getting very close to the correct answer
- [ ] A dramatic increase in loss
- [ ] A programming API for AI

8. What does model.fit do?
- [ ] It determines if your activity is good for your body
- [x] It trains the neural network to fit one set of values to another
- [ ] It optimizes an existing model
- [ ] It makes a model fit available memory

## Colaboratory 자주 묻는 질문(FAQ)

### 기본 사항
Colaboratory란 무엇인가요?
줄여서 'Colab'이라고도 하는 Colaboratory는 Google 리서치팀에서 개발한 제품입니다. Colab을 사용하면 누구나 브라우저를 통해 임의의 Python 코드를 작성하고 실행할 수 있습니다. Colab은 특히 머신러닝, 데이터 분석 및 교육에 적합합니다. 더욱 기술적으로 설명하면, Colab은 설정 없이도 사용 가능한 호스팅 Jupyter 메모장 서비스로, GPU를 포함한 컴퓨팅 리소스를 무료로 제공합니다.

정말 무료로 사용할 수 있나요?
예. Colab은 무료로 제공됩니다.

믿기 어려울 정도로 좋아 보이는데요. 어떤 제한사항이 있나요?
Colab 리소스는 보장되거나 무제한이 아니며 사용량 한도가 변동되는 경우가 있습니다. 이러한 방식은 Colab에서 리소스를 무료로 제공하기 위해 필요합니다. 자세한 내용은 리소스 한도를 참조하세요.

향상된 리소스를 더 안정적으로 사용하는 데 관심이 있다면 Colab Pro가 적합할 수 있습니다.

Jupyter와 Colab 사이에는 어떤 차이점이 있나요?
Jupyter는 Colab이 기반을 둔 오픈소스 프로젝트입니다. Colab을 사용하면 아무것도 다운로드하거나 설치, 실행하지 않고도 Jupyter 메모장을 다른 사람과 공유할 수 있습니다.

Colab 사용하기
메모장은 어디에 저장되나요? 저장한 메모장을 공유할 수 있나요?
Colab 메모장은 Google 드라이브에 저장되거나 GitHub에서 로드할 수 있습니다. 또한 Colab 메모장은 Google 문서 또는 스프레드시트와 마찬가지로 공유할 수 있습니다. Colab 메모장 오른쪽 상단에서 공유 버튼을 클릭하거나 Google 드라이브의 파일 공유 안내를 따르세요.

메모장을 공유하면 무엇이 공유되나요?
메모장을 공유하면 텍스트, 코드, 출력, 댓글 등 메모장의 모든 내용이 공유됩니다. 메모장을 저장할 때 수정 > 노트북 설정 > 이 메모장을 저장할 때 코드 셀 출력 생략을 선택하면 코드 셀 출력이 저장되거나 공유되지 않습니다. 설정한 모든 맞춤설정 파일 및 라이브러리를 비롯해 사용 중인 가상 머신은 공유되지 않습니다. 그러므로 메모장에 필요한 맞춤설정 라이브러리 또는 파일을 설치하고 로드하는 셀을 포함하는 것이 좋습니다.

기존의 Jupyter/IPython 메모장을 Colab으로 가져올 수 있나요?
예. 파일 메뉴에서 '메모장 업로드'를 선택하세요.

Colab 메모장을 검색하려면 어떻게 해야 하나요?
Google 드라이브로 Colab 메모장을 검색할 수 있습니다. 메모장 뷰 왼쪽 상단에 있는 Colab 로고를 클릭하면 드라이브에 저장된 메모장이 모두 표시됩니다. 파일 > 최근 메모장 열기를 사용하면 최근에 열었던 메모장을 검색할 수 있습니다.

코드는 어디에서 실행되나요? 브라우저 창을 닫으면 실행 상태는 어떻게 되나요?
코드는 계정 전용 가상 머신에서 실행됩니다. 한동안 유휴 상태이면 가상 머신은 삭제되고 Colab 서비스에서 설정된 최대 수명이 적용됩니다.

데이터를 다운로드하려면 어떻게 해야 하나요?
이 안내에 따라 내가 작성한 Colab 메모장을 Google 드라이브에서 다운로드하거나, Colab의 파일 메뉴에서 다운로드할 수 있습니다. 모든 Colab 메모장은 오픈소스 Jupyter 메모장 형식(.ipynb)으로 저장됩니다.

코드가 실행되는 가상 머신을 초기화하려면 어떻게 해야 하나요? 간혹 초기화가 불가능한 이유는 무엇인가요?
런타임 > 런타임 초기화를 선택하면 나에게 할당된 모든 관리형 가상 머신이 원래 상태로 되돌아갑니다. 초기화는 시스템 파일을 실수로 덮어썼거나 호환되지 않는 소프트웨어를 설치하여 가상 시스템이 비정상 상태가 된 경우 도움이 됩니다. Colab에서는 과도한 리소스 소모를 방지하기 위해 이 작업을 실행할 수 있는 빈도를 제한합니다. 초기화에 실패했다면 나중에 다시 시도해 보세요.

간혹 drive.mount()가 실패하면서 '시간 초과' 메시지가 표시되는 이유와 drive.mount()로 마운트된 폴더에서 I/O 작업이 실패하는 이유는 무엇인가요?
폴더에 파일 또는 하위 폴더가 너무 많은 경우 Google 드라이브 작업이 시간 초과될 수 있습니다. 수천 개의 항목이 최상위 수준의 '내 드라이브' 폴더에 직접 포함되어 있는 경우 드라이브를 마운트하면 시간 초과가 발생할 수 있습니다. 시간 초과되기 이전에 실패한 시도의 상태가 로컬에 부분적으로 캐시되므로 반복해서 시도하면 성공할 수도 있습니다. 이 문제가 발생할 경우 '내 드라이브'에 직접 포함된 파일 및 폴더를 하위 폴더로 이동해 보세요. drive.mount()가 성공한 후에 다른 폴더의 항목을 읽으면 비슷한 문제가 발생할 수 있습니다. 많은 항목이 포함된 폴더의 항목에 액세스하면 OSError: [Errno 5] Input/output error(python 3) 또는 IOError: [Errno 5] Input/output error(python 2) 같은 오류가 발생할 수 있습니다. 직접 포함된 항목을 하위 폴더로 이동하면 이 문제를 해결할 수 있습니다.
파일 또는 하위 폴더를 휴지통으로 이동하여 '삭제'하는 것으로는 충분하지 않을 수 있습니다. 이 경우 휴지통을 비워야 합니다.

리소스 한도
Colab에서 리소스가 보장되지 않는 이유는 무엇인가요?
컴퓨팅 리소스를 무료로 제공하려면 Colab에서는 사용량 한도와 하드웨어 가용성을 필요에 따라 유연하게 조정할 수 있어야 합니다. Colab에서 제공되는 리소스는 수요의 변동, 전반적인 성장 등의 요인에 대응할 수 있도록 시간에 따라 달라집니다.

Colab에서 허용하는 리소스 한도를 넘어 더 많은 작업을 실행하고자 하는 경우도 있을 수 있습니다. 실제로 많은 사용자가 Google에 GPU 속도 및 메모장 실행 시간 개선, 메모리 용량 확대를 비롯해 사용량 한도를 높이고 변동을 줄일 것을 요청해 왔습니다. 이처럼 Colab으로 더 많은 작업을 하고자 하는 사용자를 위해 Google에서 선보이는 새로운 버전이 바로 Colab Pro입니다. 사용자의 요구사항을 충족하기 위해 지속 가능한 방식으로 성장하는 동시에 Colab 무료 버전을 계속 제공하는 것이 장기적인 목표입니다. Colab 무료 버전에서 허용하는 리소스 한도 이상으로 Colab을 활용하는 데 관심이 있다면 Colab Pro를 사용해 보고 의견을 들려주세요.

Colab의 사용량 한도란 무엇인가요?
Colab에서는 보장된 리소스 또는 무제한 리소스를 제공하는 대신 경우에 따라 사용량 한도를 동적으로 변경함으로써 무료 리소스를 제공할 수 있습니다. 즉, 전체 사용량 한도, 유휴 시간 제한 기간, 최대 VM 수명, 사용 가능한 GPU 유형 등의 요소가 시간에 따라 달라집니다. Colab은 이러한 한도를 공개하지 않는데, 그 이유 중 하나는 한도가 빠르게 바뀔 수 있으며 실제로도 빠르게 바뀌는 경우가 있기 때문입니다.

장기간 연산을 실행하기보다는 Colab을 대화식으로 사용하거나 또는 최근에 Colab 리소스 사용량이 비교적 적었던 사용자에게 GPU 및 TPU가 우선적으로 할당되는 경우도 있습니다. 이로 인해 Colab을 장기적으로 실행되는 연산에 사용하거나 최근에 Colab에서 리소스 사용량이 비교적 많았던 사용자는 사용량 한도에 도달하여 GPU 및 TPU 액세스가 일시적으로 제한될 가능성이 높습니다. 많은 연산이 필요한 사용자는 Colab UI를 자체 하드웨어에서 실행하는 로컬 런타임으로 사용하는 것이 적합할 수 있습니다. 더 높으면서 안정적인 사용량 한도에 관심이 있다면 Colab Pro가 적합할 수 있습니다.

Colab에서 사용할 수 있는 GPU 유형은 무엇인가요?
Colab에서 사용할 수 있는 GPU 유형은 시간에 따라 달라집니다. 이러한 방식은 Colab에서 리소스를 무료로 제공하기 위해 필요합니다. Colab에서 사용할 수 있는 GPU로는 보통 Nvidia K80, T4, P4, P100이 있습니다. 특정 시점에 Colab에서 연결할 수 있는 GPU 유형을 선택할 수는 없습니다. Colab에서 가장 빠른 GPU에 더욱 안정적으로 액세스하는 데 관심이 있다면 Colab Pro가 적합할 수 있습니다.

Colab을 암호화폐 채굴에 사용하는 것은 전면 금지되어 있으며 사용할 경우 Colab을 사용할 수 없도록 계정이 완전히 제한될 수 있습니다.

Colab에서 메모장을 얼마나 오래 실행할 수 있나요?
메모장은 최대 수명이 12시간인 가상 머신에 연결되어 실행됩니다. 유휴 상태가 너무 오래 지속되면 메모장의 VM 연결이 해제됩니다. 최대 VM 수명 및 유휴 시간 제한 동작은 시간 또는 사용량에 따라 달라질 수 있습니다. 이러한 방식은 Colab에서 컴퓨팅 리소스를 무료로 제공하기 위해 필요합니다. 시간에 따라 크게 달라지지 않는 더 긴 VM 수명이나 더 관대한 유휴 시간 제한 동작에 관심이 있다면 Colab Pro가 적합할 수 있습니다.

Colab에서는 메모리를 얼마나 사용할 수 있나요?
Colab 가상 머신에서 사용할 수 있는 메모리 양은 시간에 따라 달라집니다(VM 수명 내에는 안정적임). 시간에 따라 메모리를 조정하므로 Colab을 계속 무료로 제공할 수 있습니다. Colab에서 추가 메모리가 필요하다고 판단되면 메모리가 더 많은 VM에 자동으로 할당될 수도 있습니다. Colab에서 더 많은 메모리를 더 안정적으로 사용하는 데 관심이 있다면 Colab Pro가 적합할 수 있습니다.

Colab을 최대한 활용하려면 어떻게 해야 하나요?
한정된 리소스를 소수의 사용자가 독점하지 않도록 하기 위해 Colab의 리소스는 최근에 리소스를 상대적으로 적게 사용한 사용자에게 우선으로 할당됩니다. Colab을 최대한 활용하려면 작업이 끝난 후 Colab 탭을 닫고, 작업에 필요하지 않은 GPU를 선택하지 않는 것이 좋습니다. 이렇게 하면 Colab 사용 중에 사용량 한도에 걸릴 가능성이 낮아집니다. Colab 무료 버전의 리소스 한도 이상을 사용하는 데 관심이 있다면 Colab Pro가 적합할 수 있습니다.

GPU가 활용되지 않고 있다는 메시지가 표시됩니다. 어떻게 해야 하나요?
Colab에서는 GPU와 TPU를 포함한 가속 컴퓨팅 환경을 선택사항으로 제공합니다. GPU 또는 TPU 런타임에서 코드를 실행한다고 해서 반드시 GPU 또는 TPU가 활용되는 것은 아닙니다. GPU 사용 한도에 도달하지 않도록 GPU를 활용하지 않는 경우 표준 런타임으로 전환하는 것이 좋습니다. 런타임 > 런타임 유형 변경을 선택하고 하드웨어 가속기를 없음으로 설정하세요.

Colab에서 GPU 및 TPU 런타임을 활용하는 방법의 예를 보려면 Tensorflow With GPU와 TPUs In Colab 예시 메모장을 참조하세요.

추가 질문
어떤 브라우저가 지원되나요?
Colab은 대부분의 주요 브라우저와 호환되며, 특히 Chrome, Firefox, Safari의 최신 버전을 대상으로 가장 철저하게 테스트되었습니다.

colaboratory.jupyter.org와는 어떤 관련이 있나요?
2014년에 Google에서는 Jupyter 개발팀과 함께 Colab의 초기 버전을 공개했습니다. 그 이후 Colab은 Google 내부에서 사용되면서 꾸준히 발전해 왔습니다.

다른 프로그래밍 언어도 사용할 수 있나요?
Colab은 Python과 타사 도구로 이루어진 Python 생태계를 지원하는 데 초점을 두고 있습니다. 한편 Google에서는 사용자가 R 또는 Scala 등의 다른 Jupyter 커널 지원을 바란다는 점 또한 인지하고 있습니다. 이러한 커널을 지원할 의향은 있지만, 아직 확실한 계획은 없습니다.

버그를 발견했거나 질문이 있으면 누구에게 문의해야 하나요?
Colab 메모장을 연 다음 도움말 메뉴로 이동하여 '의견 보내기...'를 선택하세요.

타사 쿠키를 허용하라는 메시지가 표시되는 이유는 무엇인가요?
Colab은 풍부한 출력 결과를 안전하게 표시하기 위해 HTML iframe과 별도의 출처에서 호스팅되는 서비스 워커를 사용합니다. 브라우저에서 iframe 내의 서비스 워커를 사용하려면 타사 쿠키를 허용해야 합니다. 모든 사이트의 타사 쿠키를 허용하는 대신 브라우저 설정에서 호스트 이름 googleusercontent.com을 허용 목록에 등록해도 됩니다.

편집기 글꼴을 변경하려면 어떻게 해야 하나요?
Colab에서는 편집기에 일반 고정 너비 글꼴을 사용합니다. 현재 사용되는 대부분의 브라우저에서 고정 너비로 사용할 글꼴 모음을 구성할 수 있습니다. 일반적인 구성 방법은 다음과 같습니다.

Firefox의 경우 Firefox 지원 문서에 나와 있는 단계에 따라 '고정 너비' 글꼴을 구성합니다.
Chrome의 경우 'chrome://settings/fonts'로 이동하여 '고정폭 글꼴' 라벨이 있는 섹션을 수정합니다.
Colab에서 Python 2가 지원 종료되는 시점은 언제인가요?
Python 개발팀에서는 2020년 1월 1일 이후부터 Python 2를 더 이상 지원하지 않을 예정이라고 발표했습니다. 이 날짜부터 Colab에서는 Python 2 런타임 업데이트를 중단했으며 앞으로 몇 개월간 Python 2 지원을 점진적으로 중단할 예정입니다.

따라서 사용자는 당분간 Python 2 메모장을 계속 사용할 수 있습니다. 하지만 특정 시점부터는 Python 2 메모장이 Python 3 런타임으로 대신 연결되기 시작할 수 있습니다. 예상치 못한 문제를 방지하려면 중요한 메모장을 Python 3로 이전하는 것이 좋습니다.

메모장의 런타임을 변경하려면 런타임 > 런타임 유형 변경을 선택한 다음 Python 3를 선택하세요. Python 2에서 Python 3로 코드를 이전하는 방법을 알아보려면 Python 설명서에서 Python 2 코드를 Python 3로 포팅하기를 참고하시기 바랍니다.

Colab Pro에 관해 자세히 알아보려면 어떻게 해야 하나요?
Colab Pro 가입 페이지에서 Colab Pro 관련 FAQ를 확인하세요.
