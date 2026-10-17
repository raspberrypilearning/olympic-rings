## Dessiner les anneaux

Dans cette étape, tu définiras le point et la direction de départ de chacun des anneaux.

\--- task ---

Fais glisser un bloc `quand je commence comme un clone`{:class="block3events"} depuis le menu des blocs `Événements`{:class="block3events"}.

```blocks3
when I start as a clone
```

\--- /task ---

Assure-toi que le sprite est orienté dans la bonne direction pour commencer à dessiner.

\--- task ---

Ajoute un bloc `s'orienter à 90`{:class="block3motion"} depuis le menu des blocs `Mouvement`{:class="block3motion"}.

```blocks3
when I start as a clone
+point in direction (90)
```

\--- /task ---

Le clone créé avec la variable 1 suivra ce programme en premier.

\--- task ---

Ajoute un bloc `si alors`{:class="block3control"} depuis le menu des blocs `Contrôle`{:class="block3control"}.

Ajoute un bloc `=`{:class="block3operators"} depuis le menu `Opérateurs`{:class="block3operators"}.

Ajoute le rapporteur `anneaux`{:class="block3variables"} depuis le menu `Variables`{:class="block3variables"}.

Remplace le `50` par `1`.

```blocks3
when I start as a clone
point in direction (90)
+if <(rings) = (1)> then
```

\--- /task ---

\--- task ---

Ajoute des blocs pour définir la position de départ du premier clone.

Règle l'angle de départ.

Définis la couleur du stylo sur bleu (utilise le code hexadécimal #0078D0).

Ajoute un bloc pour mettre le stylo en position d'écriture.

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

L'anneau comportant la variable 2 est dessiné avec des caractéristiques différentes.

\--- task ---

Duplique le bloc si alors que tu viens de créer (ou fais glisser à nouveau les mêmes blocs).

Modifie le point de départ.

Modifie l'angle initial.

Modifie également la couleur sur jaune (utilise le code hexadécimal #FFB114).

```blocks3
+if <(rings) = (2)> then
go to x: (-13) y: (-13)
turn cw (78) degrees
set pen color to (#FFB114)
pen down
```

\--- /task ---

Fais maintenant la même chose pour l'anneau avec la variable 3.
**Astuce** : le code hexadécimal à utiliser pour le noir est #000000.

\--- task ---

Duplique à nouveau le bloc si alors.

Modifie le point de départ.

Modifie l'angle initial.

Modifie également la couleur sur noir (code hexadécimal #000000).

```blocks3
+if <(rings) = (3)> then
go to x: (-56) y: (19)
turn cw (-102) degrees
set pen color to (#000000)
pen down
```

\--- /task ---

Fais maintenant la même chose pour l'anneau avec la variable 4.
**Astuce** : le code hexadécimal à utiliser pour le vert est #00A651.

\--- task ---

```blocks3
+if <(rings) = (4)> then
go to x: (46) y: (28)
turn cw (-24) degrees
set pen color to (#00A651)
pen down
```

\--- /task ---

Fais maintenant la même chose pour l'anneau avec la variable 5.
**Astuce** : le code hexadécimal à utiliser pour le rouge est #F0282D.

\--- task ---

```blocks3
+if <(rings) = (5)> then
go to x: (85) y: (20)
turn cw (-102) degrees
set pen color to (#F0282D)
pen down
```

\--- /task ---

Maintenant que tu as défini le point de départ et la direction de chaque clone, il est temps de le faire dessiner !

\--- task ---

Ajoute un bloc « répéter » en bas.

Ajoute un bloc « avancer de 1 pas » et un bloc « tourner à droite ».

Cela permettra de dessiner un cercle.

Enfin, en dehors répéter en bas, ajoute un bloc « relever le stylo ».

```blocks3
repeat (360)
move (1) steps
turn cw (1) degrees
end
pen up
```

\--- /task ---

Teste ton code.

Tu devrais voir les anneaux olympiques dessinés !

\--- save ---
