--- challenge ---

## Défi : contrôle manuel
Au lieu de déplacer la balle vers la gauche et la droite automatiquement, peux-tu permettre à ton joueur de contrôler la balle avec les touches `q` et `d` ?

Pour ce faire, tu devras supprimer le code permettant de déplacer la balle vers la gauche et la droite.

```blocks3
when green flag clicked
forever
    go to x:(-200) y:(-140)
    repeat until <key (space v) pressed?>
-       move (10) steps
-       if on edge, bounce
    end
    repeat (15)
        change y by (10)
    end
    if <touching (Gardien v)> then
        start sound (rattle v)
        broadcast (sauvé v)
    else
        start sound (cheer v)
        broadcast (but v)
    end
end
```

Tu peux alors ajouter du code pour déplacer la balle lorsque les touches sont enfoncées. Voici quelques blocs de code pour t'aider :

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
