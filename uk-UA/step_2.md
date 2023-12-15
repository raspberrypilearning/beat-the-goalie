## Рух м’яча

Давай запрограмуємо м’яч, щоб він рухався вздовж низу сцени.

--- task ---

Відкрий початковий проєкт "Серія пенальті" у Скретч.

**Online**: open the starter project at [rpf.io/beat-the-goalie-on](https://rpf.io/beat-the-goalie-on){:target="_blank"}.

Якщо у тебе є обліковий запис Скретч, то ти можеш зробити копію проєкту, натиснувши **Ремікс**.

**Offline**: open the [starter project](https://rpf.io/p/en/beat-the-goalie-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

У початковому проєкті ти маєш бачити тло із воротами, а також спрайти воротаря та футбольного м’яча.

![початкові проєкти](images/goalie-starter.png)

--- /task ---

--- task ---

Клацни на спрайт м’яча. Додай такий код, щоб м’яч рухався вздовж низу сцени, доки не натиснуто клавішу "пропуск".

![спрайт футбольного м’яча](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

Натисни на зелений прапор, щоб перевірити свій проєкт. Твій м’яч має підстрибувати вздовж низу сцени, доки не натиснуто клавішу "пропуск".

![знімок екрана](images/goalie-football-move-test.png)

--- /task ---

--- task ---

Додай такий код, щоб спрайт м’яча летів до воріт після того, як натиснуто клавішу "пропуск".

![спрайт футбольного м’яча](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
+ repeat (15)
change y by (10)
end
```

--- /task ---

--- task ---

Натисни на зелений прапор, щоб перевірити свій код. Цього разу натисни клавішу "пропуск", і твій м’яч має полетіти до воріт.

![знімок екрана](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

Натисни на зелений прапор, щоб перевірити свій код. Що трапиться, якщо ти клацнеш на прапор удруге? Чи можеш ти вирішити проблему?

--- hints ---

--- hint ---

Після `натискання зеленого прапора`{:class="block3events"} спрайт має `переміститися`{:class="block3motion"} назад на початок.

--- /hint ---

--- hint ---

Тобі знадобиться такий блок:

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

Твій код повинен виглядати так:

![спрайт футбольного м’яча](images/football-sprite.png)

```blocks3
when green flag clicked
+ go to x:(-200) y:(-140)
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
repeat (15)
change y by (10)
end
```

--- /hint ---

--- /hints ---

--- /task ---

