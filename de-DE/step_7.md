## Steuere den Torwart

Es ist viel zu einfach, ein Tor zu erzielen! Lass einen zweiten Spieler versuchen, Tore zu halten.

--- task ---

Klicke auf dein __Torwart__-Sprite und füge diesen Code hinzu, um die x-Position des Torwarts zu ändern, wenn der linke Pfeiltaste gedrückt wird.

![Torwart-Sprite](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Drücke die linke Pfeiltaste, um deinen neuen Code zu testen. Dein Torwart sollte sich nach links bewegen.

![Screenshot](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Verwende Blöcke, ähnlich wie die oben genannten, um den __Torwart__ nach rechts zu bewegen `Wenn Taste Pfeil nach rechts gedrückt wird`{:class="block3events"}.

--- hints ---

--- hint ---

Füge deinem Code Blöcke hinzu, sodass sich `Wenn Taste Pfeil nach rechts gedrückt wird`{:class="block3events"}, der __Torwart__ `ändere x um 10`{:class="block3motion"} bewegt.

--- /hint ---

--- hint ---

Du wirst diese Blöcke benötigen:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Dein Code sollte so aussehen:

![Torwart-Sprite](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
