## 3-Dimensional effects

In this step you’re going to use the `looks`{:class="block3looks"} blocks to program your sprites into `layers`{:class="block3looks"} to make them appear in front or behind each other. You will also change the `size`{:class="block3looks"} of sprites to increase the 3-dimensional effect. 

--- task ---
Notice how the rocket is smaller than the robot as well as higher up on the stage, creating the illusion of distance in this project. 

**Moon base**: [See inside](https://scratch.mit.edu/projects/447759319/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/447759319/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /task ---

--- task ---
Program your sprites into layers. You can simply program your sprites into two layers using the `front layer`{:class="block3looks"} and `back layer`{:class="block3looks"} blocks. Look at this project which brings the window frame to the front and puts everything else at the back when the green flag is clicked:

**Evening window scene**: [See inside](https://scratch.mit.edu/projects/437510050/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/437510050/?autostart=false" frameborder="0"></iframe>
</div>

--- collapse ---
---
title: Program your sprites with front and back layers 
---
Have a look at this project and notice how it uses only the front and back layers to order the sprites when you click them.

**Front and back layers:** [See inside](https://scratch.mit.edu/projects/448361272/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/448361272/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div> 

By using layers, you can create cool animated effects! This project uses only front and back layers to make the cats appear to circle the globe:

**Cats Around the World**: [See inside](https://scratch.mit.edu/projects/444530974/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/444530974/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>


Think of the sprites in your project and decide how you can have them move in front of (or behind!) different parts of your project, like the scenery or other sprites. 

Consider how many layers you will have, and add blocks that will allow your sprites to change between the layers as above.

**Tip: Treat layers like rows:** Think about layers as rows you can create to order your sprites from front to back and put them all in the right order. 

Once you know which sprites you would like to go on top, you can do this by having a sprite `go to front`{:class="block3looks"} or `go to back`{:class="block3looks"} layer, and stepping into the right position through the layers.

--- /collapse ---

You could also or create more complexity by programming your sprites from front to back in multiple layers:

--- collapse ---
---
title: Program your sprites with multiple layers
---
Have a look at how this project orders each of the sprites from front to back by using `Go backward X layers`{:class="block3looks"} to create the feeling that the number 6 is 'at the back', while the number 1 is 'at the front':

**Numbered Layers**: [See inside](https://scratch.mit.edu/projects/445055782/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445055782/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

To select your first sprite, click or tap on it under the Stage.

Click on the Code tab.

Use a `go to back layer`{:class="block3looks"} or a `go to front layer`{:class="block3looks"} block and either a `go forward 1 layer`{:class="block3looks"} or a `go backward 1 layer`{:class="block3looks"} block to create an order for your sprites and scenery.

You should get your sprite to go to the back (or front) layer and then move each sprite a concurrent number of layers at the start of your project:

Front sprite:
``` blocks3
when green flag clicked
go to [back v] layer
Go [forward v] (1) layers
```

Rear sprite:
``` blocks3
when green flag clicked
go to [back v] layer
Go [forward v] (2) layers
```

**Or:**

Front sprite:
``` blocks3
when green flag clicked
go to [front v] layer
Go [backward v] (1) layers
```

Rear sprite:
``` blocks3
when green flag clicked
go to [front v] layer
Go [backward v] (2) layers
```

--- /collapse ---

--- /task ---

--- task ---

Resize your sprites where relevant to increase the 3-dimensional effect.

--- collapse ---
---
title: Set the size of your sprites
---

**Numbers in a row**: [See inside](https://scratch.mit.edu/projects/445071529/editor){:target="_blank"}

Click or tap the backdrop to change the scenery for some added perspective!

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445071529/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>


Use the `change size by ()`{:class="block3looks"} or  `set size to ()%`{:class="block3looks"} block in your code to make your sprite shrink when it moves to the `back layer`{:class="block3looks"} and grow when it moves to the `front layer`{:class="block3looks"}!

Make your code change the size of your sprite when the layer changes by adding the `set size to ()%`{:class="block3looks"} like this:
``` blocks3
when green flag clicked
go to [front v] layer
+set size to (120)%
```

``` blocks3
when green flag clicked
go to [back v] layer
+set size to (80)%
```

``` blocks3
when green flag clicked
go to [back v] layer
+go [forward v] (1) layers
+change size by (20)
```

``` blocks3
when green flag clicked
go to [front v] layer
+go [back v] (1) layers
+change size by (-20)
```
Make sure that you are changing the right sprite each time, with the smallest sprite being the furthest back.
--- /collapse ---

--- /task ---

If you need a reminder about how to create your sprite’s movement, then explore [Animate using motion](https://github.com/raspberrypilearning/interactive-animation/edit/draft/en/step_4.md) in Challenge 1 Interactive animation.

--- save ---
