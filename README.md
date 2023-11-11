Нужно написать программу, которая будет рассчитывать количество дней в году.
Зачем это бывает нужно? Варианты бывают разные: например, для расчета продолжительности долгосрочных проектов в днях или чтобы
узнать, сколько дней потребуется для космической экспедиции на Марс.
Для расчета количества дней в году требуется знать несколько правил:
- В високосном году 366 дней, в обычном 365.
- Високосный год — это год, номер которого делится без остатка на 400 (например 2000 или 2400), либо делится на 4 но не делится на 100 (например 2008, 2096, но не 2100).

### Схема работы программы
1. Вывод сообщения в консоли `Введите год в формате "yyyy"`.
2. Ввод года в формате `yyyy` (например 2004).
3. Чтение значения из консоли и расчет количества дней.
4. Результат работы программы: напечатать в консоли количество дней в году `Количество дней 365` или `Количество дней 366`.

### Пример работы программы 1
```text
Введите год в формате yyyy: 2000 <нажмите enter>
Количество дней 366
```

### Пример работы программы 2
```text
Введите год в формате yyyy: 2018 <нажмите enter>
Количество дней 365
```
### Проверка високосности
Как проверить, високосный ли год? Для этого сначала надо проверить делимость на 400, используя year % 400 == 0. Специальный оператор % - возвращает остаток от деления. Результат вычисления будет равен 0, только если число делится нацело, иначе вернется остаток от деления. Если год делится на 400 без остатка, значит в нем точно 366 дней. Если нет, то — аналогично проверить делимость на 100: если год делится на 100, то в нем точно 365 дней. И наконец, если год не делится ни на 400, ни на 100, то проверяем делимость на 4: если делится, — то — 366 дней, иначе — 365.
