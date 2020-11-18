## 3-Dimensional effects

In this step you’re going to increase the sense of 3-dimensions, using the `looks`{:class="block3looks"} blocks to program the `size`{:class="block3looks"} of your sprites. You will also use `layers`{:class="block3looks"} to make your sprites appear in front or behind each other.

In the below example, the rocket is smaller than the bus and robot. The sprites either go in front of or behind each other. This enhances the sense of depth in the scene:

**Moon base**: [See inside](https://scratch.mit.edu/projects/447759319/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/447759319/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- task ---

Resize your sprites, where relevant, to increase the 3-dimensional effect.

--- collapse ---
---
title: Set the size of your sprites
---

**Numbers in a row**: [See inside](https://scratch.mit.edu/projects/445071529/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445071529/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

Use the `set size to ()%`{:class="block3looks"} block in your code to make your sprite decrease in size (less than 100%) when it sits towards the back or increase in size (more than 100%) when it sits towards the front. Some sprites can stay the same size. Make sure that you select the correct **Code tab** for each sprite before add new code:

``` blocks3
when green flag clicked
+set size to (120)%
```

``` blocks3
when green flag clicked
+set size to (80)%
```

--- /collapse ---

--- /task ---

--- task ---
Now program your sprites into layers.

--- collapse ---
---
title: Program your sprites in layers 
---

Have a look at how this project orders each of the sprites from front to back by using `Go backward a number of layers`{:class="block3looks"} to create the feeling that the number 6 is 'at the back', while the number 1 is 'at the front':

**Evening window scene**: [See inside](https://scratch.mit.edu/projects/437510050/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/437510050/?autostart=false" frameborder="0"></iframe>
</div>

Click on the **Code tab** of the sprite you want at the front and add a `go to front layer`{:class="block3looks"} block for the **front sprite**:

``` blocks3
when green flag clicked
go to [front v] layer
```

Now, using the `go backward (1) layers`{:class="block3looks"} to place the **next sprite** 1 layer behind the **front sprite**:

``` blocks3
when green flag clicked
go to [front v] layer
* Go [backward v] (1) layers
```

Allocate layers to other sprites. The value you use in the `go backward (1) layers`{:class="block3looks"} block will depend how many layers back you want each sprite to sit:

``` blocks3
when green flag clicked
go to [front v] layer
* Go [backward v] (2) layers
```

--- /collapse ---

--- /task ---

--- task ---

Animate your sprite by moving or changing its costumes.

--- collapse ---
---
title: Animate your sprite
---

Get your sprite moving:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

For more information, explore [Animate using motion](https://learning-admin.raspberrypi.org/en/projects/interactive-animation/3) in Challenge 1 Interactive animation.

--- /collapse ---

--- collapse ---
---
title: Animate your sprite
---

Get your sprite changing costumes:

```blocks3
when green flag clicked
forever
next costume
wait (0.3) seconds
```
If you want some  more information explore [Animate using looks](https://learning-admin.raspberrypi.org/en/projects/interactive-animation/5) in Challenge 1 Interactive animation.

--- /collapse ---

--- /task ---

--- save ---
