## Tor!

--- task ---

Kannst du einen Klang abspielen lasen und deinen Torwart so kodieren, dass er "Tor!" ruft wenn ein Tor erzielt wurde?

Denke daran, dass ein Tor erzielt wurde, wenn der Ball den Torwart nicht berührt.

![Screenshot](images/goalie-goal-test.png)

--- hints ---


--- hint ---

Wenn dein Fußball den Torwart nicht berührt (`falls wird Torwart berührt?, dann`{:class="block3control"} `sonst`{:class="block3sound"}), sollte dein Programm `spiele Klang cheer`{:class="block3sound"} (Jubel) starten und eine `sende Tor an alle`{:class="block3events"} Nachricht versenden.

Wenn der Torwart die Tor Nachricht empfängt (`wenn ich Tor empfange`{:class="block3events"}), soll er `sage Tor!`{:class="block3looks"} rufen.

--- /hint ---

--- hint ---

Du wirst diese Blöcke benötigen:

```blocks3
broadcast (Tor v)

say [Tor!] for (1) seconds

when I receive [Tor v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

Dein Code sollte so aussehen:

![Fußball-Sprite](images/football-sprite.png)

```blocks3
if <touching (Torwart v)> then
start sound (rattle v)
broadcast (Gehalten v)
else
+ start sound (cheer v)
+ broadcast (Tor v)
end
```

![Torwart-Sprite](images/goalie-sprite.png)

```blocks3
when I receive [Tor v]
say [Tor!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
