**Шаг 1.** Создайте файл `words.txt`, где будут храниться английские слова. Например, такой:

```python
python
squirrel
flask
cucumbers
```

**Шаг 2.** В начале работы программа просит пользователя представиться и запоминает его имя.

```python
Программа: Введите ваше имя
Пользователь: Василий
```

**Шаг 3.** После этого программа выбирает первое слово из списка, перемешивает буквы и предлагает пользователю его отгадать.

```python
Программа: ****Угадайте слово: ontyph
Пользователь: python
Программа: Верно! Вы получаете 10 очков.
```

```python
Программа: ****Угадайте слово: ontyph
Пользователь: java
Программа: Неверно! Верный ответ – python.
```

**Шаг 4.** Когда слова закончились, программа заносит рекорд пользователя в файл `history.txt` с историей. Например:

```python
Игорь  200
Алексей  180
Василий  120
Игорь  200
Алексей  180
Василий  120
Игорь  200
Алексей  180
Василий  120
```

**Шаг 5.** В конце необходимо вывести статистику из прошлых игр, с учетом этой игры.

```python
Всего игр сыграно: 27
Максимальный рекорд: 200
```

В программе с помощью функций должны быть сделаны:

- чтение слов из файла,
- чтение топа игроков,
- запись в топ игроков.

Критерии проверки:

- [ ]  Использованы верные режимы чтения для файлов.
- [ ]  Файлы закрываются после работы.
- [ ]  Корректная работа с переносами строк.
- [ ]  Чтение и запись выполняются в функциях с корректными аргументами и операторами return.

Демонстрируемый навык:

- [ ]  Чтение файлов.