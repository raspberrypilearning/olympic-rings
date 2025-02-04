## Set up the rings

You will use the pen tool to draw the Olympic rings accurately. 

Pay close attention to where the rings cross each other and which ring sits on top at each overlap.

--- task ---

If you are working **online**, open the [starter project](https://scratch.mit.edu/projects/1048263697/){:target="_blank"} in Scratch.
 
If you are working **offline**, open the project [starter file](https://rpf.io/p/en/olympic-rings-go){:target="_blank"} in the Scratch offline editor. If you need to download and install Scratch, you can find it [here](https://scratch.mit.edu/download){:target="_blank"}.

--- /task ---

--- task ---

Click 'see inside'.

--- /task ---

Add the pen extension blocks.

--- task ---

Click on the extension menu in the bottom left corner.

![The extension menu](images/extension_menu.png)

Choose the pen extension blocks.

--- /task ---

--- task ---

Select the dot sprite.

--- /task ---

--- task ---

Drag out a `when green flag clicked`{:class="block3events"} block from the `Events`{:class="block3events"} blocks menu.

```blocks3
when flag clicked
```

--- /task ---

A variable will be used to control the five rings.

--- task ---

Create a `rings`{:class="block3variables"} variable and add a `set rings`{:class="block3variables"} block. 

```blocks3
when flag clicked
+set [rings v] to (0)
```

--- /task ---

Erase any previous drawing.

--- task ---

From the pen blocks, add an erase all block.

Add a block to set the pen size to 10.

```blocks3
when flag clicked
set [rings v] to (0)
+erase all
+set pen size to (10)
```

--- /task ---

The next section of code will repeat five times, one for each coloured ring. 

--- task ---

Add a repeat block. 

```blocks3
when flag clicked
set [rings v] to (0)
erase all
set pen size to (10)
+repeat (5)
```

--- /task ---

Each ring will be identified by a number from 1 to 5.

--- task ---

Add a block to change the `rings`{:class="block3variables"} variable by 1. 

```blocks3
when flag clicked
set [rings v] to (0)
erase all
set pen size to (10)
repeat (5)
+change [rings v] by (1)
```

--- /task ---

You need five clones (copies), because there are five rings.

--- task ---

Add a block to create a clone of itself and a wait block.


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

**Tip**: You can hide the variable on your screen. 
Right-click on the variable box on your screen and select hide.

--- save ---
