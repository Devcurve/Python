#### Python에서 사용되는 자료형(Data Types)


1. **String**
> - 문자열 (`str`): 문자들의 연속을 나타내는 자료형입니다. 예: `"Hello, World!"`, `'Python'`

```
name = input("이름을 입력하세요: ")
greeting = "안녕하세요, 저는 " + name + " 입니다. "
print(greeting)

> Shift + Enter
```
---


2. **Number**
>- 정수형 (`int`): 정수를 나타내는 자료형입니다. 예: `10`, `-5`
>- 실수형 (`float`): 실수를 나타내는 자료형입니다. 예: `3.14`, `-2.5`

```
> 예제 1
# 두 정수의 합 구하기

# 두 개의 정수를 변수에 저장합니다.
num1 = 5
num2 = 3

# 두 정수를 더하여 결과를 저장하는 변수를 만듭니다.
sum_result = num1 + num2

# 결과를 출력합니다.
print("두 정수의 합:", sum_result)
```

```
> 예제 2
# 두 정수를 입력받고 합 구하기

# 두 개의 정수를 입력받아 변수에 저장합니다.
num1 = int(input("첫 번째 정수를 입력하세요: "))
num2 = int(input("두 번째 정수를 입력하세요: "))

# 두 정수를 더하여 결과를 저장하는 변수를 만듭니다.
sum_result = num1 + num2

# 결과를 출력합니다.
print("두 정수의 합은:", sum_result)
```
---

3. **Boolean**
> - 불린 (`bool`): 참(True) 또는 거짓(False)을 나타내는 자료형입니다. 예: `True`, `False`

```
> 예제 1

result = True
print(result)

result = False
print(result)
```

```
> 예제 2

# 두 개의 정수를 입력받아 변수에 저장합니다.
num1 = int(input("첫 번째 정수를 입력하세요: "))
num2 = int(input("두 번째 정수를 입력하세요: "))

# 서로의 값을 비교하여 True & False 를 반환 합니다.
print(num1 < num2)
```

---

4. **List**
> - 리스트 (`list`): 여러 개의 값을 순서대로 담는 자료형입니다. 값들은 대괄호(`[]`)로 둘러싸여 있고, 쉼표로 구분됩니다. 예: `[1, 2, 3]`, `['apple', 'banana', 'orange']`

```
> 예제 1

# List를 생성 합니다.
# 리스트는 대괄호로 초기값을 셋팅 합니다.
numbers = []

# 몃번의 입력을 받을지 정합니다.
numbers.append(input("첫 번째 정수를 입력하세요: "))
numbers.append(input("두 번째 정수를 입력하세요: "))
numbers.append(input("세 번째 정수를 입력하세요: "))

# 결과를 확인 합니다.  
print(numbers)
```
<p align="center">
  <img src="./Image/jupyterEditor_4.png" alt="jupyterEditor_4">
</p>

---

5. **Tuple**
> - 튜플 (`tuple`): 여러 개의 값을 순서대로 담는 자료형입니다. 값들은 소괄호(`()`)로 둘러싸여 있고, 쉼표로 구분됩니다. 튜플은 변경할 수 없는(immutable) 자료형입니다. 예: `(1, 2, 3)`, `('red', 'green', 'blue')`

```
# 가족 구성원의 이름과 나이를 튜플로 저장합니다.
father = ('아빠', 55)
mother = ('엄마', 53)
me = ('나', 25)
# brother
# sister

# 가족 구성원의 정보를 모아둔 튜플을 생성합니다.
family = (father, mother, me)

# 결과를 확인합니다.
print(family)
```
<p align="center">
  <img src="./Image/jupyterEditor_5.png" alt="jupyterEditor_5">
</p>

---

6. **Set**
> - 집합 (`set`): 중복되지 않는 값을 담는 자료형입니다. 값들은 중괄호(`{}`)로 둘러싸여 있고, 쉼표로 구분됩니다. 예: `{1, 2, 3}`, `{'apple', 'banana', 'orange'}`

```
numbers = set()

while True:
    num = int(input("숫자를 입력하세요 (0 입력 시 종료): "))
    if num == 0:
        break
    numbers.add(num)

if numbers:
    min_num = min(numbers)
    max_num = max(numbers)
    print("가장 작은 숫자:", min_num)
    print("가장 큰 숫자:", max_num)
else:
    print("입력된 숫자가 없습니다.")
```
<p align="center">
  <img src="./Image/jupyterEditor_5.png" alt="jupyterEditor_5">
</p>

---

7. **Dictionary**
> - 사전 (`dict`): 키(key)와 값(value)의 쌍을 담는 자료형입니다. 키와 값은 콜론(`:`)으로 연결되고, 각 쌍들은 쉼표로 구분됩니다. 예: `{'name': 'John', 'age': 30, 'city': 'Seoul'}`

```
dictionary = {
    "apple": "사과",
    "banana": "바나나",
    "orange": "오렌지",
    "grape": "포도"
}

word = input("영어 단어를 입력하세요: ")
if word in dictionary:
    translation = dictionary[word]
    print("한국어 뜻은:", translation)
else:
    print("사전에 없는 단어입니다.")
```
<p align="center">
  <img src="./Image/jupyterEditor_5.png" alt="jupyterEditor_5">
</p>


<!--목차 & 다음으로 페이지 이동-->
[목차](https://github.com/Devcurve/Python/blob/main/README.md)<br>
[이전 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/Variable.md)<br>
<!--[다음 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/.md)-->
