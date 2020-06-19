## Έλεγξε τον τερματοφύλακα

Είναι πολύ εύκολο να πετύχεις γκολ! Ας επιτρέψουμε σε έναν δεύτερο παίκτη να προσπαθήσει να αποκρούσει τη μπάλα.

--- task ---

Κάνε κλικ στο αντικείμενο __Τερματοφύλακας__ και πρόσθεσε αυτόν τον κώδικα για να αλλάζει η θέση x του τερματοφύλακα όταν πατάς το αριστερό βέλος.

![αντικείμενο τερματοφύλακα](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Πάτησε το αριστερό βέλος για να ελέγξεις το νέο σου κώδικα. Ο τερματοφύλακας πρέπει να μετακινείται προς τα αριστερά.

![στιγμιότυπο οθόνης](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Χρησιμοποίησε παρόμοιες εντολές με τις παραπάνω για να κάνεις τον __τερματοφύλακα__ να μετακινείται προς τα δεξιά `όταν πατηθεί πλήκτρο δεξί βέλος`{:class="block3events"}.

--- hints ---

--- hint ---

Πρόσθεσε μπλοκ στον κώδικά σου, ώστε `όταν πατηθεί το δεξί βέλος`{:class="block3events"}, ο __τερματοφύλακας__ `αλλάζει τη θέση x κατά 10`{:class="block3motion"}.

--- /hint ---

--- hint ---

Θα χρειαστείς αυτά τα μπλοκ:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Ο κώδικας θα πρέπει να μοιάζει κάπως έτσι:

![αντικείμενο τερματοφύλακα](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---