## 축구공 움직이기

무대 밑바닥을 가로질러 이동하도록 공을 코딩 해 보겠습니다.

--- task ---

'골키퍼를 이겨라' 스크래치 스타터 프로젝트를 엽니다.

**Online**: open the starter project at [rpf.io/beat-the-goalie-on](https://rpf.io/beat-the-goalie-on){:target="_blank"}.

스크래치 계정이 있는 경우 **Remix를 클릭** 하여 사본을 만들 수 있습니다.

**Offline**: open the [starter project](https://rpf.io/p/en/beat-the-goalie-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

스타터 프로젝트에서 골 배경, 축구공 및 골키퍼 스프라이트를 확인할 수 있습니다.

![스타터 프로젝트](images/goalie-starter.png)

--- /task ---

--- task ---

축구공 스프라이트를 클릭하세요. 스페이스바를 누를 때까지 축구공이 화면 하단을 따라 이동하도록 이 코드를 추가합니다.

![축구공 스프라이트](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

녹색 깃발을 눌러 시작합니다. 스페이스바를 누를 때까지 축구공이 화면 아래를 따라 튕겨야 합니다.

![스크린샷](images/goalie-football-move-test.png)

--- /task ---

--- task ---

이 코드를 축구공 스프라이트에 추가하면 스페이스바를 누른 후 축구공이 골문 쪽으로 이동합니다.

![축구공 스프라이트](images/football-sprite.png)

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

녹색 깃발을 눌러 코드를 테스트합니다. 이번에는 스페이스바를 누르면 축구공이 골문을 향해 움직여야 합니다.

![스크린샷](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

녹색 깃발을 눌러 코드를 테스트합니다. 깃발을 다시 클릭하면 어떻게 됩니까? 이 문제를 해결할 수 있습니까?

--- hints ---

--- hint ---

`초록 깃발을 클릭했을 때`{:class="block3events"} 후에, 스프라이트는 처음부터 `go to`{:class="block3events"}로 돌아가야 합니다.

--- /hint ---

--- hint ---

이 블록이 필요할겁니다.

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

다음과 같은 코드가 될 것입니다.:

![축구공 스프라이트](images/football-sprite.png)

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

