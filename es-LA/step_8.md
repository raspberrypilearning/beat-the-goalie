--- challenge ---

## Desafío: control manual
En lugar de que la pelota se mueva automáticamente a la izquierda y la derecha, ¿puedes permitir que tu jugador controle la pelota con las teclas `a` y `d`?

Para hacer esto, necesitarás eliminar el código para mover la pelota hacia la izquierda y hacia la derecha.

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
    if <touching (arquero v)> then
        start sound (rattle v)
        broadcast (atajar v)
    else
        start sound (cheer v)
        broadcast (gol v)
    end
end
```

Entonces puedes agregar código para mover la pelota cuando las teclas son presionadas. Aquí hay algunos bloques de código para ayudarte:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
