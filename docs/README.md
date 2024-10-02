# Geometric Lib
## Description
Бибилиотека Geometric Lib позволяет вычислить значение площади и периметра геометрических фигур (круг, прямоугольник, квадрат, треугольник).
Функции area и perimeter реализованы для каждой фигуры в отдельном файле.

### При написании функций использовались математические формулы
**Area**
- Circle: S = πR²
- Rectangle: S = ab
- Square: S = a²

**Perimeter**
- Circle: P = 2πR
- Rectangle: P = 2a + 2b
- Square: P = 4a

## Описание файлов.
### circle.py
В файле [circle.py](https://github.com/vasslin/geometric-lib/blob/new_features_465784/circle.py) реализованы функции поиска периметра и площади окружности с радиусом r:

```python
import math


def area(r):
    return math.pi * r * r


def perimeter(r):
    return 2 * math.pi * r
```

Функция **area(r)**:
Возвращает площадь окружности с радиусом r.

Параметры:
- r (float): радиус окружности

Возвращаемое значение:
- area(r) (float): площадь оружности радиуса r

Функция **perimeter(r)**:
Возвращает площадь окружности с радиусом r.

Параметры:
- r (float): радиус окружности

Возвращаемое значение:
- perimeter(r) (float): периметр оружности радиуса r

**Пример использования программы**
```python
area_of_circle = area(5) # возвращает площадь окружности с радиусом 5
perimeter_of_circle = perimeter(5) # возвращает периметр окружности срадиусом 5
```

### rectangle.py
В файле [rectangle.py](https://github.com/vasslin/geometric-lib/blob/new_features_465784/rectangle.py) реализованы функции поиска периметра и площади прямоугольника со сторонами a и b:

```python
def area(a, b):
    return a * b

def perimeter(a, b):
    return (a + b) * 2
```

Функция **area(a, b)**:
Возвращает площадь прямоугольника со сторонами a и b.

Параметры:
- a (float): величина первой стороны прямоугольника
- b (float): величина второй стороны прямоугольника

Возвращаемое значение:
- area(a, b) (float): площадь прямоугольника


Функция **perimeter(a, b)**:
Возвращает периметр прямоугольника со сторонами a и b.

Параметры:
- a (float): величина первой стороны прямоугольника
- b (float): величина второй стороны прямоугольника

Возвращаемое значение:
    area(a, b) (float): периметр прямоугольника



**Пример использования программы**
```python
area_of_rectangle = area(5, 2) # возвращает площадь прямоугольника со сторонами 5, 2
perimeter_of_rectangle = perimeter(5, 2) # возвращает периметр прямоугольника со сторонами 5, 2
```

### square.py
В файле [square.py](https://github.com/vasslin/geometric-lib/blob/new_features_465784/square.py) реализованы функции поиска периметра и площади квадрата со стороной a:

```python
def area(a):
    return a * a


def perimeter(a):
    return 4 * a

```

Функция **area(a)**:
Возвращает площадь квадрата со стороной a.

Параметры:
- a (float): величина  стороны квадрата

Возвращаемое значение:
- area(a) (float): площадь квадрата


Функция **perimeter(a)**:
Возвращает периметр квадрата со стороной a.

Параметры:
- a (float): величина  стороны квадрата

Возвращаемое значение:
- perimeter(a) (float): периметр квадрата



**Пример использования программы**
```python
area_of_square = area(5) # возвращает площадь квадрата со стороной 5
perimeter_of_square = perimeter(5) # возвращает периметр квадрата со стороной 5
```


### triangle.py
В файле [triangle.py](https://github.com/vasslin/geometric-lib/blob/new_features_465784/triangle.py) реализованы функции поиска периметра и площади треугольника с основанием a и высотой h:

```python
def area(a, h):
    return a * h / 2

def perimeter(a, b, c):
    return a + b + c

```

Функция **area(a)**:
Возвращает площадь треугольника с основанием a и высотой h.

Параметры:
- a (float): основание треугольника
- h (float): высота, проведенная к основанию

Возвращаемое значение:
- area(a, h) (float): площадь треугольника


Функция **perimeter(a)**:
Возвращает периметр треугольника со сторонами a, b, c.

Параметры:
- a, b, c (float): стороны треугольника

Возвращаемое значение:
- perimeter(a, b, c) (float): периметр треугольника


**Пример использования программы**
```python
area_of_triangle = area(5, 2) # возвращает площадь треугольника с основанием 5 и высотой 2
perimeter_of_triangle = perimeter(3, 4, 5) # возвращает периметр треугольника со сторонами 3, 4, 5
```

## История изменения проекта с хэшами коммитов
- commit c71567c4146853b2070ed26b986ac923b5648981 (HEAD -> new_features_465784, geometry-rep/new_features_465784)

Author: vaslin <vdolgovyazova@yandex.ru>

Date:   Sun Sep 8 10:58:48 2024 +0300

    Fixed a mistake in the rectangle perimeter and added triangle.py

- commit 5952c893d8f89da9218ce3aa3b44c4f6edc12668

Author: vaslin <vdolgovyazova@yandex.ru>

Date:   Sun Sep 8 10:27:46 2024 +0300

    Add rectangle.py

- commit d078c8d9ee6155f3cb0e577d28d337b791de28e2

Author: smartiqa <info@smartiqa.ru>

Date:   Thu Mar 4 14:55:29 2021 +0300

    L-03: Docs added

- commit 8ba9aeb3cea847b63a91ac378a2a6db758682460

Author: smartiqa <info@smartiqa.ru>

Date:   Thu Mar 4 14:54:08 2021 +0300

    L-03: Circle and square added
