## Goal!

--- task ---

Kun je een geluid laten afspelen en je keeper programmeren om te zeggen 'Goal!' wanneer er gescoord is?

Vergeet niet dat er gescoord is als de bal de keeper niet raakt.

![schermafbeelding](images/goalie-goal-test.png)

--- hints ---

--- hint ---

`Als de bal niet`{:class="block3control"} `de keeper`{:class="block3sensing"} aanraakt, moet je programma `het gejuich starten`{:class="block3sound"} en `een goal bericht uitzenden`{:class="block3events"}.

`Wanneer de keeper het goal bericht`{:class="block3events"} ontvangt, moet hij `goal zeggen`{:class="block3looks"}.

--- /hint ---

--- hint ---

Je hebt deze blokken nodig:

```blocks3
broadcast (goal v)

say [Goal!] for (1) seconds

when I receive [goal v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

Je code zou er als volgt uit moeten zien:

![voetbal sprite](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
broadcast (save v)
else
+ start sound (cheer v)
+ broadcast (goal v)
end
```

![keeper sprite](images/goalie-sprite.png)

```blocks3
when I receive [goal v]
say [Goal!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
