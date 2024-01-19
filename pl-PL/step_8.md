--- challenge ---

## Wyzwanie: sterowanie ręczne
Zamiast piłki poruszającej się automatycznie w lewo i prawo, możesz pozwolić swojemu graczowi kontrolować piłkę za pomocą klawiszy `a`i`d`?

Aby to zrobić, musisz usunąć kod do przesuwania piłki w lewo i prawo.

```blocks3
when green flag clicked
forever
    go to x:(-200) y:(-140)
    repeat until <key (spacja v) pressed?>
-       move (10) steps
-       if on edge, bounce
    end
    repeat (15)
        change y by (10)
    end
    if <touching (bramkarz v)> then
        start sound (rattle v)
        broadcast (obronione v)
    else
        start sound (cheer v)
        broadcast (gol v)
    end
end
```

Następnie możesz dodać kod, aby przesunąć piłkę po naciśnięciu klawiszy. Oto kilka bloków kodu, które mogą Ci pomóc:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
