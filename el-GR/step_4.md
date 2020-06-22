## Γκολ!

--- task ---

Μπορείς να παίξεις έναν ήχο και να προγραμματίσεις τον τερματοφύλακα να λέει "Γκολ!" όταν έχει σημειωθεί ένα γκολ;

Θυμήσου ότι ένα γκολ μετριέται εάν η μπάλα δεν αγγίζει τον τερματοφύλακα.

![στιγμιότυπο οθόνης](images/goalie-goal-test.png)

--- hints ---


--- hint ---

`Εάν η μπάλα δεν`{:class="block3control"}`αγγίζει τον τερματοφύλακα`{:class="block3sensing"} το πρόγραμμά σου θα πρέπει να `παίξει τον ήχο 'cheer'`{:class="block3sound"} και να `μεταδώσει το μήνυμα 'γκολ'`{:class="block3events"}.

`Όταν ο τερματοφύλακας λάβει το μήνυμα 'γκολ'`{:class="block3events"} θα πρέπει να `πει 'Γκολ!'`{:class="block3looks"}.

--- /hint ---

--- hint ---

Θα χρειαστείς αυτά τα μπλοκ:

```blocks3
broadcast (γκολ v)

say [Γκολ!] for (1) seconds

when I receive [γκολ v]

start sound (cheer v)
```

--- /hint ---

--- hint ---

Ο κώδικάς σου θα πρέπει να μοιάζει κάπως έτσι:

![αντικείμενο μπάλας](images/football-sprite.png)

```blocks3
if <touching (τερματοφύλακας v)> then
start sound (rattle v)
broadcast (απόκρουση v)
else
+ start sound (cheer v)
+ broadcast (γκολ v)
end
```

![αντικείμενο τερματοφύλακα](images/goalie-sprite.png)

```blocks3
when I receive [γκολ v]
say [Γκολ!] for (1) seconds
```

--- /hint ---



--- /hints ---


--- /task ---
