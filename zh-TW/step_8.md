--- challenge ---

## 挑戰：手動控制
除了讓足球左右自動移動之外，你能用 `a` 和`d` 按鍵讓你的球員控制足球嗎？

為此，你需要刪除讓足球左右移動的程式。

```blocks3
when green flag clicked
forever
    go to x:(-200) y:(-140)
    repeat until <key (space v) pressed?>
-       move (10) steps
-       if on edge, bounce
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

然後，您可以加入程式讓玩家在按下按鍵時移動足球。 這些程式積木可以幫助你：

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
