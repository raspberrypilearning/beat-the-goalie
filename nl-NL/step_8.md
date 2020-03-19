--- challenge ---

## Uitdaging: handmatige bediening
In plaats van dat de bal automatisch naar links en rechts beweegt, kun je je speler de bal laten besturen met de toetsen `a` en `d`?

Om dit te doen moet je de code verwijderen om de bal naar links en rechts te bewegen.

```blocks3
wanneer op de groene vlag wordt geklikt
herhaal
    ga naar x:(- 200) y:(- 140)
    herhaal tot < toets (spatiebalk v) ingedrukt?>
- neem (10) stappen
- keer om aan de rand
    einde
    herhaal (15)
        verander y met (10)
    einde
    als <raak ik (goalie v) ?> dan
        start geluid (rattle v)
        zend signaal (save v)
    anders
        start geluid (cheer v)
        zend signaal (goal v)
    einde
einde
```

Je kunt vervolgens code toevoegen om de bal te verplaatsen wanneer de toetsen worden ingedrukt. Hier zijn enkele codeblokken om je te helpen:

```blocks3
verander x met (-5)

als <> dan 
einde

< toets (a v) ingedrukt?>
```

--- /challenge ---
