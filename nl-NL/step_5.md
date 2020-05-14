## Een timer toevoegen

Laten we een timer toevoegen, zodat de speler binnen 30 seconden zoveel mogelijk doelpunten moet maken.

--- task ---

`Maak een nieuwe variabele`{:class="block3variables"} genaamd `timer`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Klik op je __speelveld__ en voeg deze code toe om de `timer`{:class="block3variables"} in te stellen op 30 aan het begin van het spel.

![speelveld sprite](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
```

--- /task ---

--- task ---

Vervolgens moet je een `herhaal tot`{:class="block3control"} blok toevoegen, zodat de timer kan aftellen totdat deze op 0 komt.

![speelveld sprite](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
+repeat until <(timer :: variables) = [0]>
end
```

--- /task ---

--- task ---

Laat de timer aftellen 1 seconde totdat deze 0 bereikt.

![speelveld sprite](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
repeat until <(timer :: variables) = [0]>
+wait (1) seconds
+change [timer v] by (-1)
end
```

--- /task ---

--- task ---

Zodra de timer 0 heeft bereikt, moet je `het 'fluit'-geluid`{:class="block3sound"} laten afspelen en vervolgens het spel stoppen.

![speelveld sprite](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
repeat until <(timer :: variables) = [0]>
wait (1) seconds
change [timer v] by (-1)
end
+play sound (whistle v) until done
+stop [all v]
```

--- /task ---

--- task ---

Klik op de groene vlag om de code te testen. Je timer moet beginnen op 30 en eindigen op 0.

![schermafbeelding](images/goalie-timer-test.png)

Je kunt je timer instellen om op 10 te starten als je niet 30 seconden wilt wachten!

--- /task ---

--- task ---

Je hebt slechts de kans om 1 doelpunt te scoren! Om meer dan 1 kans te hebben, voeg een `herhaal`{:class="block3control"} blok aan de __voetbal__ code toe. Je kunt ook een `wacht`{:class="block3control"} blok tussen doelschoten toevoegen.

![voetbal sprite](images/football-sprite.png)

```blocks3
when green flag clicked
+forever
	go to x:(-200) y:(-140)
	repeat until <key (space v) pressed?>
		move (10) steps
		if on edge, bounce
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

--- /task ---

