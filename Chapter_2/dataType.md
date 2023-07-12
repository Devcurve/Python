#### Python에서 사용되는 자료형(Data Types)

1. **Number**
>- 정수형 (`int`): 정수를 나타내는 자료형입니다. 예: `10`, `-5`
>- 실수형 (`float`): 실수를 나타내는 자료형입니다. 예: `3.14`, `-2.5`


```
> 예제 1
age = 10
print("나이:", age)
```

```
> 예제 2
num1 = int(input("첫 번째 정수를 입력하세요: "))
num2 = int(input("두 번째 정수를 입력하세요: "))
sum_result = num1 + num2
print("두 정수의 합은:", sum_result)
```


<pre>
<code>import math

radius = float(input("원의 반지름을 입력하세요: "))
area = math.pi * radius ** 2
print("원의 넓이는:", area)
</code>
</pre>

---

2. **String**
> - 문자열 (`str`): 문자들의 연속을 나타내는 자료형입니다. 예: `"Hello, World!"`, `'Python'`

<pre>
<code>name = input("이름을 입력하세요: ")
age = input("나이를 입력하세요: ")
greeting = "안녕하세요, 저는 " + name + "이고 " + age + "살입니다."
print(greeting)
</code>
</pre>

---

3. **Boolean**
> - 불린 (`bool`): 참(True) 또는 거짓(False)을 나타내는 자료형입니다. 예: `True`, `False`

<pre>
<code>age = int(input("나이를 입력하세요: "))
is_adult = age >= 18
print("성인 여부:", is_adult)
</code>
</pre>

---

4. **List**
> - 리스트 (`list`): 여러 개의 값을 순서대로 담는 자료형입니다. 값들은 대괄호(`[]`)로 둘러싸여 있고, 쉼표로 구분됩니다. 예: `[1, 2, 3]`, `['apple', 'banana', 'orange']`

<pre>
<code>numbers = []
count = int(input("숫자의 개수를 입력하세요: "))

for i in range(count):
    num = float(input("숫자를 입력하세요: "))
    numbers.append(num)

sum_result = sum(numbers)
avg_result = sum_result / count

print("리스트의 합은:", sum_result)
print("리스트의 평균은:", avg_result)
</code>
</pre>

---

5. **Tuple**
> - 튜플 (`tuple`): 여러 개의 값을 순서대로 담는 자료형입니다. 값들은 소괄호(`()`)로 둘러싸여 있고, 쉼표로 구분됩니다. 튜플은 변경할 수 없는(immutable) 자료형입니다. 예: `(1, 2, 3)`, `('red', 'green', 'blue')`

<pre>
<code>
fruits = ("사과", "오렌지")
prices = (1500, 1000)

for i in range(len(fruits)):
    print(fruits[i], "의 가격은", prices[i], "원입니다.")
</code>
</pre>

---

6. **Set**
> - 집합 (`set`): 중복되지 않는 값을 담는 자료형입니다. 값들은 중괄호(`{}`)로 둘러싸여 있고, 쉼표로 구분됩니다. 예: `{1, 2, 3}`, `{'apple', 'banana', 'orange'}`

<pre>
<code>
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
</code>
</pre>

---

7. **Dictionary**
> - 사전 (`dict`): 키(key)와 값(value)의 쌍을 담는 자료형입니다. 키와 값은 콜론(`:`)으로 연결되고, 각 쌍들은 쉼표로 구분됩니다. 예: `{'name': 'John', 'age': 30, 'city': 'Seoul'}`

<pre>
<code>dictionary = {
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
</code>
</pre>


<!-- ## [목차](./READMY.md) -->
<a href="../READMY.md">처음으로</a> <br>
<a href="../READMY.md">다음</a>
