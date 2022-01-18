## De bal verplaatsen

Laten we de bal programmeren om over de onderkant van het speelveld te bewegen.

--- task ---

Open het 'Beat the Goalie' Scratch-startproject.

**Online**: open het startproject op [scratch.mit.edu/projects/395259876](https://scratch.mit.edu/projects/395259876){:target="_blank"}.

Als je een Scratch account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline**: open het [startproject](https://rpf.io/p/nl-NL/beat-the-goalie-go){:target="_blank"} in de offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

In het startproject zou je een doelachtergrond, een voetbal en een keeper sprite moeten zien.

![startprojecten](images/goalie-starter.png)

--- /task ---

--- task ---

Klik op je voetbalsprite. Voeg deze code toe, zodat de voetbal langs de onderkant van het scherm beweegt totdat de spatiebalk wordt ingedrukt.

![voetbal sprite](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

Klik op de groene vlag om je project te testen. Je voetbal zou langs de onderkant van het scherm moeten stuiteren totdat de spatiebalk wordt ingedrukt.

![schermafbeelding](images/goalie-football-move-test.png)

--- /task ---

--- task ---

Voeg deze code toe aan je voetbalsprite, zodat de voetbal richting het doel beweegt nadat de spatiebalk is ingedrukt.

![voetbal sprite](images/football-sprite.png)

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

Klik op de groene vlag om je code te testen. Druk deze keer op de spatiebalk en je voetbal zou naar het doel moeten gaan.

![schermafbeelding](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

Klik op de groene vlag om je code te testen. Wat gebeurt er als je een tweede keer op de vlag klikt? Kun jij het probleem oplossen?

--- hints ---


--- hint ---

Nadat op de groene vlag `is geklikt`{:class="block3events"} moet de sprite `teruggaan`{:class="block3motion"} naar het begin.

--- /hint ---

--- hint ---

Je hebt dit blok nodig:

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

Je code zou er als volgt uit moeten zien:

![voetbal sprite](images/football-sprite.png)

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

