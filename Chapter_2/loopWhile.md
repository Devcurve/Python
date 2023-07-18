## **반복문 or while**

### ___while 설명___
- `while`문은 주어진 조건이 `참`인 경우에 코드 블록을 `반복적으로 실행`합니다.

```
> 방법

while 조건:
    # 코드 블록

-----------------------------------------------

while 조건:
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
num = 1

while num <= 5:
    print(num)
    num += 1

===================
> 1
> 2
> 3
> 4
> 5
```
<br>

---

### ___while 예제___

- 1부터 5까지 숫자 출력하기

```
> 예제 1

num = 1

while num <= 5:
    print(num)
    num += 1
```
<br><br>

- 구구단 출력하기 (3단)

```
> 예제 2

num = 1

while num <= 9:
    print(3, "x", num, "=", 3 * num)
    num += 1
```
<br><br>
- 리스트 요소 출력하기

```
> 예제 3

fruits = ["사과", "바나나", "딸기", "수박", "포도"]
index = 0

while index < len(fruits):
    print(fruits[index])
    index += 1
```
<br><br>
- 문자열 반복 출력하기

```
> 예제 4

word = "Hello"
index = 0

while index < len(word):
    print(word[index])
    index += 1
```
<br><br>
- 별 피라미드 출력하기

```
> 예제 5

num = 1

while num <= 5:
    print("*" * num)
    num += 1
```
<br><br>

---
<!--목차 & 다음으로 페이지 이동-->
[목차](https://github.com/Devcurve/Python/blob/main/README.md)<br>
[이전 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/Operators.md)<br>
<!--[다음 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/.md)-->
