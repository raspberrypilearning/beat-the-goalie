## 進球！

--- task ---

你可以在射門進球後，播放一段音效和程式讓你的守門員說'進球!'嗎？

請記住，如果足球沒有碰到守門員，則已經進球。

![截圖](images/goalie-goal-test.png)

--- hints ---

--- hint ---

`如果足球沒有`{:class="block3control"} `碰到守門員`{:class="block3sensing"} ，你的程式應該要`開始播放歡呼的音效`{:class="block3sound"} 並且 `廣播進球的消息`{:class="block3events"}。

`當守門員接收到進球的消息`{:class="block3events"} 他應該要 `說進球！`{:class="block3looks"}.

--- /hint ---

--- hint ---

你會需要這些積木：

```blocks3
broadcast (goal v)

say [Goal!] for (1) seconds

when I receive [goal v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

你的程式應該會像這樣：

![足球角色](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
broadcast (save v)
else
+ start sound (cheer v)
+ broadcast (goal v)
end
```

![守門員角色](images/goalie-sprite.png)

```blocks3
when I receive [goal v]
say [Goal!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
