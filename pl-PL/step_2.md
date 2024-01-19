## Przenoszenie piłki

Zaprogramujmy piłkę, aby poruszała się po dolnej części sceny.

--- task ---

Otwórz startowy projekt 'Pokonaj bramkarza' w Scratch.

**Online**: otwórz startowy projekt [rpf.io/beat-the-goalie-on](https://rpf.io/beat-the-goalie-on){:target="_blank"}.

Jeśli masz konto Scratch, możesz wykonać kopię klikając **Remiks**.

**Offline**: otwórz [startowy projekt](https://rpf.io/p/en/beat-the-goalie-go){:target="_blank"} w edytorze offline.

Jeśli chcesz zainstalować edytor Scratch w wersji offline, możesz go pobrać ze strony [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

W projekcie startowym powinieneś zobaczyć tło bramki, piłkę i duszka bramkarza.

![startowy projekt](images/goalie-starter.png)

--- /task ---

--- task ---

Kliknij na duszka piłkarza. Dodaj ten kod, aby piłka poruszała się wzdłuż dolnej części ekranu, aż do naciśnięcia klawisz spacji.

![duszek piłki](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

Kliknij zieloną flagę, aby przetestować swój project. Twoja piłka powinna odbijać się wzdłuż dołu ekranu, aż do naciśnięcia klawisz spacji.

![zrzut ekranu](images/goalie-football-move-test.png)

--- /task ---

--- task ---

Dodaj ten kod do duszka bramkarza, aby piłka poruszała się w kierunku bramki po naciśnięciu klawisz spacji.

![duszek piłki](images/football-sprite.png)

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

Kliknij zieloną flagę, aby testować kod. Tym razem naciśnij klawisz spacji, a Twoja piłka powinna zmierzać do bramki.

![zrzut ekranu](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

Kliknij zieloną flagę, aby testować kod. Co się stanie, jeśli klikniesz flagę po raz drugi? Czy możesz rozwiązać ten problem?

--- hints ---

--- hint ---

Po `kliknięciu zielonej flag`{:class="block3events"} duszek będzie musiał `iść do`{:class="block3motion"} początku.

--- /hint ---

--- hint ---

Będziesz potrzebował tego bloku:

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

Twój kod powinien wyglądać tak:

![duszek piłki](images/football-sprite.png)

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

