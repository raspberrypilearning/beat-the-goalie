## Bestuur de keeper

Het is veel te gemakkelijk om een doelpunt te scoren! Laten we een tweede speler toestaan ballen tegen te houden.

--- task ---

Klik op je __Goalie__ sprite en voeg deze code toe om de x-positie van de keeper te wijzigen wanneer de linkerpijl wordt ingedrukt.

![keeper sprite](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Druk op de pijl naar links om je nieuwe code te testen. Je keeper moet naar links gaan.

![schermafbeelding](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Gebruik blokken vergelijkbaar met die hierboven om __Goalie__ naar rechts `te laten bewegen wanneer de pijltoets naar rechts wordt ingedrukt`{:class="block3events"}.

--- hints ---


--- hint ---

Voeg blokken toe aan de code zodat `wanneer de pijltoets naar rechts wordt ingedrukt`{:class="block3events"}, de positie van de __Goalie's__ `x wordt gewijzigd met 10`{:class="block3motion"}.

--- /hint ---

--- hint ---

Je hebt deze blokken nodig:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Je code zou er als volgt uit moeten zien:

![keeper sprite](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
