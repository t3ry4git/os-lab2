# Лабораторна робота №2. Синхронізація процесів. Telegram: @t3ry444y
## Скріншот програми
![Alt text](https://github.com/73794449/os-lab2/blob/master/screenshot.png)

## Варіант 23(8)
### Об’єкт моделювання:
Автомат для продажу авіабілетів. 
Автомат приймає гроші (тут тільки одного визначеного номіналу – 1грн.) і видає здачу монетами вартістю до 1 грн. (1, 2, 5, 10, 25, 50 коп.). Сума здачі розраховується. Початкова кількість монет кожного номіналу задається  і становить: 
1 коп. – 50 шт., 2 коп. – 25 шт.,  
5 коп. – 20 шт.,  10 коп. – 15 шт.,  
25 коп. – 10 шт.,  50 коп. – 5 шт.,  
Введення запиту на продаж здійснюється шляхом вибору певного пункту меню:  

 0 – включити автомат

 1 – купити білет до Києва вартістю 28 коп.

 2 – білет до Москви вартістю 37 коп.

 3 – білет до Лондона вартістю 50 коп.

 4 – білет до Берлина вартістю 77 коп. 

 5 – білет до Парижа вартістю 91 коп.

Якщо здачу видати можливо, програма формує потрібний набір монет для здачі (також коригує банк монет) і формує сигнал на видачу. Якщо потрібних купюр для здачі не достає, формується відповідне повідомлення. Вимоги на видачу грошей надходять після чергового сеансу продажу або відмови.
### Кількість терміналів і процесів:
Модель автомата представити у вигляді двох взаємодіючих процесів А і В. Процес А визначає факти надходження вимог на продаж і потрібну суму здачі. Процес В очікує момент появи необхідності видати здачу і, якщо величина здачі відома, визначає кількість і номінали потрібних монет або неможливість видачі. 
### Засоби синхронізації: 
Для організації доступу до подільних ресурсів використати семафори.

## Оцінювання
Робота і захист: 20