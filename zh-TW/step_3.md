## 有進球嗎？

一旦球到達球門，就必須被做出判定。 __如果__球碰到守門員，那就是防守成功，__否則__是一個進球。

--- task ---

將這個程式添加到足球角色程式的末尾，讓您可以檢查足球是否觸碰到守門員。

![足球角色](images/football-sprite.png)

```blocks3
repeat (15)
change y by (10)
end
+if <touching (goalie v)> then
else
end
```

--- /task ---

--- task ---

`發出“嘎嘎”聲` {:class="block3sound"}`如果守門員防守成功` {:class="block3control"}。

![足球角色](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
+start sound (rattle v)
else
end
```

--- /task ---

--- task ---

您還可以向守門員廣播一則消息，讓他們可以告訴您足球已被守下。

守下足球後廣播“防守成功”消息。

![足球角色](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
+broadcast (save v)
else
end
```

--- /task ---

--- task ---

現在，您可以編碼守門員說“防守成功！”當他們收到消息時。

![守門員角色](images/goalie-sprite.png)

```blocks3
when I receive [save v]
say [Save!] for (1) seconds
```

--- /task ---

--- task ---

透過嘗試射門得分來測試您的程式。 如果您的守門員守下了足球，他們應該說“防守成功！”。

![截圖](images/goalie-save-test.png)

--- /task ---
