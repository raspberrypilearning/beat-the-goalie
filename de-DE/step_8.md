--- challenge ---

## Herausforderung: manuelle Steuerung
Kannst du deinem Spieler erlauben, den Ball mit den Tasten `a` und `d` zu steuern, anstatt sich automatisch nach links und rechts zu bewegen?

Dazu musst du den Code zum Bewegen des Balls nach links und rechts entfernen.

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
    if <touching (goalie v)> then
        start sound (rattle v)
        broadcast (save v)
    else
        start sound (cheer v)
        broadcast (goal v)
    end
end
```

Du kannst dann Code hinzufügen, um den Ball zu bewegen, wenn die Tasten gedrückt werden. Hier sind einige Codeblöcke, die Dir helfen:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
