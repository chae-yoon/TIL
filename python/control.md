# 제어문(Control Statement)

## 제어문이란

- 파이썬은 기본적으로 위에서부터 아래로 순차적으로 명령을 수행
- 특정 상황에 따라 코드를 선택적으로 실행(분기/조건)하거나 계속하여 실행(반복)하는 제어가 필요함
- 제어문은 순서도(flow chart)로 표현이 가능

<br>

## 조건문(Conditional Satatement)

- 참/거짓을 판단할 수 있는 조건식과 함께 사용
- expression에는 참/거짓에 대한 조건식
  - 조건이 참인 경우 이후 들여쓰기 되어있는 코드 블럭 실행
  - 이외의 경우 else 이후 들여쓰기 되어있는 코드 블럭 실행
  - else는 선택적으로 활용 가능함

```python
if < expression >:
  # Run this Code block
else:
  # Run this Code block
```

<br>

## 복수 조건문

- 복수의 조건식을 활용할 경우 elif를 활용하여 표현

```python
if < expression >:
  # Run this Code block
elif < expression >:
  # Run this Code block
elif < expression >:
  # Run this Code block
else:
  # Run this Code block
```

<br>

## 중첩 조건문

- 조건문은 다른 조건문에 중첩되어 사용될 수 있음
- 단, 들여쓰기를 유의하여 작성할 것

```python
if < expression >:
  # Run this Code block
  if < expression >:
    # Run this Code block
else:
  # Run this Code block
```

<br>

## 반복문(Loop Statement)

- 특정 조건을 도달할 때까지, 계속 반복되는 일련의 문장

<br>

## 반복문의 종류

- while문
  - 종료조건에 해당하는 코드를 통해 반복문을 종료시켜야 함
- for문
  - 반복가능한 객체를 모두 순회하면 종료(별도의 종료조건이 필요 없음)
- 반복 제어
  - break, continue, for-else

## while문

- while문은 조건식이 참인 경우 반복적으로 코드를 실행

```python
while < expression >:
  # Run this Code block
```

<br>

## for문

- 시퀀스(string, tuple, list, range)를 포함한 순회가능한 객체요소를 모두 순회함
- 처음부터 끝까지 모두 순회하므로 별도의 종료조건이 필요하지 않음
- 순회 가능한 객체: 컨테이너형(문자열, 리스트, 튜플, range, set, dictionary) 등

```python
for < 변수명 > in < iterable >:
  # Run this Code block
```

<br>

## 반복문 제어

- break
  - 반복문을 종료
- continue
  - continue 이후의 코드 블록은 수행하지 않고, 다음 반복을 수행
- for-else
  - 끝까지 반복문을 실행한 이후에 else문 실행
  - break를 통해 중간에 종료되는 경우 else문은 실행되지 않음
