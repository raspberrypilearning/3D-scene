## Scenery

In the previous step you decided what you want your backdrop to be. Now it's time to think about how you want to create your **scenery**.

--- task ---

If you have chosen a backdrop that already has objects drawn in it,  you will not be able to animate the objects. Although these type of backdrops can work well, in an interactive animation it is easier to choose a simple backdrop or design your own background and add the objects you need in to your scene as **sprites** which you can then code. Creating some of the objects in your scene as sprites will give you more freedom as you go on to develop your project.

![Backdrop with furniture](images/challenge2-backdrop-bedroom.png){:width="400px"}

![Backdrop without furniture/objects](images/challenge2-backdrop-no-objects.png){:width="400px"}

![Sprite furniture/objects](images/challenge2-objects.png){:width="400px"}

Decide if you want to continue to use the Scratch backdrop you have chosen (changing the backdrop is easy), or if you want to design your own background or you may want to do a bit of both. Whether you are using a backdrop or making a background, for the rest of this project we will name the very back of your scene the **background**.

--- collapse ---
---

title: Design your own background

---

WRITE SRTUFF HERE! The background will the very back of your scene - it  might be sky, the sky and hills - you decide. 

--- /collapse ---

--- / task ---


--- task ---

In the real world the background if often static such as buildings or hills. In Scratch you can create some great effects by moving your backdr

Some sprites that don't move in the real world, such as a tree, are often static in Scratch. Some sprites which do move in the real world, such as a cat, often move in Scratch. But c


Scratch backdrop


Each sprite will `move`{:class="block3motion"} within a `forever`{:class="block3control"} block so that it keeps moving.

--- /task ---

Imagine
--- task ---

--- no-print ---

The **See inside** button in a Scratch project allows you to investigate the project's code. Click the below button to see inside 'Bouncing dragonfly'.

**Bouncing dragonfly**: [See inside](https://scratch.mit.edu/projects/435667657/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435667657/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

--- /task ---

--- task ---

To select your first sprite, click or tap on it under the Stage.

Click on the **Code** tab. 

--- /task ---

--- task ---

Add code to make your sprite bounce and/or spin around the Stage in the way you want it to. 

If you need a reminder about how to create your sprite's movement when it bounces on the edge of the Stage, then click the below **How to...**

--- collapse ---
---

title: Bounce across the Stage

---
--- no-print ---

**Girl moving across the Stage**: [See inside](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite bounce on the left-hand and right-hand edges of the Stage. Because the sprite rotates horizontally, it appears to flip when changing its direction when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

The `point in direction`{:class="block3motion"} block automatically points your sprite to the right (`90` degrees) when the green flag is clicked. If you change the number of degrees to `-90`, your sprite will point left.

Add a `set rotation  style`{:class="block3motion"} block and select the drop-down `left-right`{:class="block3motion"} so your sprite won't flip upside down when it bounces off the edge of the Stage.  

**Tip:** You can drag your sprite on the Stage to move it to the y (up-down) position that you want.

--- /collapse ---

--- collapse ---
---

title: Bounce up and down the Stage

---
--- no-print ---

**Girl jumping**: [See inside](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite bounce up and down the Stage when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Change the number of degrees in the `point in direction`{:class="block3motion"} block to `0` to make a sprite point upwards when the green flag is clicked.

Add a `set rotation  style`{:class="block3motion"} block and select the drop-down `don't rotate`{:class="block3motion"} block to stop your sprite rotating, even when it bounces.

**Tip:** You can drag your sprite around the Stage to move it to the x (left-right) position that you want.

--- /collapse ---

--- collapse ---
---

title: Bounce at an angle

---

--- no-print ---

**Football bouncing**: [See inside](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite appear to rotate randomly when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

If your sprite moves at `45` degrees, you will find it appears to bounces off the edge of the Stage in a random direction. Change the number of degrees in the `point in direction`{:class="block3motion"} block to `45` to make a sprite bounce all around.

Add a `set rotation  style`{:class="block3motion"} block and select the drop-down `all around`{:class="block3motion"} block, so your sprite will turn when it bounces off the edge of the Stage.  

--- /collapse ---

--- collapse ---
---

title: Spin around

---
--- no-print ---

**Bat spinning**: [See inside](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite spin when it is clicked:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Change the degrees by which your sprite turns to `1` within a `forever`{:class="block3control"} loop and your sprite will appear to spin.

**Tip:** If you don't add a `move`{:class="block3control"} block, your sprite will spin in the position its in. 

--- /collapse ---

--- collapse ---
---

title: Move in a circle

---

--- no-print ---

**Moon orbit**: [See inside](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite fly in a circle when it is clicked:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Change the degrees by which your sprite `moves`{:class="block3control"} to `1` and `turns`{:class="block3control"} to `1` within a `forever`{:class="block3control"} loop and your sprite will appear to move in a big circle.

**Tip**: If you want your sprite to always start in the centre of the Stage, you can add `go to x:(0) y: (0)`{:class="block3motion"} before the `forever`{:class="block3control"} block. 

--- /collapse --- 

--- /task ---

--- task ---
Remember to keep running your project to test it. Is the program working as you had planned?

It might take a few experiments to get suitable behaviour for your sprite.

You could:
+ Drag your sprite to a different starting location on the Stage.
+ Increase the number of steps in `move ( ) steps`{:class="block3motion"} to make your sprite move faster, or decrease it to move slower.
+ Change the number of degrees in `point in direction ( )`{:class="block3motion"} to change the direction that your sprite starts to move in. 
+ Change the number of degrees in `turn right`{:class="block3motion"} or `turn left`{:class="block3motion"} so that your sprite turns faster or slower. 
+ Combine `move ( ) steps`{:class="block3motion"} and `turn right`{:class="block3motion"} or `turn left`{:class="block3motion"} so that your sprite moves and turns. 
+ Experiment with `set rotation style [ ]`{:class="block3motion"} to make sure you understand what the different options do.

**Tip:** It's easier to identify issues if you make one change at a time and then run your program.

--- /task ---

--- save ---

