## タイマーを追加 (ついか) する

タイマーを追加して、30秒以内にできるだけたくさんゴールを決めなければならないようにしましょう。

--- task ---

`タイマー`{:class="block3variables"}という`新しい変数`{:class="block3variables"} (へんすう) を作ります。

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

__ステージ__をクリックします。このコードを追加して、ゲームが始まったときに`タイマー`{:class="block3variables"}を30にします。

![ステージのスプライト](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
```

--- /task ---

--- task ---

次に、`まで繰り返す`{:class="block3control"} (くりかえす) ブロックを追加する必要があります。このブロックを使うと、タイマーが0になるまで動かすことができます。

![ステージのスプライト](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
+repeat until <(timer :: variables) = [0]>
end
```

--- /task ---

--- task ---

タイマーを0になるまで1秒ごとに1ずつへらしていきましょう。

![ステージのスプライト](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
repeat until <(timer :: variables) = [0]>
+wait (1) seconds
+change [timer v] by (-1)
end
```

--- /task ---

--- task ---

タイマーが0になったら、`「ホイッスル」という音を鳴らして`{:class="block3sound"}ゲームを終わらせましょう。

![ステージのスプライト](images/stage-sprite.png)

```blocks3
when green flag clicked
set [timer v] to [30]
repeat until <(timer :: variables) = [0]>
wait (1) seconds
change [timer v] by (-1)
end
+play sound (whistle v) until done
+stop [all v]
```

--- /task ---

--- task ---

緑の旗をクリックしてゲームをテストします。 タイマーは30で始まり、0で終わります。

![スクリーンショット](images/goalie-timer-test.png)

30秒も待ちたくない場合は、タイマーを10から始まるようにかえることができます！

--- /task ---

--- task ---

ゴールを決めるチャンスが1回しかありません！ チャンスをふやすには、`ずっと`{:class="block3control"}ブロックを__ボール__のコードのまわりに追加します。 また、シュートとシュートの間に`待つ`{:class="block3control"}ブロックを追加することもできます。

![ボールのスプライト](images/football-sprite.png)

```blocks3
when green flag clicked
+forever
    go to x:(-200) y:(-140)
    repeat until <key (space v) pressed?>
        move (10) steps
        if on edge, bounce
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

--- /task ---

