## Distance and depth

Now, you’re going to look at how to layer sprites to make some appear in front or behind others by using some of the `looks`{:class="block3looks"} blocks.

When you think about a stage or theatre in real life, you understand that the actors can move closer or further away from the audience; so that one can pass in front of another. This is called **depth**, and it makes things feel more realistic when you watch them (even cartoons!)

You can use `layers`{:class="block3looks"} in your Scratch projects to create the same effect! 

In addition to coding layers to create a sense of 3-dimensions, in this step you will also change the size of sprites in relation to each other. This will help to create a greater sense of depth to your scenery. Bigger sprites appear to be closer to the front of the stage with smaller sprites appearing further away.

**Cars in Space**: [See inside](https://scratch.mit.edu/projects/447759319/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/447759319/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>


--- task ---
Now, we're going to create multiple layers for your sprites. You can keep it simple and just use the `front layer`{:class="block3looks"} and `back layer`{:class="block3looks"} if you like, or create multiple layers for more complex projects.

This project uses front and back `layers`{:class="block3looks"} to make the cats appear to circle the globe:

**Cats Around the World**: [See inside](https://scratch.mit.edu/projects/444530974/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/444530974/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>


Think of the sprites in your project and decide how you can have them move in front of (or behind!) different parts of your project, like the scenery or other sprites. 

Consider how many layers you will have, and add blocks that will allow your sprites to change between the layers as above.

--- collapse ---

--- 
title: Treat layers like rows
---
**Tip:** Think about layers as rows you can create to order your sprites from front to back and put them all in the right order. 

Once you know which sprites you would like to go on top, you can do this by having a sprite `go to front`{:class="block3looks"} or `go to back`{:class="block3looks"} layer, and stepping into the right position through the layers.

--- /collapse ---

To select your first sprite, click or tap on it under the Stage.

Click on the Code tab.

Use a `go to [back v] layer`{:class="block3looks"} or a `go to [front v] layer`{:class="block3looks"} block and either a `go [forward v] (1) layer`{:class="block3looks"} or a `go [backward v] (1) layer`{:class="block3looks"} block to create an order for your sprites and scenery.

--- collapse ---
--- 
title: Control layer placement with code
---
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

Have a look at how this project orders the sprites from front to back by using `Go [backward v] (1) layers`{:class="block3looks"} to create the feeling that the number 6 is 'at the back', while the number 1 is 'at the front':

**Numbered Layers**: [See inside](https://scratch.mit.edu/projects/445055782/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445055782/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>
--- /task ---

--- task ---
You can also create static scenery by using sprites and shapes to create a 'foreground' and 'background' in your scene. Once you have your `layers`{:class="block3looks"} set up, use the `Go [backward v] (1) layers`{:class="block3looks"} or `Go [forward v] (1) layers`{:class="block3looks"} to change whether your sprites are behind or in front of parts of your scenery to make it feel more three dimensional! 

--- collapse ---
---
title: Creating a foreground and background with sprites
---
You can also use the  `layer`{:class="block3looks"} blocks in your scripts, to  dynamically change the order of sprites and create the illusion of depth while your code is running. 


Click the green flag on the project below and notice how the cat goes behind one tree, but in front of another:

**Depth with Layers**: [See inside](https://scratch.mit.edu/projects/447184192/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/447184192/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

--- collapse ---
---
title: Creating a foreground and background with scenery
---
You can also create parts of your scenery as separate sprites which sit on different `layers`{:class="block3looks"} by using the **paint editor**, then have your character sprite move between the shapes you create. This may suit your project better than using existing sprites from the library and will allow you to easily mask the edges of your stage. 

**Hills as sprites**: [See inside](https://scratch.mit.edu/projects/446137341/editor){:target="_blank"}

![Make hills as a number of sprite](images/challenge2-backdrop-sprites-person.gif)

![Make hills as a number of sprite](images/challenge2-backdrop-sprites.png){:width="400px"}

If you need some reminders, click back to the previous **Scenery** step for some tips!

--- /collapse ---

--- /task ---

**Using size to create distance**

--- task ---
When we look at things which are further away, they look a lot smaller than they do up close. If we really want our animation to look realistic, we can change the size of our sprites to mimic this effect. Have a look at this project and notice how the size of the numbers adds to the illusion of distance:

**Depth and Distance**: [See inside](https://scratch.mit.edu/projects/445071529/editor){:target="_blank"}

Click (or tap on mobile!) the backdrop to change the scenery for some added perspective!

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
