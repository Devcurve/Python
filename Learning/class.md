## class

- `__init__`(self, ...): 객체 초기화를 위한 생성자 메서드입니다. 객체가 생성되면 자동으로 호출됩니다.

```
class Box:
    def __init__(self, number):
        self.number = number  
    # Box 클래스에 number 라는 필드값이 생성됩니다.
    # 그리고 그 안에 숫자를 넣습니다. 보통 이것을 초기화 라고 이야기 합니다.

box = Box(10)
print(box.number)



> 10
```
<br><br>

- `__str__`(self): 객체를 사람이 읽기 쉬운 문자열로 나타내는 메서드입니다. 박스를 문자열로 바꿔서 출력할 때 자동으로 사용됩니다

```
class Box:
    def __init__(self, number):
        self.number = number  

    def __str__(self):
        return f"이 박스 안에는 {self.number}가 있어요!"

    # f"%#@$#%#@" 문자열 앞에 'f' 를 넣는 이유는...
    # 문자열 내부에 '{self.number}' 이러한 방식으로 변수를 사용할 수 있습니다.
    # python 3.6 이상 버전에서만 사용 가능합니다.

box = Box(10)
print(box)



> 이 박스 안에는 10가 있어요!
```
<br><br>

- `__repr__`(self): 객체의 정확한 문자열 표현을 반환하는 메서드로 개발자에게 편의를 제공하며, 주로 디버깅용입니다. 반환된 문자열은 가능한 한 객체를 재생성하기 위한 코드 형식이어야 합니다.

```
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def __repr__(self):
        return f"Person('{self.name}', {self.age})"

person = Person('John', 20)

# 디버깅
print(person)  # 출력: Person('John', 20)

# 객체의 재생성
new_person = eval(repr(person))
print(new_person)  # 출력: Person('John', 20)



> Person('John', 20)
> Person('John', 20)
```
<br><br>

- `__add__`(self, other): `+` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.

```
class Box:
    def __init__(self, number):
        self.number = number  # 박스 안에 숫자를 넣습니다.

    def __add__(self, other):
        return Box(self.number + other.number)  # 두 박스를 더하면, 숫자가 더해진 새 박스를 만듭니다.

    def __str__(self):
        return f"이 박스 안에는 값은 {self.number} 입니다."  # 박스를 설명하는 문자열을 만듭니다.


# 각각 5와 3으로 초기화 합니다.
box1 = Box(5)
box2 = Box(3)

# 두 객체를 더하면, 결과값이 반환된 새로운 객체가 만들어집니다.
box3 = box1 + box2

# 객체끼리 더했지만 객체 내부에 생성된 값이 변경된 것이 핵심입니다.

# 결과 출력
print(box3)



> 이 박스 안에는 값은 8 입니다.
```
<br><br>

- `__sub__`(self, other): `-` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.

```
class Box:
    def __init__(self, number):
        self.number = number  # 박스 안에 숫자를 넣습니다.

    def __sub__(self, other):
        return Box(self.number - other.number)  # 두 박스를 빼면, 숫자가 뺀 값이 들어간 새 박스를 만듭니다.

    def __str__(self):
        return f"이 박스 안에는 {self.number}가 있어요!"  # 박스를 설명하는 문자열을 만듭니다.

# 각각 5와 3으로 초기화 합니다.
box1 = Box(5)
box2 = Box(3)

# 객체끼리 뺐지만 객체 내부에 생성된 값이 변경된 것이 핵심입니다.

# 두 객체를 뺀면, 결과값이 반환된 새로운 객체가 만들어집니다.
box3 = box1 - box2

# 결과 출력
print(box3)



> 이 박스 안에는 값은 2 입니다.
```
<br><br>


#### **___위 예제를 확인하고, 아래 내용을 작성해주세요___**

- `__mul__`(self, other): `*` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__truediv__`(self, other): `/` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__floordiv__`(self, other): `//` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__mod__`(self, other): `%` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__pow__`(self, other): `**` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__eq__`(self, other): `==` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__ne__`(self, other): `!=` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__lt__`(self, other): `<` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__le__`(self, other): `<=` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__gt__`(self, other): `>` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.
- `__ge__`(self, other): `>=` 연산자의 동작을 정의할때 이 메서드를 사용할 수 있습니다.

---

- `__len__`(self): 객체의 길이를 반환하기 위한 메서드입니다. 주로 컨테이너 객체(리스트, 튜플, 문자열 등)에서 사용됩니다.

```
class Box:
    def __init__(self):
        self.apples = []  # 바구니 안에 사과를 넣습니다.

    def add_apple(self, apple):
        self.apples.append(apple)  # 사과를 바구니에 추가합니다.

    def __len__(self):
        return len(self.apples)  # 바구니 안의 사과 개수를 반환합니다.


box = Box()  # 바구니를 만듭니다.
box.add_apple('apple1')  # 사과를 바구니에 넣습니다.
box.add_apple('apple2')  # 또 다른 사과를 바구니에 넣습니다.
print(len(box))  # 바구니 안의 사과 개수를 출력합니다.

box.add_apple('apple3')  # 또 다른 사과를 바구니에 넣습니다.
print(len(box))  # 바구니 안의 사과 개수를 출력합니다.



> 2
> 3
```

- 하지만 일반적으로 `len()` 함수를 사용했던것과 같이 사용할 수 있다.

```
list = []
list.append(1)

print(len(list))

> 1
```

```
# 마찬가지로 다음과 같은 방식으로 사용할 수 있기때문에 사용자가 선택적으로 사용할 수 있다.
print(len(box.apples))
print(len(box))
```

<br><br>


- `__getitem__`(self, index): 객체에서 인덱싱을 통해 특정 요소를 반환하기 위한 메서드로, 대괄호를 이용한 인덱싱에 대해 동작을 정의할 때 사용됩니다.

```
class Box:
    def __init__(self):
        self.apples = []  # 바구니 안에 사과를 넣습니다.

    def add_apple(self, apple):
        self.apples.append(apple)  # 사과를 바구니에 추가합니다.

    def __getitem__(self, index):
        return self.apples[index]  # 바구니 안의 사과를 인덱스로 반환합니다.

box = Box()  # 바구니를 만듭니다.

box.add_apple('apple1')  # 사과를 바구니에 넣습니다.
box.add_apple('apple2')  # 또 다른 사과를 바구니에 넣습니다.

# 객체를 생성했지만 리스트와 같은 방식으로 사용할 수 있다.
print(box[0])
print(box[1])


> apple1
> apple2
```
<br><br>


- `__setitem__`(self, index, value): 객체에서 인덱싱을 통해 특정 요소를 설정하기 위한 메서드입니다.

```
class Box:
    def __init__(self):
        self.items = []  # 박스 안에 아이템을 넣습니다.

    def add_item(self, item):
        self.items.append(item)  # 아이템을 박스에 추가합니다.

    def __getitem__(self):
        return self.items  # 박스 안의 아이템을 인덱스로 반환합니다.

    def __getitem__(self, index):
        return self.items[index]  # 박스 안의 아이템을 인덱스로 반환합니다.

    def __setitem__(self, index, value):
        self.items[index] = value  # 박스 안의 아이템을 인덱스로 할당하거나 변경합니다.

box = Box()  # 박스를 만듭니다.

box.add_item('item1')  # 아이템을 박스에 넣습니다.
box.add_item('item2')  # 또 다른 아이템을 박스에 넣습니다.

print(box[0])  # 박스 안의 첫 번째 아이템을 출력합니다.



> item1
```

```
box[0] = 'new_item'  # 박스 안의 첫 번째 아이템을 변경합니다.

print(box[0])  # 박스 안의 첫 번째 아이템을 출력합니다.
print(box[1])  # 박스 안의 두 번째 아이템을 출력합니다.



> new_item
> item2
```
<br><br>


- `__delitem__`(self, index): 객체에서 인덱싱을 통해 특정 요소를 삭제하기 위한 메서드입니다.

```
class Box:
    def __init__(self):
        self.items = []  # 박스 안에 아이템을 넣습니다.

    def add_item(self, item):
        self.items.append(item)  # 아이템을 박스에 추가합니다.

    def __getitem__(self, index):
        return self.items[index]  # 박스 안의 아이템을 인덱스로 반환합니다.

    def __delitem__(self, index):
        del self.items[index]  # 박스 안의 아이템을 인덱스로 삭제합니다.

box = Box()  # 박스를 만듭니다.

box.add_item('item1')  # 아이템을 박스에 넣습니다.
box.add_item('item2')  # 또 다른 아이템을 박스에 넣습니다.

print(box[0])  # 박스 안의 첫 번째 아이템을 출력합니다.

del box[0]  # 박스 안의 첫 번째 아이템을 삭제합니다.

print(box[0])  # 박스 안의 첫 번째 아이템을 출력합니다.


> item1
> item2

```
- `['item1', 'item2']` 각각 두 값을 넣은뒤 첫번째 인덱스에 있는 원소를 삭제한다면, 리스트에 `item2` 만 남게되는 예제입니다.
<br><br>

---

<!--목차 & 다음으로 페이지 이동-->
[목차](https://github.com/Devcurve/Python/blob/main/README.md)<br>
[이전 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/File_read_write.md)<br>
<!--[다음 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/.md)-->
