#Use variables to control the scene
Now you are going to add variables and use them to control the way your project behaves. You could add a variable that changes the colour or other graphic effects or a variable that controls the speed of your project. 

**Tip:** You can use a variable instead of a fixed value in a (input) to a block. 

--- task ---
Think of something you would like the user to be able to change in your project using a slider. This could be the size or graphic effects of a sprite or the speed that a sprite moves at.

In this space scene you can adjust the view of the planet that you see from inside your spaceship. Change the zoom slider to change the size of the planet to make it seem closer or further away and change the colour slide to change the colour effect. 

**Space scene**: [See inside](https://scratch.mit.edu/projects/444586036/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444586036/?autostart=false" frameborder="0"></iframe>
</div>

--- /task ---

--- task ---
Make a new variable and change it to use a slider on the Stage. Drag the variable into a block so that you can control the value. 

--- collapse ---
title: Add a variable with a slider

**Tip:** Always give a variable a sensible name so that you will remember what it is for. You can rename it later if you think of a better name. 

--- /collapse ---

**Tip:** If a block that uses a variable is inside a forever loop then it will use the changed variable value the next time the loop runs. If a block that uses a variable is under a `when this sprite clicked` block then it will use the new value the next time the sprite is clicked. 

You can use one of these examples to get started:

--- collapse ---

---

title: Control movement speed with a variable

---

**Beetle speed**: [See inside](https://scratch.mit.edu/projects/444523655/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444523655/?autostart=false" frameborder="0"></iframe>
</div>

Use a variable called `speed`{:class="block3data"} to control how many steps a sprite moves each time a `forever`{:class="block3control"} loop runs. Setting the speed to a higher number will make the sprite move faster. 

Set the range of the slider to the minimum and maximum speeds that you want to allow (for example 0 and 10).

```blocks3
when flag clicked
forever
move (speed) steps
if on edge, bounce
```

If you want **a different sprite** to go twice and fast then you can multiply `speed`{:class="block3data"} by two to make it move twice as many steps:

```blocks3
when flag clicked
forever
move ((speed) * (2) ) steps
if on edge, bounce
```
--- /collapse ---

--- collapse ---

---

title: Control ghost effect with a variable to see through a sprite

---

**Transparent rainbow**: [See inside](https://scratch.mit.edu/projects/444579529/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444579529/?autostart=false" frameborder="0"></iframe>
</div>

You can use a `ghost`{:class="block3data"} variable to control the ghost effect on a sprite at the front and use it to reveal or hide sprites in lower layers. 

```blocks3
when flag clicked
go to [front v] layer
```

```blocks3
when flag clicked
forever
set [ghost v] effect to (ghost)
```

--- /collapse ---

--- collapse ---

---

title: Change graphic effects when you click on a sprite

---

https://scratch.mit.edu/projects/444527974/
--- /collapse ---

--- collapse ---

---

title: Speed up a sound

---

--- /collapse ---

--- /task ---

--- task ---


--- /task ---


