## Controle o goleiro

É muito fácil marcar um gol! Vamos permitir que um segundo jogador tente defender os gols.

--- task ---

Clique no seu ator __Goleiro__ e adicione este código para alterar a posição x do goleiro quando a seta para a esquerda for pressionada.

![ator goleiro](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Pressione a seta para a esquerda para testar seu novo código. Seu goleiro deve se mover para a esquerda.

![captura de tela](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Use blocos similares aos acima para fazer o __Goleiro__ se mover para a direita `quando a seta para a direita for pressionada`{:class="block3events"}.

--- hints ---

--- hint ---

Adicione blocos ao seu código para que ` quando a tecla seta para a direita for pressionada`{:class="block3events"}, a posição do __Goleiro__ `posição x é alterada por 10`{:class="block3motion"}.

--- /hint ---

--- hint ---

Você vai precisar desses blocos:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Seu código deve ficar assim:

![ator goleiro](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
