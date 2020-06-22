## 控制守門員

進球太容易了！ 我們讓第二個玩家嘗試並守下足球。

--- task ---

點擊您的__ 守門員 __ 角色並添加此程式，讓玩家在按下左箭頭時可以更改守門員的x位置。

![守門員角色](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

按左方向鍵來測試您的新程式。 您的守門員應該向左移動。

![截圖](images/goalie-move-left-test.png)

--- /task ---

--- task ---

使用與上述相似的積木讓__守門員__往右移動`當玩家按下右方向鍵` {：class =“ block3events”}。

--- hints ---

--- hint ---

將積木添加到您的程式中，以便在` 玩家按下右方向鍵時` {：class =“ block3events”}，__ 守門員的__ ` x位置以10改變 ` {：class =“ block3motion”}。

--- /hint ---

--- hint ---

你會需要這些積木：

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

你的程式應該會像這樣：

![守門員角色](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
