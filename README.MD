# Лабораторная работа №9(Вариант 3)
## Задание
Генератор простых чисел.
### Программный код
```
def f(n):
    def chisla(x):
        for i in range(2, int(x**0.5)+1):
            if x % i == 0: 
                return False #не является простым числом
        return True
    for i in range(2, n+1):
        if chisla(i):
            yield i #это ключевое слово, которое используется для возврата из функции с сохранением состояния её локальных переменных

for i in f(10):
    print(i)
```
### Результат работы программы
<image src = 1.png alt="результат программы">