## Gol!

--- task ---

Você consegue tocar um som e programar o seu goleiro para dizer 'Gol!' quando um gol for marcado?

Lembre-se de que um gol foi marcado se a bola não estiver tocando o goleiro.

![captura de tela](images/goalie-goal-test.png)

--- hints ---


--- hint ---

`Se a bola não estiver`{:class="block3control"} `tocando no goleiro`{:class="block3sensing"} seu programa deve `iniciar o som da torcida`{:class="block3sound"} e `transmita uma mensagem de gol`{:class="block3events"}.

`Quando o goleiro recebe a mensagem de gol`{:class="block3events"} deve `dizer Gol!`{:class="block3looks"}.

--- /hint ---

--- hint ---

Você vai precisar desses blocos:

```blocks3
broadcast (gol v)

say [Gol!] for (1) seconds

when I receive [gol v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

Seu código deve ficar assim:

![ator bola](images/football-sprite.png)

```blocks3
if <touching (Goleiro v)> then
start sound (rattle v)
broadcast (defesa v)
else
+ start sound (cheer v)
+ broadcast (gol v)
end
```

![ator goleiro](images/goalie-sprite.png)

```blocks3
when I receive [gol v]
say [Gol!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
