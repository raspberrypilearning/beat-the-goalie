## Gol!

--- task ---

Czy potrafisz odtwarzać dźwięk i zaprogramować bramkarza, aby powiedzieć "Gol!", gdy piłka wpadnie do bramki?

Pamiętaj, że bramka została zdobyta, jeśli piłka nie dotyka bramkarza.

![zrzut ekranu](images/goalie-goal-test.png)

--- hints ---

--- hint ---

`Jeśli piłka nie`{:class="block3control"} `dotykają bramkarza`{:class="block3sensing"} Twój program powinien `zagrać dźwięk radości`{:class="block3sound"} i `nadać komunikat o golu`{:class="block3events"}.

`Kiedy bramkarz otrzyma komunikat o golu`{:class="block3events"} powinien `powiedzieć gol`{:class="block3looks"}.

--- /hint ---

--- hint ---

Będziesz potrzebował tych bloków:

```blocks3
broadcast (gol v)

say [Gol!] for (1) seconds

when I receive [gol v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

Twój kod powinien wyglądać tak:

![duszek piłki](images/football-sprite.png)

```blocks3
if <touching (bramkarz v)> then
start sound (rattle v)
broadcast (obronione v)
else
+ start sound (cheer v)
+ broadcast (gol v)
end
```

![duszek bramkarza](images/goalie-sprite.png)

```blocks3
when I receive [gol v]
say [Gol!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
