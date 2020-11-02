## Animate using looks
Now you're going to add `Looks`{:class="block3looks"} blocks inside a `forever`{:class="block3control"} block, to create an animation effect to make your sprite look more interesting.

--- task ---

Think about how you want to animate your sprite using `Looks`{:class="block3looks"} blocks. 

The **Ghost** sprite is animated by its changing costume and brightness:

**Ghost animation**: [See inside](https://scratch.mit.edu/projects/436255738/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/436255738/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /task ---

--- task ---
Add code to your sprite to create an animation effect. If you don't think your sprite needs an animation, you can skip this task. 

Use one of the animation effects below as a starting point:

--- collapse ---
---
title: Change looks to create an animation effect
---

**Beating heart**: [See inside](https://scratch.mit.edu/projects/435725413/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/435725413/?autostart=false" frameborder="0"></iframe>
</div>

You can use the `set size`{:class="block3looks"} or `change size`{:class="block3looks"} block to create a pulsing effect, such as a beating heart.

**Note:** The `set size`{:class="block3looks"} block sets size to a specific value, while `change size`{:class="block3looks"} changes the value from what it previously was, e.g. `change size by 10`{:class="block3looks"} adds `10` to the value of size.

```blocks3
when green flag clicked
set size to (160) %
forever
change size by (40)
wait (0.2) seconds
change size by (20)
wait (0.2) seconds
change size by (-20)
wait (0.2) seconds
change size by (-40)
wait (0.2) seconds
end
```

This code uses a series of `change size`{:class="block3looks"} and `wait`{:class="block3control"} blocks to make the heart grow and shrink. Try to create your own pulsating sprite.

You could also try change the `graphic effects`{:class="block3looks"} to create a sprite that continues to change its appearance. 

```blocks3
when green flag clicked
change [ghost v] effect by (75)
wait (1) seconds
change [ghost v] effect by (-75)
```

**Note:** If you use code that changes a graphic effect and then changes it back again, don't forget to use a `wait`{:class="block3control"} block in between, otherwise it will happen so fast that you won't see it!

You can use a `clear graphic effects`{:class="block3looks"} block at any time to reset the effects.

```blocks3
clear graphic effects
```

--- /collapse ---

--- collapse ---
---
title: Change costumes to make a simple animation
---

Some Scratch sprites have costumes that can be used to create a simple animation. 

**Avery walking**: [See inside](https://scratch.mit.edu/projects/436256679/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/436256679/?autostart=false" frameborder="0"></iframe>
</div>


Use `next costume`{:class="block3looks"} inside a `forever`{:class="block3control"} loop with a `wait`{:class="block3control"} block to create an animation: 

```blocks3
when green flag clicked
forever
next costume
wait (0.3) seconds
```

One second is often too long to wait before changing to the next costume, so you need to use numbers smaller than `1` in the `wait`{:class="block3control"} block. A wait of `0.1` is one tenth of a second, and `0.5` is half a second. If you wait `0.2` seconds, then the sprite will change costumes five times every second. 

When a sprite reaches its last costume, the `next costume`{:class="block3looks"} block goes back to the first costume, so the sprite continues to move. 

You can combine animation with movement to create sprites that walk or fly.

--- /collapse ---

If your sprite doesn't have costumes that are suitable for animation, then you can make your own:

--- collapse ---
---
title: Duplicate and edit a costume to use in an animation
---

Some Scratch sprites just have one costume or have multiple sprites that don't work as an animation. If you choose one costume, then duplicate it and make a small change, it can create an animation effect. 

**Robot animation**: [See inside](https://scratch.mit.edu/projects/436260207/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/436260207/?autostart=false" frameborder="0"></iframe>
</div>

Switch to the **Costumes** tab for your sprite. 

The **Robot** sprite comes with costumes for three different robots and you only want to use one of them. Delete any costumes that you will not use in your animation. 

Right-click on the costume, and choose **Duplicate**. 

Make small changes to the costume, you could move, rotate, or change all or part of the costume. Alternatively, you could add movement lines. 

If your costume uses vector graphics, then you can select parts of a costume to change. 

![Animated gif showing changes to Robot costume](images/edit-robot-costume.gif)

You can duplicate the costume again and make more changes to add more frames to your animation.

You can now use your costumes in a simple sprite animation.

--- /collapse ---

--- /task ---

--- task ---
Work on your animation until you get the effect you want. 

You can change the timing of your animation if you change the value in the `wait`{:class="block3control"} block. You might also want to change the movement code for the sprite. 

**Tip:** It is always good to try one change at a time and test what it does so that you can easily undo any changes that you do not like. 

--- /task ---


--- save ---

