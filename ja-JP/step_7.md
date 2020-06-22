## ゴールキーパーを動かす

あまりにもかんたんにゴールできてしまいます！ もう一人のプレイヤーがシュートをふせげるようにしてみましょう。

--- task ---

__ゴールキーパー__のスプライトをクリックして、左矢印キーが押されたときにゴールキーパーのx座標 (ざひょう) をかえるコードを追加します。

![ゴールキーパーのスプライト](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

左矢印キーを押して、新しいコードをテストします。 ゴールキーパーが左に動くはずです。

![スクリーンショット](images/goalie-move-left-test.png)

--- /task ---

--- task ---

上記のようなブロックを使って、__ゴールキーパー__を`右矢印キーが押されたときに`{:class="block3events"}右に動かします。

--- hints ---

--- hint ---

`右向き矢印キーが押されたとき`{:class="block3events"}、__ゴールキーパーの__`x座標が10ずつかわります`{:class="block3motion"}。

--- /hint ---

--- hint ---

使うのはこのブロックです。

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

コードは次のようになります。

![ゴールキーパーのスプライト](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
