## Draw the rings

--- task ---

Drag out a `when I start as a clone`{:class="block3events"} block from the `Events`{:class="block3events"} blocks menu.

```blocks3
when I start as a clone
```

--- /task ---

Make sure the sprite is facing the correct direction to start drawing.

--- task ---

Add a `point in direction 90`{:class="block3motion"} block from the `Motion`{:class="block3motion"} blocks menu.

```blocks3
when I start as a clone
+point in direction (90)
```

--- /task ---

The clone that is created with the variable of 1 will follow this program first.

--- task ---

Add an `if then`{:class="block3events"} block from the `Events`{:class="block3events"} blocks menu.

Add an `=`{:class="block3operators"} block from the `Operators`{:class="block3operators"} menu.

Add the `rings`{:class="block3variables"} reporter from the `Variables`{:class="block3variables"} menu.

Change the `50` to `1`. 

```blocks3
when I start as a clone
point in direction (90)
+if <(rings) = (1)> then
```

--- /task ---

--- task ---

Add blocks to set the starting position of the first clone.

Set the angle to start with. 

Set the pen colour to blue (use hex code #0078D0).

Add a block to put the pen down.

```blocks3
when I start as a clone
point in direction (90)
if <(rings) = (1)> then
+go to x: (-116) y: (-20)
+turn cw (156) degrees
+set pen color to (#0078D0)
+pen down
```

--- /task ---

The ring with the variable of 2 is drawn with different characteristics.

--- task ---

Duplicate the if-then block you just created (or drag in the same blocks again). 

Change the starting location.

Change the angle that it starts with. 

Also change the colour to yellow (use hex code #FFB114).

```blocks3
+if <(rings) = (2)> then
go to x: (-13) y: (-13)
turn cw (78) degrees
set pen color to (#FFB114)
pen down
```

--- /task ---

Now do the same for the ring with the variable of 3.
**Tip**: The hex code to use for black is #000000.

--- task ---

Duplicate the if-then block again. 

Change the starting location. 

Change the angle that it starts with. 

Also change the colour to black (hex code #000000).

```blocks3
+if <(rings) = (3)> then
go to x: (-56) y: (19)
turn cw (-102) degrees
set pen color to (#000000)
pen down
```

--- /task ---

Now do the same for the ring with the variable of 4.
**Tip**: The hex code to use for green is #00A651.

--- task ---

```blocks3
+if <(rings) = (4)> then
go to x: (46) y: (28)
turn cw (-24) degrees
set pen color to (#00A651)
pen down
```

--- /task ---

Now do the same for the ring with the variable of 5.
**Tip**: The hex code to use for red is #F0282D.

--- task ---

```blocks3
+if <(rings) = (5)> then
go to x: (85) y: (20)
turn cw (-102) degrees
set pen color to (#F0282D)
pen down
```

--- /task ---

Now that you have set the starting location and direction for each clone, it is time to make it draw! 

--- task ---

Add a repeat block at the bottom. 

Add a move 1 step block and a turn right block. 

This will make it draw a circle.

Finally, outside of the repeat at the bottom, add a pen up block.

```blocks3
repeat (360)
move (1) steps
turn cw (1) degrees
end
pen up
```

--- /task ---

Test your code. 

You should see the Olympic rings being drawn!


--- save ---
