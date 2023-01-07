# 용어

## 객체(Object)

숫자, 문자, 클래스 등 값을 가지고 있는 모든 것

<br>

## 변수(Variable)

컴퓨터 메모리 어딘가에 저장되어 있는 객체를 참조하기 위해 사용되는 이름
<br>
동일 이름에 다른 객체를 언제든 할당할 수 있기 때문에 `변수`라고 불림

변수는 할당 연산자 `=`를 통해 값을 할당(assignment)

<br>

### 변수 할당

- 같은 값을 동시에 할당 할 수 있음

  ```python
  x = y = 1004
  ```

- 다른 값을 동시에 할당 할 수 있음

  ```python
  x, y = 1, 2
  ```

- 각각 값을 바꿔서 저장 할 수 있음

```python
x = 10
y = 20

y, x = x, y
```

<br>

## 식별자(Identifiers)

파이썬 객체(변수, 함수, 모듈, 클래스 등)를 식별하는데 사용하는 이름(name)

<br>

### 규칙

- 식별자의 이름은 영문 알파벳, 언더스코어(\_), 숫자로 구성
- 첫 글자에 숫자가 올 수 없음
- 길이 제한이 없고, 대소문자를 구별
- 키워드 및 예약어는 사용할 수 없음 (ex. False, None, True, and, ...)
- 내장함수나 모듈 등의 이름으로 만들면 안됨 (ex. print, input, ...)

<br>

## 자료형(Data Type)

<br>

### 자료형 분류

- <b>숫자</b>
  - 수치형(Numberic Type)
    - [int(정수, integer)](#int)
    - [float(부동소수점, 실수, floating point number)](#float)
    - [complex(복소수, complex number)](#complex)
  - [불린형(Boolean Type)](#boolean)

<br>

- <b>시퀀스(Sequence)</b>
  - [문자열(String)](#string)
  - 튜플(Tuple)
  - [리스트(List)](#list)
  - [레인지(Range)](#range)

<br>

- <b>컬렉션(Collection)</b>
  - 집합(Set)
  - 딕셔너리(Dictionary)

<br>

- <b>None</b>

<br>

### int

- 모든 정수의 타입
- 오버플로우가 발생하지 않음

<br>

### float

- 정수가 아닌 모든 실수의 타입
- 부동소수점
  > 실수 연산 과정에서 오류가 발생할 수 있음

<br>

### complex

- 실수부와 허수부로 구성된 복소수의 타입
- 허수부는 `j`로 표현

<br>

### boolean

- True / False 값을 가진 타입
- 비교 / 논리 연산을 수행함에 있어서 활용됨

<br>

### string

- 모든 문자는 str 타입
- 문자열은 작은 따옴표(')나 큰 따옴표(")를 활용하여 표기
- 따옴표 안에 따옴표를 표현할 경우 다른 따옴표로 문자열 생성
- 삼중으로 따옴표를 사용한 경우 여러줄을 나눠 입력 가능
- 인덱스를 통해 특정 값에 접근할 수 있음
- 변경 불가능함(Immutable)
- 반복 가능함(Iterable)

<br>

### list

- 변경 가능한 값들의 나열된 자료형
- 순서를 가지며, 서로 다른 타입의 요소를 가질 수 있음
- 변경 가능함(Mutable)
- 반복 가능함(Iterable)
- 항상 대괄호 형태로 정의하며, 요소는 `콤마(,)`로 구분
- `대괄호` 혹은 `list()` 를 통해 생성
- 순서가 있는 시퀀스로 인덱스를 통해 접근 가능
- 값 추가는 `.append()` 활용

  ```python
  even_numbers = [2, 4, 6, 8]
  even_numbers.append(10)

  print(even_numbers) # [2, 4, 6, 8, 10]
  ```

- 값 삭제는 `.pop()` 활용

  ```python
  even_numbers = [2, 4, 6, 8]
  even_numbers.pop(0)

  print(even_numbers) # [4, 6, 8]
  ```

<br>

### range

- 숫자의 시퀀스를 나타내기 위해 사용
- 변경 불가능함(Immutable)
- 반복 가능함(Iterable)
- 기본형: range(n)
  - 0부터 n-1까지의 숫자의 시퀀스
- 범위 지정: range(n, m)
  - n부터 m-1까지의 숫자의 시퀀스
- 범위 및 스텝 지정: range(n, m, s)
  - n부터 m-1까지 s만큼 증가시키며 숫자의 시퀀스

<br>

### None

- 값이 없음을 표현하기 위한 None 타입
- 일반적으로 반환 값이 없는 함수에서 사용하기도 함

<br>

## 주석(Comment)

코드에 대한 설명

주석으로 처리될 내용 앞에 `#`을 입력

<br>

## String Formatting

### %-formatting

- 문자열을 변수를 활용하여 만드는 방법

```python
name = 'Kim'
score = 4.5

print('Hello, $s' % name)
print('내 성적은 %d' % score)
print('내 성적은 %f' % score)
```

```bash
Hello, Kim
내 성적은 4
내 성적은 4.500000
```

<br>

### f-string

- 문자열을 변수를 활용해여 만드는 방법

```python
name = 'Kim'
score = 4.5

print(f'Hello, {name}! 내 성적은 {score}')
```

```bash
Hello, Kim! 내 성적은 4.5
```

<br>

## 형 변환(Typecasting)

### 암시적 형 변환(Implicit)

- 사용자가 의도하지 않고, 파이썬 내부적으로 자료형을 변환 하는 경우

<br>

### 명시적 형 변환(Explicit)

- str\*, float ⇒ int
- str\*, int ⇒ float
- int, float, list, tuple, dict ⇒ str

> \*형식에 맞는 문자열만 가능
