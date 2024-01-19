## Kontroluj bramkarza

Zdecydowanie zbyt łatwo jest strzelić gola! Pozwólmy, aby drugi gracz próbował obronić strzał.

--- task ---

Kliknij duszka swojego __bramkarza__ i dodaj ten kod, aby zmienić pozycję x bramkarza po naciśnięciu strzałki w lewo.

![duszek bramkarza](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

Naciśnij strzałkę w lewo, aby przetestować nowy kod. Twój bramkarz powinien przesunąć się w lewo.

![zrzut ekranu](images/goalie-move-left-test.png)

--- /task ---

--- task ---

Użyj bloków podobnych do tych, wyżej, aby __Bramkarz__ przesuwał się w prawo `kiedy klawisz strzałka w prawo jest naciśnięty`{:class="block3events"}.

--- hints ---

--- hint ---

Dodaj bloki do swojego kodu, aby `kiedy klawisz strzałka w prawo jest naciśnięty`{:class="block3events"}, __pozycja x zmienia się o 10__ dla duszka `bramkarza` {:class="block3motion"}.

--- /hint ---

--- hint ---

Będziesz potrzebował tych bloków:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

Twój kod powinien wyglądać tak:

![duszek bramkarza](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
