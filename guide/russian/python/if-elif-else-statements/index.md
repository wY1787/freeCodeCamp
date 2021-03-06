---
title: If Elif Else Statements

localeTitle: Операторы if / elif / else
---
## Операторы if / elif / else

Структура `if` / `elif` / `else` - это общий способ управления потоком программы, позволяющий выполнять определенные блоки кода в зависимости от значения некоторых данных. Если условие, следующее за ключевым словом `if` оценивается как `true` , блок кода будет выполняться: Обратите внимание, что скобки не используются до и после проверки условий, как на других языках.

```python
if True:
  print('If block will execute!')
```
_Обратите внимание, что скобки не используются до и после проверки условий, как это делается в других языках._

```python

x = 5

if x > 4:
  print("The condition was true!") #this statement executes
```

> **Подсказка** : Вы можете использовать **1** как альтернативу **True** и **0** вместо **False**
_Пример_:
```python
if 1:   # 1 принимается за true
  print('If block will execute!')
 ```
Вы можете дополнительно добавить ответ `else` который будет выполняться, если условие `false` :
```python

if not True:
  print('If statement will execute!')
else:
  print('Else statement will execute!')

```
Также вы можете посмотреть на этот пример:
```python

y = 3 
 
if y > 4: 
  print("I won't print!") #это значение не выведется 
else: 
  print("The condition wasn't true!") #выведется это значение 

```
_Обратите внимание, что нет никакого условия после ключевого слова `else` - оно ловит все ситуации, когда условие в предыдущем блоке вернуло `false`._

Можно проверить несколько условий , включив одну или несколько проверок `elif` после вашего первоначального оператора `if`, но из них будет выполнено только одно условие:

```python

z = 7 
 
if z > 8: 
  print("I won't print!") #это значение не выведется 
elif z > 5: 
  print("I will!") #выведется это значение
elif z > 6: 
  print("I also won't print!") #это значение не выведется 
else: 
  print("Neither will I!") #это значение не выведется 

```

_Обратите внимание, что будет выполняться только первое условие, которое вернуло `true` . Несмотря на то, что `z > 6` тоже`true` , блок `if/elif/else` завершается после первого истинного условия. Это означает, что `else` будет выполняться только в том случае, если ни одно из условий не было равно `true` ._

Мы также можем создавать вложенные `if` выражения для принятия решений. Перед тем как продолжить, обратитесь к <a href = 'https://guide.freecodecamp.org/python/code-blocks-and-indentation' target='\_blank' rel='nofollow'>руководству по отступам</a> .

Давайте возьмем пример нахождения числа, которое равно и больше, чем '10':

```python 
x = 34 
if x %  2 == 0:  # так вы можете создать комментарий, проверка на четность. 
  if x > 10: 
    print("This number is even and is greater than 10") 
  else: 
    print("This number is even, but not greater 10") 
else: 
  print ("The number is not even. So point checking further.") 

```

Это был простой пример для вложенных `if` выражений. Пожалуйста, не стесняйтесь изучать больше онлайн.

Хотя приведенные выше примеры просты, вы можете создавать более сложные условия, используя [логические сравнения](https://guide.freecodecamp.org/python/comparisons) и [логические операторы](https://guide.freecodecamp.org/python/boolean-operations) .

**_Встроенный оператор python if-else_**


Мы также можем использовать операторы if-else встроенные функции python Следующий пример должен проверить, больше ли число или равно 50, если да, верните True:

```python 
x = 89 
is_greater = True if x >= 50 else False 

 
print(is_greater) 
```

Вывод
```python
> 
True 
> 

```
