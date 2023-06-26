Пример работы программы:

```python
**Программа:**

Сегодня мы потренируемся расшифровывать азбуку Морзе
Нажмите Enter и начнем

**Пользователь:**

**Программа:**
Слово 1 – ... -. .- -.- .

**Пользователь:**
Snake

**Программа:**
Верно, Snake!
Слово 2 – - .. -. -.--

**Пользователь:**
Shiny

**Программа:**
Неверно, Tiny!
Слово 3 .-- . .-.. .-..  .--. .-.. .- -.-- . -..

**Пользователь:**
wellplayed
**Программа:**
Верно, wellplayed!

Всего задачек: 3
Отвечено верно: 2
Отвечено неверно: 1
```

**Обратите внимание, в рамках этой работы вам необходимо задокументировать код.**

**Шаг 0.** Составьте список английских слов и фраз, которые будете расшифровывать.

Например: code, bit, list, soul, next

**Шаг 1.** Напишите функцию morse_encode(word), которая переводит слова на английском языке в последовательности точек и тирe. Например

```python
morse_encode("little")
>>> .-.. .. - - .-.. .
```

```python
morse_encode("snake")
>>> ... -. .- -.- .
```

```python
morse_encode("wellplayed")
>>> .-- . .-.. .-.. .--. .-.. .- -.-- . -..
```

Словарь с кодами возьмите отсюда
https://gist.github.com/mohayonao/094c71af14fe4791c5dd

**Шаг 2.** Напишите функцию get_word() которая получает случайное слово из списка.

```python
get_word()
>>> bit
get_word()
>>> next
get_word()
>> lead
```

**Шаг 3.** Создайте в начале программы список answers = []. Напишите функцию `print_statistics(answers)` которая на основе списка answers типа [True, False, False, True, False] выводит статистику типа

```python
Всего задачек: 5
Отвечено верно: 2
Отвечено неверно: 3
```

**Шаг 4.**  При старте программы выведите приветственную информацию.

```python
Сегодня мы потренируемся расшифровывать морзянку.
Нажмите Enter и начнем
```

**Шаг 5.** Запустите цикл задавания вопросов. В одной игре – 5 вопросов.

В каждой итерации 

- получайте случайное слово с помощью ранее написанной функции
- кодируйте его с помощью ранее написанной функции
- выводите для пользователя
- получайте ввод
- сравнивайте с загаданным словом
- комментируйте верный или неверный ответ
- верность ответа складывайте в переменную answers.

Слова могут повторяться во время тренировки, это не страшно.

**Шаг 6.** Выведите статистику с помощью вызова ранее написанной функции

Протестируйте работу приложения и отправьте ссылку на colab

### Несколько рекомендаций по оформлению кода

1. Размещайте функции в начале кода, сразу после импортов, отделяя каждую функцию двумя пустыми строками, это требование PEP 8.

```python
# Верно

import random

def foo():
	pass 

def bar():
  pass
```

```python
# Неверно

def foo():
	pass 

import random

def bar():
  pass
```

1. Добавляйте docstring к каждой функции, размещайте пояснения именно там, а не в комментариях.

```python
# Верно

def get_random_word(words):
	""" 
  Получает случайное слово 
  из списка слов 
  """
  word = random.choice(words)
  return word

```

```python
# Неверно

# Получает случайное слово 
# из списка слов 

def get_random_word(words):

  word = random.choice(words)
  return word

```

**Критерии выполнения:**

- [ ]  Вопросы задаются корректно.
- [ ]  Все функции задокументированы (те добавлены комментарии или докстринги)
- [ ]  Слова преобразуются корректно.
- [ ]  Return используется корректно.
- [ ]  Статистика считается верно.
- [ ]  Функции написаны и работают как нужно.