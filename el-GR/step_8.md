--- challenge ---

## Πρόκληση: χειροκίνητος έλεγχος
Αντί η μπάλα να κινείται αυτόματα αριστερά και δεξιά, μπορείς να κάνεις τον παίκτη σου να ελέγχει την μπάλα με τα πλήκτρα `a` και `d`;

Για να το κάνεις αυτό, θα πρέπει να αφαιρέσεις τον κώδικα για την κίνηση της μπάλας αριστερά και δεξιά.

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
    if <touching (τερματοφύλακας v)> then
        start sound (rattle v)
        broadcast (απόκρουση v)
    else
        start sound (cheer v)
        broadcast (γκολ v)
    end
end
```

Στη συνέχεια, μπορείς να προσθέσεις κώδικα για να μετακινείς την μπάλα όταν πατάς τα πλήκτρα. Ακολουθούν ορισμένα χρήσιμα μπλοκ κώδικα για να σε βοηθήσουν:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
