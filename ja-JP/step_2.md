## ボールを動かす

ボールにコードを入れて、ステージの下を動くようにしましょう。

--- task ---

「ゴールを決めろ」の基本 (きほん) の Scratch プロジェクトを開きます。

**オンライン**: [scratch.mit.edu/projects/410609028](https://scratch.mit.edu/projects/410609028){:target="_blank"}から基本のプロジェクトを開きます。

Scratch アカウントを持っている場合は、 **リミックス**ボタンをクリックしてプロジェクトをコピーできます。

**オフライン**: オフラインエディターで[基本のプロジェクト](https://rpf.io/p/ja-JP/beat-the-goalie-go){:target="_blank"}を開きます。

[rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}から Scratch オフラインエディターをダウンロードしてインストールできます。

基本のプロジェクトには、ゴールの背景 (はいけい) 、ボール、ゴールキーパーのスプライトがあります。

![基本のプロジェクト](images/goalie-starter.png)

--- /task ---

--- task ---

ボールのスプライトをクリックします。 このコードを追加 (ついか) して、スペースキーが押されるまで、ボールが画面の下にそって移動 (いどう) するようにします。

![ボールのスプライト](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

緑の旗をクリックしてゲームをテストします。 スペースキーが押されるまで、ボールが画面の下を左右に動き、端まで行ったらはね返ります。

![スクリーンショット](images/goalie-football-move-test.png)

--- /task ---

--- task ---

このコードをボールのスプライトに追加して、スペースキーが押されたあとにボールがゴールに向かって移動するようにします。

![ボールのスプライト](images/football-sprite.png)

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

緑の旗をクリックしてゲームをテストします。 今回はスペースキーを押すと、ボールがゴールに向かって移動します。

![スクリーンショット](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

緑の旗をクリックしてゲームをテストしましょう。 旗をもう一度クリックするとどうなりますか？ この問題をなおすことはできますか？

--- hints ---


--- hint ---

`緑の旗が押されたとき`{:class="block3events"}、スプライトは始めの位置 (いち) に `移動`{:class="block3motion"}する必要があります。

--- /hint ---

--- hint ---

使うのはこのブロックです。

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

コードは次のようになります。

![ボールのスプライト](images/football-sprite.png)

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

