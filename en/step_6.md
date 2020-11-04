## Adjustable speed

--- task ---

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

--- /task ---
 
--- save ---
