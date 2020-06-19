## But !

--- task ---

Peux-tu jouer un son et coder ton gardien pour dire « But ! » quand un but a été marqué ?

Rappelle-toi qu'un but a été marqué si le ballon ne touche pas le gardien.

![capture d'écran](images/goalie-goal-test.png)

--- hints ---


--- hint ---

`Si la balle de foot ne`{:class="block3control"} `touche pas le gardien`{:class="block3sensing"} ton programme devrait `commencer le son d'applaudissements`{:class="block3sound"} et `diffuser un message de but`{:class="block3events"}.

`Quand le gardien reçoit le message but`{:class="block3events"} il devrait `dire but`{:class="block3looks"}.

--- /hint ---

--- hint ---

Tu auras besoin de ces blocs :

```blocks3
broadcast (but v)

say [But !] for (1) seconds

when I receive [but v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

Ton code devrait ressembler à ceci :

![sprite de ballon de foot](images/football-sprite.png)

```blocks3
if <touching (Gardien v)> then
start sound (rattle v)
broadcast (sauvé v)
else
+ start sound (cheer v)
+ broadcast (but v)
end
```

![sprite gardien](images/goalie-sprite.png)

```blocks3
when I receive [but v]
say [But !] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
