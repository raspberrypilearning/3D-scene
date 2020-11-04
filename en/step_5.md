## Distance and depth

Now, you’re going to look at how to layer sprites to make some appear in front or behind others by using some of the `looks`{:class="block3looks"} blocks.

When you think about a stage or theatre in real life, you understand that the actors can move closer or further away from the audience; so that one can pass in front of another. This is called **depth**, and it makes things feel more realistic when you watch them (even cartoons!)

You can use `layers`{:class="block3looks"} in your Scratch projects to create the same effect! 

--- no-print ---

This project uses front and back `layers`{:class="block3looks"} to make the cats appear to circle the globe:

**Layers**: [See inside](https://scratch.mit.edu/projects/444530974/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/444530974/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

--- task ---
Think of the sprites in your project and decide how you can have them move in front of (or behind!) different parts of your project, like the scenery or other sprites. 

Consider how many layers you will have, and add blocks that will allow your sprites to change between the layers as above.

--- collapse ---

--- 
title: Treat layers like rows!
---
**Tip:** Think about layers as rows you can create to order your sprites from front to back and put them all in the right order. 

Once you know which sprites you would like to go on top, you can do this by having a sprite `go to front`{:class="block3looks"} or `go to back`{:class="block3looks"} layer, and stepping into the right position through the layers.

--- /collapse ---

--- /task ---

--- task ---
To select your first sprite, click or tap on it under the Stage.

Click on the Code tab.
--- /task ---

--- task ---
Use a `go to [back v] layer`{:class="block3looks"} or a `go to [front v] layer`{:class="block3looks"} block and either a `go [forward v] (1) layer`{:class="block3looks"} or a `go [backward v] (1) layer`{:class="block3looks"} block to create an order for your sprites and scenery.

--- collapse ---
--- 
title: Control layer placement with code
---
You should get your sprite to go to the back (or front) layer and then move a number of layers at the start of your project:

``` blocks3
when green flag clicked
go to [back v] layer
Go [forward v] (1) layers
```

Or:

``` blocks3
when green flag clicked
go to [front v] layer
Go [backward v] (1) layers
```

--- /collapse ---

--- /task ---

--- no-print ---
Have a look at how this project orders the sprites from front to back by using `Go [backward v] (1) layers`{:class="block3looks"}

**Numbered Layers**: [See inside](https://scratch.mit.edu/projects/445055782/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445055782/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>
--- /no-print ---

--- task ---
Once you have your `layers`{:class="block3looks"} set up, use the `Go [backward v] (1) layers`{:class="block3looks"} or `Go [forward v] (1) layers`{:class="block3looks"} to change whether your sprites are behind or in front! 
--- /task ---

You can also use the  `layer`{:class="block3looks"} blocks while your code is running, to  automatically change the order of sprites and create the illusion of depth. 

--- no-print ---
Click the green flag on the project below and notice how the cat goes behind one tree, but in front of another:

**Depth with Layers**: [See inside](https://scratch.mit.edu/projects/445072215/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/445072215/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>
--- /no-print ---

--- task --- 


--- /task ---


--- save ---
