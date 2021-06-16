## Was het een doelpunt?

Zodra de bal het doel heeft bereikt, moet er een beslissing worden genomen. __Als__ de bal de keeper raakt, dan is het een redding, __anders__ is het een doelpunt.

--- task ---

Voeg deze code toe aan het einde van je voetbal sprite code, zodat je kunt controleren of de bal de keeper raakt.

![voetbal sprite](images/football-sprite.png)

```blocks3
repeat (15)
change y by (10)
end
+if <touching (goalie v)> then
else
end
```

--- /task ---

--- task ---

`Start het 'rammelaar'-geluid`{:class="block3sound"} `als de keeper de bal heeft tegengehouden`{:class="block3control"}.

![voetbal sprite](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
+start sound (rattle v)
else
end
```

--- /task ---

--- task ---

Je kunt ook een bericht naar de keeper sturen, zodat deze je kan vertellen dat de bal is tegengehouden.

Verzend een 'save' bericht wanneer de bal is tegengehouden.

![voetbal sprite](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
+broadcast (save v)
else
end
```

--- /task ---

--- task ---

Je kunt nu je keeper programmeren om 'Save!' te zeggen wanneer het bericht ontvangen wordt.

![keeper sprite](images/goalie-sprite.png)

```blocks3
when I receive [save v]
say [Save!] for (1) seconds
```

--- /task ---

--- task ---

Test je code door te proberen te scoren. Als je keeper de bal tegenhoudt, moet hij 'Save!' zeggen.

![schermafbeelding](images/goalie-save-test.png)

--- /task ---
