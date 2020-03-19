## De bal verplaatsen

Laten we de bal programmeren om over de onderkant van het speelveld te bewegen.

--- task ---

Open het 'Beat the Goalie' Scratch-startproject.

**Online**: open het startproject op [rpf.io/beat-the-goalie-on](http://rpf.io/beat-the-goalie-on){: target = "_ blank"}.

Als je een Scratch account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline**: open het [startproject](http://rpf.io/p/en/beat-the-goalie-go){:target="_blank"} in de offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}.

In het startproject zou je een doelachtergrond, een voetbal en een keeper sprite moeten zien.

![startprojecten](images/goalie-starter.png)

--- /task ---

--- task ---

Klik op je voetbalsprite. Voeg deze code toe, zodat het voetbal langs de onderkant van het scherm beweegt totdat de spatiebalk wordt ingedrukt.

![voetbal sprite](images/football-sprite.png)

```blocks3
wanneer op de groene vlag wordt geklikt
herhaal tot < toets (spatiebalk v) ingedrukt?>
neem (10) stappen
keer om aan de rand
einde
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
wanneer op de groene vlag wordt geklikt
herhaal tot < toets (spatiebalk v) ingedrukt?>
neem (10) stappen
keer om aan de rand
einde
+ herhaal (15)
verander y met (10)
einde
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
ga naar x:(- 200) y:(- 140)
```

--- /hint ---

--- hint ---

Je code zou er als volgt uit moeten zien:

![voetbal sprite](images/football-sprite.png)

```blocks3
wanneer op de groene vlag wordt geklikt
+ ga naar x:(- 200) y:(- 140)
herhaal tot < toets (spatiebalk v) ingedrukt?>
neem (10) stappen
keer om aan de rand
einde
herhaal (15)
verander y met (10)
einde
```

--- /hint ---

--- /hints ---

--- /task ---

