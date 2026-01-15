## Mettre en place les anneaux

Tu vas utiliser l'outil Stylo pour dessiner les anneaux olympiques avec précision.

Fais bien attention à l’endroit où les anneaux se croisent et à quel anneau passe au-dessus à chaque intersection.

--- task ---

Si tu travailles **en ligne**, ouvre le [projet de démarrage](https://scratch.mit.edu/projects/1048263697/){:target="_blank"} dans Scratch.

Si tu travailles **hors ligne**, ouvre le [fichier de démarrage](https://rpf.io/p/fr-FR/olympic-rings-go){:target="_blank"} du projet dans l'éditeur hors ligne de Scratch. Si tu dois télécharger et installer Scratch, tu peux le trouver [ici](https://scratch.mit.edu/download){:target="_blank"}.

--- /task ---

--- task ---

Clique sur « voir à l'intérieur ».

--- /task ---

Ajoute les blocs d'extension Stylo.

--- task ---

Clique sur le menu Extension dans le coin inférieur gauche.

![Le menu Extension](images/extension_menu.png)

Choisis les blocs d'extension Stylo.

--- /task ---

--- task ---

Sélectionne le sprite point.

--- /task ---

--- task ---

Fais glisser un bloc `quand le drapeau vert est cliqué`{:class="block3events"} depuis le menu des blocs `Événements`{:class="block3events"}.

```blocks3
when flag clicked
```

--- /task ---

Une variable sera utilisée pour contrôler les cinq anneaux.

--- task ---

Crée une variable `anneaux`{:class="block3variables"} et ajoute un bloc `mettre anneaux`{:class="block3variables"}.

```blocks3
when flag clicked
+set [anneaux v] to (0)
```

--- /task ---

Efface tout dessin précédent.

--- task ---

À partir des blocs Stylo, ajoute un bloc « effacer tout ».

Ajoute un bloc pour mettre la taille du stylo à 10.

```blocks3
when flag clicked
set [anneaux v] to (0)
+erase all
+set pen size to (10)
```

--- /task ---

La section de code suivante se répétera cinq fois, une fois pour chaque anneau coloré.

--- task ---

Ajoute un bloc « répéter ».

```blocks3
when flag clicked
set [anneaux v] to (0)
erase all
set pen size to (10)
+repeat (5)
```

--- /task ---

Chaque anneau sera identifié par un numéro de 1 à 5.

--- task ---

Ajoute un bloc pour ajouter la variable `anneaux`{:class="block3variables"} à 1.

```blocks3
when flag clicked
set [anneaux v] to (0)
erase all
set pen size to (10)
repeat (5)
+change [anneaux v] by (1)
```

--- /task ---

Il te faut cinq clones (copies), car il y a cinq anneaux.

--- task ---

Ajoute un bloc pour créer un clone de lui-même et un bloc « attendre ».

```blocks3
when flag clicked
set [anneaux v] to (0)
erase all
set pen size to (10)
repeat (5)
change [anneaux v] by (1)
+create clone of (moi-même v)
+wait (0.1) seconds
```

--- /task ---

**Astuce** : tu peux cacher la variable sur ton écran.
Fais un clic droit sur la case de la variable à l'écran et sélectionne « Cacher ».

--- save ---
