## Goal!

--- task ---

Can you play a sound and code your goalie to say 'Goal!' when a goal has been scored?

Remember that a goal has been scored if the ball is not touching the goalie.

![screenshot](images/goalie-goal-test.png)

--- hints ---
--- hint ---

Your code should look like this:

![football sprite](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
broadcast (save v)
else
+ start sound (cheer v)
+ broadcast (goal v)
end
```

![goalie sprite](images/goalie-sprite.png)

```blocks3
when I receive [goal v]
say [Goal!] for (1) seconds
```

--- /hint ---
--- /hints ---



--- /task ---
