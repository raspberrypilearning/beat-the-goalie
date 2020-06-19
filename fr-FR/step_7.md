## Contrôler le gardien de but

C'est beaucoup trop facile de marquer un but ! Laissons un deuxième joueur essayer de sauver des buts.

--- task ---

Clique sur ton sprite __Gardien__ et ajoute ce code pour changer la position x du gardien lorsque tu appuies sur la flèche de gauche.

![sprite gardien](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Appuie sur la flèche de gauche pour tester ton nouveau code. Ton gardien devrait se déplacer vers la gauche.

![capture d'écran](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Utilise des blocs similaires à ceux ci-dessus pour que le __Gardien__ se déplace vers la droite `lorsque la touche fléchée droite est enfoncée`{:class="block3events"}.

--- hints ---


--- hint ---

Ajoute des blocs à ton code de sorte que `lorsque la touche fléchée droite est enfoncée`{:class="block3events"}, la position x du __Gardien__ `est modifiée de 10`{:class="block3motion"}.

--- /hint ---

--- hint ---

Tu auras besoin de ces blocs :

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Ton code devrait ressembler à ceci :

![sprite gardien](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
