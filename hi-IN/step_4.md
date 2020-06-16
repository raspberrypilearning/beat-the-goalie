## गोल!

--- task ---

क्या आप एक ध्वनि बजा सकते हैं और 'गोल' कहने के लिए अपने गोलकीपर को कोड कर सकते हैं कि गोल कब किया गया है?

याद रखें कि यदि गेंद गोल को छू नहीं रहा है तो एक गोल किया गया है।

![स्क्रीनशॉट](images/goalie-goal-test.png)

--- hints ---


--- hint ---

`If the football is not`{:class="block3control"} `touching the goalie`{:class="block3sensing"} your program should `start the cheer sound`{:class="block3sound"} और `broadcast a goal message`{:class="block3events"}.

`When the goalie receives the goal message`{:class="block3events"} it should `say goal`{:class="block3looks"}.

--- /hint ---

--- hint ---

आपको इन ब्लॉकों की जरुरत होगी:

```blocks3
broadcast (goal v)

say [Goal!] for (1) seconds

when I receive [goal v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

आपका कोड इस तरह दिखना चाहिए:

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
broadcast (save v)
else
+ start sound (cheer v)
+ broadcast (goal v)
end
```

![गोलकीपर स्प्राइट ](images/goalie-sprite.png)

```blocks3
when I receive [goal v]
say [Goal!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
