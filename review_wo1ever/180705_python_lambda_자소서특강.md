# 180705

## 애란선생님

### 오전수업

#### 함수란?

- 인셉션처럼 꿈 속의 꿈, 꿈 속의 꿈 속의 꿈, ..., 꿈을 깨면서 꿈 안의 것을 하나(토템) 가지고 나올 수 있는데 이게 return 되는 값이라고 볼 수 있음.
- www.stackoverflow.com : 개발자들의 지식인같은 사이트

#### lambda 란?

```python
names = ['Alan', 'Dave', 'Brad', 'Cate']
ages = [50, 60, 30, 40]
```

: 이름과 나이를 담고 있는 리스트를 만들어서 정렬함.

```python
students = list(zip(names, ages))    #list 두 개를 잠궈주어 튜플을 만듬
students
```

: 튜플이 네 개가 있는 리스트가 하나 만들어짐.

: [('Alan', 50), ('Dave', 60), ('Brad', 30), ('Cate', 40)] 

```python
def by_name(student):
  return student[0]

def by_age(student):
  return student[1]

sorted(students, key=by_name)
sorted(students, key=by_age)

# key: student의 몇 번째 인자(0, 1)로 정렬시키기. 함수 밖에서 key를 이용하여 정렬해 줌.
# def 함수 이름을 지어주어야 함.
```

```python
# 위의 사용자정의 함수와 동일한 결과
sorted(students, key=lambda s: s[0])
# 함수의 인자(key)를 함수로 받은 셈(second order fuctnion)

# 위의 코드와 동일
by_name = lambda s: s[0]
sorted(students, key=by_name)
```

: student를 정렬할건데, s의 0번째 것을 뽑아 정렬해라.

- lambda: 한 줄짜리 짧은 함수를 이름짓지 않고 순식간에 쓰고 버리는 함수
- lambda는 이름이 없는 함수임.
- 다음번에 호출 불가능(일회성)

```python
def blah(x):
    return x * 2
# 위의 함수와 동일한 결과
lambda x : x * 2


def blahblah(x, y):
    return x + y
# 위의 함수와 동일한 결과
a = lambda x, y : x + y

# a를 계속 재활용한다면 일회용은 아닌 셈, 변수에 정의하지 말라는 경고 뜸
```

- abstraction(정의) --> application / call(적용)
- higher-order function(고차 함수) : 함수와 여러 함수를 포갬



#### 실습1
#### 실습2
농구 평균 득점으로 정렬하기
분산이 작은 선수 고르기

```
수업 끝나고 연습 해 보기
```

- 리스트를 담는 함수는 보통 복수형으로  씀.







## 오후 수업

### 매력적인 나 사용 제안서 - 자소서 피드백

#### 김지해 선생님

##### 자소서를 쓰자

자소서가 정답은 아니다.

실존에 대한 물음? / 취업이라는 목적을 위해 최소한의 노력을 들여 쓰는 글

##### 1. 자소서 예시

우리가 흔히 하는 착각은  개발에 대한 지식이 없을 수도 있다. (정보의 불균형에 대해 감안하고 쓰기)

만국 공통어로 작성하자.

안좋은 데이터는 보여줄 필요가 없음! 좋은 데이터들만 보여줘도 모자란데...

​	(eg) 스티브잡스가  말했다.... 광고를 보았다... 

- 나 똑똑해
- 나 다른 사람들과 잘 지내
- 나 잠재력 있어

##### 2. 자소서의 특징

- 설명하는 글

  나에 대한 정보를 주는 글

- 공식적인 글

  일정한 형식과 객관적 시각을 유지

- 사적인 내용을 공적인 형식으로 갖춰야 하는 글!

- 줄바꿈이 단락이다.

  한 줄씩 바꾸기가 너무 익숙해져 있음

- 분량도 중요하다.

##### 3. 첫 문장이 중요하다!

- 감성적, 주관적인 단어나 문장을 지양하자.

  (eg) 무언가를 창조, 즐겁다 (?)

  (eg) 정직원 제안을 받았어? 뭘 했길래? 뭘 잘했어? 궁금하네

- 500원으로 낚되, 정보 불균형에서 친절해지자.

  초등학교 6학년 조카에게 설명하는 듯이

- 육하원칙을 기반으로 작성하자.

  누가(나), **언제, 어디서, 무엇을, 어떻게**(당위성이 필요한 글)

  구체적인 수치를 나타내면 기억에 더 잘 남음.

- **어떻게** 했는지?

  행동 쓰기가 중요!

##### 4. 자소서의 내용

- 팀플은 무조건 팀장이어야 함.
- 회사 칭찬을 좀 해야 됨.

###### 첫 문장 쓰기 실습

```
ver1.

저는 통계학과와 산업공학과를 졸업하여 그 동안 통계 분석에 관련한 이론을 다지고, 분석적인 사고를 키웠습니다.

ver2.

저는 졸업 논문 프로젝트를 진행하며 새로운 시각으로 문제를 해결했던 경험이 있습니다.

ver3.

저는 졸업 논문 프로젝트 중 새로운 시각으로 접근하여 이혼율에 영향을 미치는요인들을 83%의 적합도로 분석하였던 경험이 있습니다.
```

###### 입사 후 포부

###### 지원동기와 입사 후 포부가 합쳐져 있을 경우

- 회사 예찬과 칭찬
- 1단락에는 직무 동기, 2단락에는 회사 동기를 작성

###### 지원동기 내용

- 내가 무슨 경험을 해 보았다. 이게 어떤 거였다.
- 이런 경험을 해 보니까 이런걸 배웠고, 적성과 흥미에 맞았다. 관심이 생겼다.

###### 지원동기 쓰기 실습

```
저는 졸업 논문 프로젝트 중 새로운 시각으로 접근하여 이혼율에 영향을 미치는 요인들을 83%의 적합도로 분석하여 수업에서 A+의 성적을 받았던 경험이 있습니다. 이혼의 요인을 더욱 정확하게 분석하기 위하여 출산율, 혼인율 등 정형화된 데이터뿐만 아니라 성격이나 기분과 같이 주관적인 데이터들이 필요했습니다. 저는 날씨가 사람의 영향에 영향을 미친다고 생각하였고, 새로운 요인으로 '날씨'를 추가하였습니다. 그 결과 제가 설정한 모형은 10년간의 이혼율을 83%의 정확도로 적합할 수 있었고, 교수님에게도 칭찬을 들으며 좋은 성적을 받았습니다.

프로젝트를 진행하며 저는 얻을 수 없었던 정성적 데이터를 어떤 방식으로 대체할까에 대한 고민을 하게 되었습니다. 주변에서 쉽게 얻을 수 있는 정량적 데이터를 이용하기로 생각해 보았습니다. 분석을 통하여 유의미한 결과를 얻는 일에 흥미가 생겼고, 이 과정에서 저의 새로운 시각으로 데이터를 바라보는 힘이 큰 도움이 되었습니다.
```



