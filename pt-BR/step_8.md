--- challenge ---

## Desafio: controle manual
Em vez de a bola se mover para a esquerda e direita automaticamente, você pode permitir que seu jogador controle a bola com as teclas `a` e `d` chaves?

Para fazer isso, você precisará remover o código para mover a bola para a esquerda e para a direita.

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

Você pode adicionar código para mover a bola quando as teclas forem pressionadas. Aqui estão alguns blocos de código para ajudá-lo:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
