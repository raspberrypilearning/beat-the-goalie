## Controla al arquero

¡Es demasiado fácil anotar un gol! Dejemos que un segundo jugador intente y ataje goles.

--- task ---

Haz clic en tu objeto __Arquero__ y añade este código para cambiar la posición x del arquero cuando la flecha izquierda es presionada.

![objeto arquero](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Presiona la flecha izquierda para probar tu nuevo código. Tu arquero debe moverse hacia la izquierda.

![captura de pantalla](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Usa bloques similares a los de arriba para hacer que el __Arquero__ se mueva a la derecha `cuando la tecla de flecha derecha es presionada`{:class="block3events"}.

--- hints ---


--- hint ---

Añade bloques a tu código para que `cuando la tecla de flecha derecha es presionada`{:class="block3events"}, el __Arquero__ `cambia su posición x por 10`{:class="block3motion"}.

--- /hint ---

--- hint ---

Necesitarás estos bloques:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Tu código debería verse así:

![objeto arquero](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
