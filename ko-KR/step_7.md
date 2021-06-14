## 골키퍼 조종하기

골을 넣는 것은 너무 쉽습니다! 두 번째 플레이어가 골을 세이브하도록 해 보겠습니다.

--- task ---

왼쪽 화살표를 눌렀을 때 골키퍼의 X축 위치를 바꾸기 위해 __골키퍼__ 스프라이트를 클릭하고 이 코드를 추가하세요.

![골키퍼 스프라이트](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

새 코드를 테스트하려면 왼쪽 화살표를 누르세요. 골키퍼는 왼쪽으로 움직여야 합니다.

![스크린샷](images/goalie-move-left-test.png)

--- /task ---

--- task ---

위와 비슷한 블록을 사용해 `오른쪽 화살표키가 눌렸을 때`{:class="block3events"} __골키퍼__를 오른쪽으로 움직이게 해보세요.

--- hints ---

--- hint ---

코드에 블록을 추가하여 `오른쪽 화살표 키를 눌렀을 때`{:class="block3events"}, __골키퍼의__ `X좌표를 10만큼 바꾸기`{:class="block3motion"}

--- /hint ---

--- hint ---

이 블럭들이 필요할겁니다.

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

다음과 같은 코드가 될 것입니다.:

![골키퍼 스프라이트](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
