## Faire bouger la balle de foot

Nous allons programmer la balle pour qu'elle se déplace en bas de la scène.

--- task ---

Ouvre le projet Scratch de démarrage « Battre le gardien de but ».

**Online**: open the starter project at [rpf.io/beat-the-goalie-on](https://rpf.io/beat-the-goalie-on){:target="_blank"}.

Si tu as un compte Scratch, tu peux en créer une copie en cliquant sur **Remix**.

**Offline**: open the [starter project](https://rpf.io/p/en/beat-the-goalie-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

Dans le projet de démarrage, tu devrais voir un arrière-plan de but, un ballon de foot et un sprite de gardien.

![projets de démarrage](images/goalie-starter.png)

--- /task ---

--- task ---

Clique sur ton sprite de ballon de foot. Ajoute ce code, de sorte que la balle de foot se déplace en bas de l'écran jusqu'à ce que la barre d'espace soit enfoncée.

![sprite de ballon de foot](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

Clique sur le drapeau vert pour tester ton projet. Ta balle de foot devrait rebondir en bas de l'écran jusqu'à ce que la barre d'espace soit enfoncée.

![capture d'écran](images/goalie-football-move-test.png)

--- /task ---

--- task ---

Ajoute ce code à ton sprite de ballon de foot, afin que la balle de foot se dirige vers le but après que la barre d'espace ait été pressée.

![sprite de ballon de foot](images/football-sprite.png)

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

Clique sur le drapeau vert pour tester ton code. Cette fois-ci, appuie sur la barre d'espace et ta balle de foot devrait aller vers le but.

![capture d'écran](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

Clique sur le drapeau vert pour tester ton code. Que se passe-t-il si tu cliques sur le drapeau une deuxième fois ? Peux-tu résoudre ce problème ?

--- hints ---

--- hint ---

Après que le `drapeau vert soit cliqué`{:class="block3events"} le sprite devra `aller`{:class="block3motion"} au début.

--- /hint ---

--- hint ---

Tu auras besoin de ce bloc :

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

Ton code devrait ressembler à ceci :

![sprite de ballon de foot](images/football-sprite.png)

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

