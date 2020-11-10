## Distance and depth

Now, you’re going to use the `looks`{:class="block3looks"} blocks to program your sprites into 'layers'{:class="block3looks"} to make them appear in front or behind each other. You will also change the `size`{:class="block3looks"} of sprites in relation to each other. 

**Cars in Space**: [See inside](https://scratch.mit.edu/projects/447759319/editor){:target="_blank"}

Click or tap the backdrop to change the scene!

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/447759319/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- task ---
Now, program your sprites into layers by programming them. You can keep it simple and just use the `front layer`{:class="block3looks"} and `back layer`{:class="block3looks"} if you like, or create multiple layers for more complex projects.

--- collapse ---
---
title: Program your sprites into layers
---

This project uses front and back layers to make the cats appear to circle the globe:

**Cats Around the World**: [See inside](https://scratch.mit.edu/projects/444530974/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/444530974/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>


Think of the sprites in your project and decide how you can have them move in front of (or behind!) different parts of your project, like the scenery or other sprites. 

Consider how many layers you will have, and add blocks that will allow your sprites to change between the layers as above.

**Tip: Treat layers like rows:** Think about layers as rows you can create to order your sprites from front to back and put them all in the right order. 

Once you know which sprites you would like to go on top, you can do this by having a sprite `go to front`{:class="block3looks"} or `go to back`{:class="block3looks"} layer, and stepping into the right position through the layers.

--- /collapse ---

--- collapse ---
---
title: Program your sprites from front to back
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
You can also create static scenery by using sprites and shapes to create a 'foreground' and 'background' in your scene. Once you have your layers set up, use the `Go backward 1 layers`{:class="block3looks"} or `Go forward 1 layers`{:class="block3looks"} to change whether your sprites are behind or in front of parts of your scenery to make it feel more three dimensional! 

--- collapse ---
---
title: Creating a foreground and background with sprites
---
You can also use the  `layer`{:class="block3looks"} blocks in your scripts, to  dynamically change the order of sprites and create the illusion of depth while your code is running. 


Click the green flag on the project below and notice how the character goes behind one tree, but in front of another:

**Depth with Layers**: [See inside](https://scratch.mit.edu/projects/447184192/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/447184192/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

--- /task ---

--- task ---
Now, we're going to change the size of some of our sprites to make it appear as fi they are further away from us than others. When we look at things which are further away in real life, they look a lot smaller than they do up close. If we really want our animation to look realistic, we can change the size of our sprites to mimic this effect. Have a look at this project and notice how the size of the numbers adds to the illusion of distance:

**Depth and Distance**: [See inside](https://scratch.mit.edu/projects/445071529/editor){:target="_blank"}

Click or tap the backdrop to change the scenery for some added perspective!

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445071529/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>


Use the `change size by ()`{:class="block3looks"} or  `set size to ()%`{:class="block3looks"} block in your code to make your sprite shrink when it moves to the `back layer`{:class="block3looks"} and grow when it moves to the `front layer`{:class="block3looks"}! 

--- collapse ---
---
title: Changing size with layer
---
Make your code change the size of your sprite when the layer changes by adding the `set size to ()%`{:class="block3looks"} like this:
``` blocks3
when [up arrow v] key pressed
go to [front v] layer
set size to (120)%
```


``` blocks3
when [down arrow v] key pressed
go to [back v] layer
set size to (100)%
```

You can also have the size of your sprite change every time it changes layer by using the `change size by ()`{:class="block3looks"} blocks:

``` blocks3
when [up arrow v] key pressed
go [forward v] (1) layers
change size by (20)
```

``` blocks3
when [down arrow v] key pressed
go [back v] (1) layers
change size by (-20)
```

--- /collapse ---

--- /task ---


--- save ---
