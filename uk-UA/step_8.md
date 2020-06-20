--- challenge ---

## Завдання: ручне керування
Замість автоматичного переміщення м’яча вліво-вправо, чи можеш ти дати можливіть гравцеві керувати ним за допомогою клавіш `a` та `d`?

Щоб це зробити, тобі треба видалити код для руху м’яча вліво-вправо.

```blocks3
when green flag clicked
forever
    go to x:(-200) y:(-140)
    repeat until <key (space v) pressed?>
-       move (10) steps
-       if on edge, bounce
    end
    repeat (15)
        change y by (10)
    end
    if <touching (goalie v)> then
        start sound (rattle v)
        broadcast (save v)
    else
        start sound (cheer v)
        broadcast (goal v)
    end
end
```

Далі ти можеш додати код, щоб рухати м’яч, коли натиснуто відповідні клавіші. Ось деякі блоки коду, які стануть тобі в пригоді:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
