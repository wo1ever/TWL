20180703 Tue 수업 w/애란선생님
===========================

파이썬 기초 1 (오전)
----------------



### 0. 수업 전 공지사항 & 과제 점검 

- "수업 시작 10분 전에 와서 팀별로 회고합시다."
- 각 조에서 하나씩 스크래치로 만든 코드와 결과물 공유/발표
- 어제 수업 설문에 대한 피드백
  - 직관이 아니라 데이터, 데이터가 아니라 직관 등의 이분법적인 구분은 지양해야. 조화를 이루도록 한다.

  - 린(lean)과 애자일(agile)은 일본 도요타 방식의 영향을 받았기 때문에 비슷하다. 다품종 소량생산의 방식을 택하고, 수요가 바뀔 때 그러한 흐름에 기민하게 대응하는 방법. 즉, 뿌리가 같기 때문에 비슷함. 

    

### 1. 수업의 목표

- 파이썬 소개

- 기본 문법과 개념 익히기

- 파이썬 프로그래밍 환경 Colab 익히기

   
#### 1.1. 파이썬 소개

- 파이썬은 1991년에 Guido van Rossum 이 개발한 프로그래밍 언어의 한 종류이다. 주로 쓰이는 분야는 데이터 분석, 과학 계산, 웹 프로그래밍 등이다. 간혹 게임 서버 쪽에서도 사용된다. 범용 언어라 어디에서든 쓰일 수 있긴 하지만, 언어별로 약간씩 특성이 다르기 때문에 특정 분야에서 선호되는 경향들은 존재한다. 

  - 위키의 List of programming languages 에 나오는 프로그래밍 언어의 리스트에서, 컴퓨터가 읽을 수 있도록 코드를 짜서 개별 이름들을 데이터로 뽑아낼 수 있다. 
  - 예시는 selector 문법으로, HTML 문서에서 원하는 부분만 뽑아내는 문법이다. 파이썬에서도 활용할 수 있다. 

  

- **파이썬의 장점** 

  - 데이터를 분석한 결과를 웹사이트와 연동하는 것이 우리가 가장 자주 하게 될 일이다. 웹을 만들지 않고, 앱을 만든다 하더라도 앱이 데이터를 가져오는 곳은 주로 웹이다. 보통은 데이터를 가공한 다음 웹을 통해서 그 데이터를 제공하고, 그것이 웹 혹은 앱으로 출력된다. 파이썬을 배우면 데이터 수집, 분석, 실제 웹 서비스에 적용하기까지의 과정을 한 언어에 끝낼 수 있다. 

- 프로그래밍 언어론적 측면에서 제법 괜찮은 문법, 제법 괜찮은 성능. 

- 질문1: 괜찮은 문법, 괜찮은 성능이라고 얘기할 때의 기준? 

애란선생님이 언어를 평가 할 때의 기준 두 가지는, 첫번째는 언어의 문법을 설명하기 위해 작성해야 하는 매뉴얼이 짧을 수록 좋은 언어. 즉, 문법에 대한 설명이 간결하면 간결할 수록 괜찮은 언어. 파이썬은 그럭저럭 짧은 편이다. 이를테면, io라는 언어는 그런 면에서는 괜찮은 편. 문법이 워낙 간소하기 때문에 아주 기본적인 개념을 만들려고 할 때 여러가지를 조합해야 한다는 단점이 있다. basic/visual basic같은 경우는 그런 면에서 비효율적. 두번 째는, 인간이 쓰고 익히기에 얼마나 직관적인가. 파이썬은 이 두 가지를 그럭저럭 균형을 맞추고 있다. 

파이썬에서 쓰는 대부분의 패키지들은 C언어로 개발된 다음 파이썬으로 포장된 것이다. 그래서 C의 성능을 가지고 있는 경우가 대부분. C언어와 파이썬 자체만 놓고 보았을 때는 파이썬의 성능이 떨어질 수 있지만, 우리가 사용하는 패키지들에서는 문제가 되지 않는다. 

  - 다양한 패러다임을 지원한다. 예를 들어, 1부터 10까지 더하는 서로 다른 방식들을 전부 지원한다. 

- 질문2: 다양한 패러다임이란 무엇인가요?

어제 실습했듯 동일한 결과물을 표현하기 위한 알고리즘은 여러 가지가 있다. 이러한 측면에서 파이썬은 여러가지 방법들, 여러 알고리즘을 전반적으로 잘 표현해낼 수 있는 언어이다. 

- 질문3: 컴퓨터랑 가깝지 않은데 사람들이 왜 많이 쓰나요?

컴퓨터와 가깝지 않다는 건 사람과 가깝다는 뜻이다. 즉, 컴퓨터의 사고 방식과 가깝다는 뜻이다. 컴퓨터를 극도로 활용하여 성능이 빨라질 수는 있지만 인간이 사고하는 방식과는 거리가 멀어서 익숙해지느 ㄴ데에 굉장히 힘들 수 있다. 사람과 거리가 먼 언어들로 컴퓨터를 접하게 되면, 프로그래밍에 대해 굉장히 왜곡된 사고를 갖게 될 위험이 있다. 언어를 배운다는 것은 생각하는 방식을 새로 배우는 것과 마찬가지이기 때문에 중요하다. 대부분의 상황에서는, 성능이 빠른 것 보다 인간이 수월하게 자신의 의도를 반영하고 생각을 표현할 수 있는 것이 프로그래밍 언어 사용에 더 중요하다. 왜냐하면 전반적으로 컴퓨터가 워낙 빠르기 때문이다. 

- 질문4: C의 내용물에 파이썬의 껍데기를 씌워서 구현 한 패키지들이 있다고 했는데, 이러한 면에서 다른 언어들과의 조합 수월성을 따져보았을 때 파이썬이 좋은 언어라는 뜻인가요?

파이썬을 Glue Language라고도 하는데, 접착제 언어이다. 보통 Glue Language라고 불리우는 루비 등의 언어는 사실 성능이 아주 빠르지는 않다는 뜻도 된다. 왜냐하면 주요 기능들을 타 언어로 만든 것이기 때문이다. 파이썬은 C보다 20배 정도 느리지만, 그렇다 해도 썩 괜찮은 편이다. R은 C보다 수백 배 느리기 때문에 성능상 문제가 된다. 분야에 따라 다르긴 하지만, 인간이 인지적으로 100분의 1초/10분의 1초를 식별하기는 어렵지만, 컴퓨터 입장에서는 굉장히 큰 차이다. 분야에 따라 이런 것이 크게 문제가 되기도 한다. 

  - 개발자 커뮤니티가 훌륭하다는 특장점. 한국 개발자 커뮤니티도 괜찮게 유지되고 있다. 

  - 참고자료가 제법 풍부하다. 


#### 1.2. Scratch에서 Python으로! (간단한 실습!)

블록을 가지고 놀면서 Scratch에서 Python으로 자연스럽게 넘어가 봅시다. 

짝 프로그래밍: 애자일 방법론을 적극적으로 실천하는 조직에서는, 짝 프로그래밍이 아닌 경우 코드를 한 줄도 짜지 않는 경우도 있다. 최소한 그 코드를 알고 있는 사람이 두 명이 된다는 장점이 있고, 서로가 짝을 바꾸면서 자신이 알고 있는 지식을 공유하고 지식이 전파된다.
 

**실습1(예시):** 이름을 입력받고, 이름에게 인사하는 프로그램을 만들어 봅시다. 

**실습2:** 1부터 100까지 모두 더한 값 출력하기. 


<블럭>

set *total* to *0* ---> 변수 *total* 을 0으로 설정하기 
Count(셈하기) with *i* from *1* to *100* by(증분하기) *1* ---> 변수 *i*를 1부터 100까지 1만큼 증분하며 셈하기(더하기)
do change *total* by *i* ---> total을 i만큼 증분하며 바꾸기 
print *total* ---> total을 출력하기 


```python
from numbers import Number

count = None 
total = None
i = None
average = None

count = 0 
total = 0
for i in range(3, 101, 3):
  total = (total if isinstance(total, Number) else 0) + i
  count = (count if isinstance(count, Number) else 0) + 1
average = total / count
print(average)

```

<코드 설명>

*count*를 0으로 설정
*total*을 0으로 설정 
for문 (반복문) : 3부터 101보다 작은 수 사이를 3만큼 증가하며 i에 입력
total을 i로 설정 ---> 101보다 작은 3의 배수의 합 
for문 안에서 (i가 101보다 작을 때 까지) count를 1씩 증가 —> 3의 배수의 개수 세기 
*average*를 *total* 나누기 *count*로 설정
*average* 결과를 출력 

**실습3:** 1부터 100사이의 3의 배수의 합의 평균 구하기 

```python
from numbers import Number

count = None 
total = None
i = None
average = None


count = 0
total = 0
for i in range(3, 101, 3):
  total = (total if isinstance(total, Number) else 0) + i
  count = (count if isinstance(count, Number) else 0) + 1
average = total / count
print(average)
```

<코드 설명>

파이썬 기초 2 (오후)
----------------

### 1. 수업의 목표

* Python 문법 익히기
* 함수 개념 익히기
* 통계수업 복습 겸 파이썬 연습: 표본분산, 표본표준편차, 중앙값 계산해 보기 

### 2. 파이썬 프로그램 실행 순서 이해하기 

``` python
n = 0 
total = 0

for i in range(5):

    total = total + i

    n = n + 1

average = total / n

print(average)

```

`n = 0`  

- 파이썬 문법도 Scratch에서 본 것 처럼 엄밀하게 정해져 있다. 여기에서의 = 는 assignment operator로, 대입 연산자이다. 오른 쪽에는 반드시 수식, 왼 쪽에는 반드시 변수가 와야 한다.  여기에서 0 은 literal (그 자체), 정수 리터럴 int literal. 
  - 대입문은 반드시 왼 쪽에는 변수가 오고, = (대입 연산자)가 나오고, 오른 쪽에 expression, 수식이 나와야 한다. 그런데 수식이 아니라 정수 리터럴을 썼음에도 연산이 되었다는 것은, 모든 literal은 expression임을 뜻한다. 
- 컴퓨터는 2진수를 좋아한다. 메모리에 15라는 정수를 넣을 때, 파이썬은 여러 가지 방법으로 이를 실행할 수 있다. n이라는 프레임을 만들고, object를 메모리 안에 넣을 때를 생각해 보자. 15라는 리터럴은 expression의 일종이다. 모든 expression은 평가를 할 수 있다. 
  - n = 15가 평가되면, evaluated value가 도출되는데, 이 값이 object가 된다. total = 0 이 평가되면, 이 값은 0이다. 
  - 그러나 n = 0, total = 0 이면, 화살표가 같은 objects를 가리킨다. 
  - 컴퓨터의 메모리는 기본적으로 휘발성이기 때문에, 메모리가 꺼지면 여기에서 지정한 내용들은 휘발된다. 파일에 저장하거나 기타의 조치를 취하지 않으면, 죽은 Objects가 된다0

`for i in range(5):`

- for 변수 in 뭔가가 여러개 담겨 있는 바구니: = list 
  - list에 담겨 있는 개수만큼 for 문 안에 있는 행위를 반복한다. 
  - for 변수 in [0, 1, 2, 3, 4] 로 하여도 됨. 이는 0부터 4까지를 원소로 갖는 리스트를 표현하는 리터럴이다. 
  - range(100) 은 0~99까지 100개의 elements가 생긴다. 
  - 문법 뒤에 : (콜론)이 있어야 한다. 콜론이 없으면 실행되지 않는다. 

`total = total + i`

- 대입문. 왼 쪽에 변수, 대입 연산자, expression. 

  - 정의상 expression + expression도 expression이다. 대입문의 오른 쪽에는 expression만 올 수 있고, e+e도 e이기 때문에 가능한 대입문이다. 

- total에 담겨 있던 값 0, i에 담겨 있던 값 0, total + i 의 평가값 0. 그리하여 이 줄을 실행해도 달라질 것은 없다. 

- 수학에서는 x = 5 이면, 그 문제가 끝 날 때까지 x는 5이다. 파이썬에서는 n = 0이, n을 0이라고 하자, 는 뜻이 아니라 n 에 0을 담겠다는 뜻이다. 약속이나 선언이 아닌 '명령'으로 생각하면 편함. 

- 들여쓰기 레벨이 같은 구문들이 하나의 블럭이 된다. 스페이스 4개. 스페이스 4개로 적용된 tab 하나일 경우 tab도 허용. 

반복할 경우, parent 구문이 child를 낳고, child를 kill함. kill해도 죽지 않는 경우 demon이라고 함. 

`average = total / n`

- float 옵젝트가 생긴다. 컴퓨터에는 무한한 정수가 없다. 컴퓨터는 자릿수를 제한하거나 정밀도를 제한하여 메모리를 확보한다. 부동소수점 float 표기값이 결과가 된다. 파이썬에서 2와 2.0은 다르다. 2는 정수, int. 2.0은 부동소수점 float. 나눗셈의 결과 같은 것은 자동으로 float화 한다. 

- 파이썬에서 실수와 정수를 더하면 실수가 된다. 

    - 실습
    평균 구하기 
    
    
중요한 설명!!

재귀적 결합. Scratch에서 나만의 블럭을 만드는 것과 같은 개념.

```python
def calc_sum(numbs):
    result = 0 
    for num in numbs:
      result = result + num
    return result
    
scores = [50, 60, 70]
total = calc_sum(scores)
print(total)
```

`def calc_sum(numbs) block`
서로 다른 두 단어를 붙일 때 언더바를 쓰자는 약속. calculate_summation = 뭔가를 다 더해주는 함수. 블럭이 시작되기 전엔 항상 컬런을 붙인다. 구멍이 하나 뚫려있는 상자를 만들었다고 생각. 이 구멍에 리스트를 넣어보자. 이 블럭은 calc_sum이라는 함수타입의 objects를 참조. 이 단계를 실행하면, 블럭을 실행한 게 아니라 정의되기만 한 것. 
  
`return과 print 함수의 차이?`
print 는 유서깊은 함수... 어떤 단말기에 결과를 출력한다는 뜻. 함수에서 return을 하면, return된 아이가 메모리에만 있지 print하라고 시키기 전에는 보이지 않는다. 

`scores = [50, 60, 70]`
여기에서부터 실행되기 시작. 

`total = calc_sum(scores)`
함수를 호출하는 액션 함수이름(어쩌구). 글로벌 프레임과 함수만의 프레임. 함수가 실행이 끝나는 순간 함수의 프레임은 사라진다. 이러한 calc_sum(scores)의 결과값을 total에 대입한다는 대입항. 이렇게 프레임이 쌓이는 것을 stack이라고 한다. 그러면서 store이라는 이름으로 지정해준 리스트가, 위 블럭에서 만든 곳으로 들어가게 됨. 

`return`
호출했던 곳으로 돌아간다.


함수 내부의 이름공간과, 글로벌의 이름공간은 별개이다. 함수 내부에서 지정한 이름과 글로벌 공간에서 지정한 이름은 서로 별개이다. 블럭 함수 안에서 일어나는 일은 바깥 세상과 격리되어 있다. 그 결과값을 내보내거나, 입력값을 받을 수 있을 뿐. 