--- challenge ---

## Uitdaging: handmatige bediening
In plaats van dat de bal automatisch naar links en rechts beweegt, kun je je speler de bal laten besturen met de toetsen `a` en `d`?

Om dit te doen moet je de code verwijderen om de bal naar links en rechts te bewegen.

```blocks3
when green flag clicked
forever
	go to x:(-200) y:(-140)
	repeat until <key (space v) pressed?>
-		move (10) steps
-		if on edge, bounce
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

Je kunt vervolgens code toevoegen om de bal te verplaatsen wanneer de toetsen worden ingedrukt. Hier zijn enkele codeblokken om je te helpen:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
