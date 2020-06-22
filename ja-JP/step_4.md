## ゴール！

--- task ---

ゴールしたときに、音を鳴らしてゴールキーパーに「ゴール！」と言わせることができますか？

ボールがゴールキーパーにふれていない場合は、ゴールしたことになることをおぼえておきましょう。

![スクリーンショット](images/goalie-goal-test.png)

--- hints ---

--- hint ---

`ボールが`{:class="block3control"} `ゴールキーパーにふれて`{:class="block3sensing"}`いなければ、`{:class="block3control"} プログラムは`歓声 (かんせい) の音を鳴らし、 `{:class="block3sound"}<0>「ゴール」メッセージを送る</0>{:class="block3events"}必要があります。

`ゴールキーパーが「ゴール」メッセージを受け取ったら、`{:class="block3events"}`「ゴール！」`{:class="block3looks"}と言います。

--- /hint ---

--- hint ---

使うのはこのブロックです。

```blocks3
broadcast (goal v)

say [Goal!] for (1) seconds

when I receive [goal v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

コードは次のようになります。

![ボールのスプライト](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
broadcast (save v)
else
+ start sound (cheer v)
+ broadcast (goal v)
end
```

![ゴールキーパーのスプライト](images/goalie-sprite.png)

```blocks3
when I receive [goal v]
say [Goal!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
