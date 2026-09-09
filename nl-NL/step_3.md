## De ringen tekenen

In deze stap bepaal je het startpunt en de startrichting voor elk van de ringen.

\--- task ---

Sleep een `wanneer ik als kloon start`{:class="block3events"} blok uit het `Gebeurtenissen`{:class="block3events"} blokkenmenu.

```blocks3
when I start as a clone
```

\--- /task ---

Zorg ervoor dat de sprite in de juiste richting wijst voordat je begint met tekenen.

\--- task ---

Voeg een `richt naar 90 graden`{:class="block3motion"} blok toe vanuit het `Beweging`{:class="block3motion"} blokkenmenu.

```blocks3
when I start as a clone
+point in direction (90)
```

\--- /task ---

De kloon die met de variabelewaarde 1 wordt aangemaakt, zal dit programma als eerste uitvoeren.

\--- task ---

Voeg een `als dan`{:class="block3control"}-blok toe vanuit het menu met `Besturen`{:class="block3control"}-blokken.

Voeg een `=`{:class="block3operators"} blok toe vanuit het `Functies`{:class="block3operators"} menu.

Voeg de `ringen`{:class="block3variables"}-waarde toe vanuit het `Variabelen`{:class="block3variables"} menu.

Verander de `50` in `1`.

```blocks3
when I start as a clone
point in direction (90)
+if <(rings) = (1)> then
```

\--- /task ---

\--- task ---

Voeg blokken toe om de startpositie van de eerste kloon in te stellen.

Stel de beginhoek in.

Stel de penkleur in op blauw (gebruik hexcode #0078D0).

Voeg een blokj toe om de pen neer te zetten.

```blocks3
when I start as a clone
point in direction (90)
if <(rings) = (1)> then
+go to x: (-116) y: (-20)
+turn cw (156) degrees
+set pen color to (#0078D0)
+pen down
```

\--- /task ---

De ring met de variabelewaarde 2 wordt getekend met andere kenmerken.

\--- task ---

Dupliceer het als dan-blok dat je zojuist hebt gemaakt (of sleep dezelfde blokken er opnieuw in).

Wijzig de startlocatie.

Verander de beginhoek.

Verander de kleur naar geel (gebruik hexcode #FFB114).

```blocks3
+if <(rings) = (2)> then
go to x: (-13) y: (-13)
turn cw (78) degrees
set pen color to (#FFB114)
pen down
```

\--- /task ---

Doe nu hetzelfde voor de ring met de variabelewaarde 3.
**Tip**: De hexcode voor zwart is #000000.

\--- task ---

Dupliceer het als dan-blok opnieuw.

Wijzig de startlocatie.

Verander de beginhoek.

Verander de kleur naar zwart (hexcode #000000).

```blocks3
+if <(rings) = (3)> then
go to x: (-56) y: (19)
turn cw (-102) degrees
set pen color to (#000000)
pen down
```

\--- /task ---

Doe nu hetzelfde voor de ring met de variabelewaarde 4.
**Tip**: De hexcode voor groen is #00A651.

\--- task ---

```blocks3
+if <(rings) = (4)> then
go to x: (46) y: (28)
turn cw (-24) degrees
set pen color to (#00A651)
pen down
```

\--- /task ---

Doe nu hetzelfde voor de ring met de variabelewaarde 5.
**Tip**: De hexcode voor rood is #F0282D.

\--- task ---

```blocks3
+if <(rings) = (5)> then
go to x: (85) y: (20)
turn cw (-102) degrees
set pen color to (#F0282D)
pen down
```

\--- /task ---

Nu je de startlocatie en -richting voor elke kloon hebt ingesteld, is het tijd om hem te laten tekenen!

\--- task ---

Voeg onderaan een herhaalblok toe.

Voeg een blok 'neem 1 stappen' en een blok 'draai naar rechts' toe.

Hierdoor zal er een cirkel getekend worden.

Voeg ten slotte, buiten de herhaling onderaan, een pen op-blok toe.

```blocks3
repeat (360)
move (1) steps
turn cw (1) degrees
end
pen up
```

\--- /task ---

Test je code.

Je zou moeten zien hoe de Olympische ringen worden getekend!

\--- save ---
