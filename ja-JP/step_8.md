--- challenge ---

## チャレンジ: 自分で動かす
ボールが自動で左右に動くのではなく、プレーヤーが `a` と `d` キーでボールをコントロールできるようにすることはできますか？

そのためには、ボールを左右に動かすコードを削除 (さくじょ) する必要があります。

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

その後、キーが押されたときにボールを動かすコードを追加することができます。 役に立つコードブロックをいくつかしょうかいします。

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
