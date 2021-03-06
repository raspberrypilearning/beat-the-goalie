## Керування воротарем

Забити год - занадто легко! Давай додамо ще одного гравця, який намагатиметься захистити ворота.

--- task ---

Клацни на спрайт __Воротар__ і додай такий код, щоб змінювати позицію x воротаря, коли натиснуто клавішу зі стрілкою вліво.

![спрайт воротаря](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Натисти клавішу зі стрілкою вліво, щоб перевірити свій код. Твій воротар має рухатися вліво.

![знімок екрана](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Використовуй блоки, подібні до вищенаведених, щоб __Воротар__ рухався вправо `коли клавішу "стрілка праворуч" натиснуто`{:class="block3events"}.

--- hints ---


--- hint ---

Додай блоки до свого коду, щоб `коли клавішу "стрілка праворуч" натиснуто`{:class="block3events"}, __Воротар__ `змінював x на 10`{:class="block3motion"}.

--- /hint ---

--- hint ---

Тобі знадобляться такі блоки:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Твій код повинен виглядати так:

![спрайт воротаря](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
