--- challenge ---

## 도전과제: 수동으로 제어하기
공이 자동으로 좌우로 움직이는 대신, 플레이어가 `a`와 `d`키로 공을 제어하도록 할 수 있나요?

이렇게 하려면 공이 좌우로 움직이는 코드를 제거해야 합니다.

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

그런 다음 키를 눌렀을 때 공이 움직이는 코드를 추가할 수 있습니다. 다음은 도움이 될 코드 블록입니다.

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
