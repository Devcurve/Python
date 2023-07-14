
## **조건문 or 분기문**

### ___if 설명___
- `if`문은 주어진 조건이 '참'인 경우에만 특정 코드 블록을 실행합니다.

```
> 방법

if 조건:
    # 조건이 참일 때 실행되는 코드
```
<br>

### ___예시___
- 사탕 분배하기

```
candies = int(input("사탕 개수를 입력하세요: "))

if candies == 0:
    print("사탕이 없어요. ㅠㅠ")

if candies == 1:
    print("사탕이 1개 있어요!")

if candies >= 2:
    print("사탕이 여러 개 있어요!")
```
<br>

---

### ___if - else 설명___
- `if-else`문은 주어진 조건이 '참'인 경우와 '거짓'인 경우에 대해 서로 다른 코드 블록을 실행합니다.

```
> 방법

if 조건:
    # 조건이 참일 때 실행되는 코드
else:
    # 조건이 거짓일 때 실행되는 코드
```
<br>

### ___if - elif - else 설명___
- 여러 개의 조건을 비교해야 하는 경우 `if-elif-else`문을 사용할 수 있습니다. `elif`키워드는 이전 조건이 거짓인 경우에 다음 조건을 검사합니다.

```
> 방법

if 조건1:
    # 조건1이 참일 때 실행되는 코드
elif 조건2:
    # 조건2가 참일 때 실행되는 코드
else:
    # 모든 조건이 거짓일 때 실행되는 코드
```
<br>

### ___사용방법___
```
num = int(input("숫자를 입력하세요: "))

if num > 0:
    print("입력한 숫자는 양수입니다.")
elif num < 0:
    print("입력한 숫자는 음수입니다.")
else:
    print("입력한 숫자는 0입니다.")
```
<br>

### ___예제___

- 놀이공원 입장료 계산하기

```
> 예제 1

height = int(input("키를 입력하세요 (cm): "))

if height >= 120:
    print("놀이공원에 입장할 수 있습니다!")
else:
    print("키가 작아서 놀이공원에 입장할 수 없습니다.")
```
<br><br>

- 점수에 따른 학점 부여하기

```
> 예제 2

score = int(input("시험 점수를 입력하세요: "))

if score >= 90:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
elif score >= 60:
    grade = "D"
else:
    grade = "F"

print("학점은", grade, "입니다.")
```
<br><br>
- 날씨에 따른 옷차림 추천하기

```
> 예제 3

weather = input("오늘 날씨는 어때요? (맑음/흐림/비/눈): ")

if weather == "맑음":
    outfit = "반팔과 반바지"
elif weather == "흐림" or weather == "비":
    outfit = "긴팔과 바지"
elif weather == "눈":
    outfit = "두꺼운 옷과 장화"
else:
    outfit = "올바른 날씨 정보를 입력하세요."

print("오늘은", weather, "이니까", outfit, "를 입으세요!")
```
<br><br>
- 짝수와 홀수 판별하기

```
> 예제 4

number = int(input("숫자를 입력하세요: "))

if number % 2 == 0:
    print("입력한 숫자는 짝수입니다.")
else:
    print("입력한 숫자는 홀수입니다.")
```
<br><br>
- 나이에 따른 할인 혜택 제공하기

```
> 예제 5

age = int(input("나이를 입력하세요: "))

if age < 8:
    print("무료 입장입니다!")
elif age >= 8 and age < 18:
    print("청소년 할인이 적용됩니다.")
else:
    print("일반 요금이 적용됩니다.")
```
<br><br>

---
<!--목차 & 다음으로 페이지 이동-->
[목차](https://github.com/Devcurve/Python/blob/main/README.md)<br>
[이전 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/dataType.md)<br>
[다음 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/space.md)
