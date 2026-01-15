## De ringen opzetten

Je gebruikt het pen-gereedschap om de Olympische ringen nauwkeurig te tekenen.

Let goed op waar de ringen elkaar kruisen en welke ring bij elke overlapping bovenop ligt.

--- task ---

Als je **online** werkt, open dan het [startproject](https://scratch.mit.edu/projects/1048263697/){:target="_blank"} in Scratch.

Als je **offline** werkt, open dan het project [startbestand](https://rpf.io/p/nl-NL/olympic-rings-go){:target="_blank"} in de offline-editor van Scratch. Als je Scratch wilt downloaden en installeren, kun je het [hier](https://scratch.mit.edu/download){:target="_blank"} vinden.

--- /task ---

--- task ---

Klik op 'Bekijk van binnen'.

--- /task ---

Voeg de pen-uitbreidingsblokken toe.

--- task ---

Klik op het extensiemenu in de linkerbenedenhoek.

![Het uitbreidingsmenu](images/extension_menu.png)

Kies de pen-uitbreidingsblokken.

--- /task ---

--- task ---

Selecteer de dot-sprite.

--- /task ---

--- task ---

Sleep een `wanneer op groene vlag wordt geklikt`{:class="block3events"} blok uit het `Gebeurtenissen`{:class="block3events"} blokkenmenu.

```blocks3
when flag clicked
```

--- /task ---

Een variabele zal worden gebruikt om de vijf ringen te besturen.

--- task ---

Maak een variabele `ringen`{:class="block3variables"} aan en voeg een `maak ringen`{:class="block3variables"} blok toe.

```blocks3
when flag clicked
+set [rings v] to (0)
```

--- /task ---

Wis alle eerdere tekeningen.

--- task ---

Voeg vanuit de penblokken een wisblok toe.

Voeg een blok toe om de pengrootte op 10 in te stellen.

```blocks3
when flag clicked
set [rings v] to (0)
+erase all
+set pen size to (10)
```

--- /task ---

Het volgende stukje code wordt vijf keer herhaald, één keer voor elke gekleurde ring.

--- task ---

Voeg een herhaal blok toe.

```blocks3
when flag clicked
set [rings v] to (0)
erase all
set pen size to (10)
+repeat (5)
```

--- /task ---

Elke ring wordt aangeduid met een nummer van 1 tot en met 5.

--- task ---

Voeg een blok toe om de variabele `ringen`{:class="block3variables"} met 1 te veranderen.

```blocks3
when flag clicked
set [rings v] to (0)
erase all
set pen size to (10)
repeat (5)
+change [rings v] by (1)
```

--- /task ---

Je hebt vijf klonen (kopieën) nodig, omdat er vijf ringen zijn.

--- task ---

Voeg een blok toe om een kloon van zichzelf te maken en een wachtblok.

```blocks3
when flag clicked
set [rings v] to (0)
erase all
set pen size to (10)
repeat (5)
change [rings v] by (1)
+create clone of (myself v)
+wait (0.1) seconds
```

--- /task ---

**Tip**: Je kunt de variabele op je scherm verbergen.
Klik met de rechtermuisknop op het variabele vakje op je scherm en selecteer 'verdwijn'.

--- save ---
