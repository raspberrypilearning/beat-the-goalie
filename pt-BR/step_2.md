## Movendo a bola

Vamos programar a bola para percorrer a parte inferior do palco.

--- task ---

Abra o projeto inicial Scratch 'Vença o goleiro'.

**Online**: abra o projeto inicial em [scratch.mit.edu/projects/406770282](https://scratch.mit.edu/projects/406770282){:target="_blank"}.

Se você tiver uma conta do Scratch, você pode fazer uma cópia clicando em **Remix**.

**Offline**: abra o [projeto inicial](http://rpf.io/p/pt-BR/beat-the-goalie-go){:target="_blank"} no editor offline.

Se você precisar baixar e instalar o editor offline do Scratch, você pode encontrá-lo em [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}.

No projeto inicial, você deve ver um cenário de gol, uma bola e o goleiro.

![projetos iniciais](images/goalie-starter.png)

--- /task ---

--- task ---

Clique no seu ator bola. Adicione este código, para que bola se mova na parte inferior da tela até que a barra de espaço seja pressionada.

![ator bola](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

Clique na bandeira verde para testar seu projeto. Sua bola deve percorrer ao longo da parte inferior da tela até que a barra de espaço seja pressionada.

![captura de tela](images/goalie-football-move-test.png)

--- /task ---

--- task ---

Adicione este código ao seu ator bola, para que bola se mova em direção ao gol depois que a barra de espaço for pressionada.

![ator bola](images/football-sprite.png)

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

Clique na bandeira verde para testar seu código. Desta vez, pressione a barra de espaço e sua bola deve se mover em direção ao gol.

![captura de tela](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

Clique na bandeira verde para testar seu código. O que acontece se você clicar na bandeira uma segunda vez? Você pode resolver o problema?

--- hints ---


--- hint ---

Depois que a bandeira verde `bandeira verde é clicada`{:class="block3events"} o ator terá que `ir para`{:class="block3motion"} de volta ao início.

--- /hint ---

--- hint ---

Você vai precisar deste bloco:

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

Seu código deve ficar assim:

![ator bola](images/football-sprite.png)

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

