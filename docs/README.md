
# How to use calculator:
1. Run `python calculate.py`
2. Enter the figure name. Available are Circle, Square.
3. Enter the function: Area or Perimeter.
4. Enter figure sizes. Radius for circle, one side for square.
5. Get the answer!

# Math formulas
## Area
- Circle: `S = πR²`
- Rectangle: `S = ab`
- Square: `S = a²`
- Triangle: `S = sqrt(p * (p-a) * (p-b) * (p-c))` where p is semiperimeter

## Perimeter
- Circle: `P = 2πR`
- Rectangle: `P = 2a + 2b`
- Square: `P = 4a`
- Triangle: `P = a + b + c`

# Общее описание решения 
## Circle
Принимая радиус, функция возвращает площадь круга и его периметр.
## Square
Принимая сторону квадрата, функция возвращает площадь квадрата и его периметр.
## Triangle 
Принимая 3 стороны треугольника, функция возвращает площадь треугольника и его периметр.

# Описание каждый функции с примерами вызова
## Функции для квадрата
### area(a) - Нахождение площади квадрата
- Принимает число a (сторону квадрата), возвращает квадрат числа a
```python
def area(a):  
    return a * a   
```
### Пример вызова 
- a = 4, функция вернет число 16

### perimeter(a) - Нахождение периметра квадрата
- Принимает число a (сторону квадрата), возвращает число a умноженное на 4
```python
def perimeter(a):  
    return 4 * a   
```

### Пример вызова 
- a = 3, функция вернет число 12

## Функции для круга
### area(r) - Нахождение площади круга
- Принимает число r (радиус круга), возвращает число pi унможенное на квадрат r
```python
def area(r): 
    return math.pi * r * r
```
### Пример вызова
- r = 4, функция вернет число 50,24

### perimeter(r) - Нахождение периметра круга
- Принимает число r (радиус круга), возвращает число 2 умноженное на pi и на r (периметр круга)
```python
def perimeter(r): 
    return 2 * math.pi * r   
```
### Пример вызова
- r = 4, функция вернет число 25,12

## Функции для треугольника
### area(a, b, c) - Нахождение площади треугольника
- Принимает 3 числа a, b, c (стороны треугольника), возвращает сумму 3 чисел a, b, c деленных на два
```python
def area(a, b, c):
    return (a + b + c) / 2
```
### Пример вызова
- a = 4 | b = 3 | c = 4, функция вернет число 5,5

### perimeter(r) - Нахождение периметра круга
- Принимает 3 числа a, b, c (стороны треугольника), возвращает сумму 3 чисел a, b, c
```python
def perimeter(a, b, c):
    return a + b + c 
```
### Пример вызова
- a = 4 | b = 3 | c = 4, функция вернет число 11

# История изменения проекта 

``` git
86edb1c (origin/release) L-05: Update Docs. Add user agreement info
438b89a L-05: Add user agreement
6adb962 L-03: Docs added
3049431 (origin/feature) L-04: Add rectangle.py
b5b0fae (HEAD -> feature/documentation, origin/develop, develop) L-04: Update docs for calculate.py
d76db2a L-04: Add calculate.py
51c40eb L-04: Doc updated for triangle
d080c78 L-04: Triangle added
d078c8d (origin/main, origin/HEAD, main) L-03: Docs added
8ba9aeb L-03: Circle and square added

```