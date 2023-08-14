## **반복문 or for**
### ___for 설명___
- `for`문은 `시퀀스(예: 리스트, 튜플, 문자열)`의 각 원소에 대한 코드 블록을 `반복적으로 실행`합니다.

```
> 방법

for 요소 in 시퀀스:
    # 코드 블록

-----------------------------------------------

for 요소 in 시퀀스:
  ┌────────────────────────────────────────┐
┌──┐반복문이 실행되는 코드 블록
│공│문장1
│백│문장2
└──┴───────────────────────────────────────┘

-----------------------------------------------
```
<br>

### ___예시___
- 과일의 종류

```
fruits = ["사과", "바나나", "딸기"]

for fruit in fruits:
    print(fruit)

===================
> "사과"
> "딸기"
> "바나나"
```
<br>

---

### ___for 예제___

- 1부터 5까지 숫자 출력하기

```
> 예제 1

for i in range(1, 6):
    print(i)
```
<br><br>

- 구구단 출력하기 (2단)

```
> 예제 2

for i in range(1, 10):
    print(2, "x", i, "=", 2 * i)
```
<br><br>
- 리스트 요소 출력하기

```
> 예제 3

fruits = ["사과", "바나나", "딸기", "수박", "포도"]

for fruit in fruits:
    print(fruit)
```
<br><br>
- 문자열 반복 출력하기

```
> 예제 4

word = "Hello"

for ch in word:
    print(ch)
```
<br><br>
- 별 피라미드 출력하기

```
> 예제 5

for i in range(1, 6):
    print("*" * i)
```
<br><br>

---
<!--목차 & 다음으로 페이지 이동-->
[목차](https://github.com/Devcurve/Python/blob/main/README.md)<br>
[이전 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/space.md)<br>
[다음 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/Operators.md)
