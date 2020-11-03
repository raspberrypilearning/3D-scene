## Sound

Now you're going to add some `sounds`{:class="block3sounds"} to your project. Depending on your plans, this could be a continuous background soundtrack or sounds that happen at a specific time, such as when a new sprite appears.

--- task ---
 
Think about what kind of sound you want and when you want that sound to happen.
 
This project has a soundtrack that runs throughout, plus the **???** sprite makes a sound whenever it touches the edge of the Stage:
 
**?soundtrack?**: [See inside](https://scratch.mit.edu/projects/436255738/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe src="https://scratch.mit.edu/projects/436255738/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>
 
--- /task ---
 
--- task ---
Add code to run `sounds`{:class="block3sound"} blocks where you want sound in your project.
 
Have a look at these how to’s depending on what kind of soundtrack you want to use:
 
--- collapse ---
---
title: Continuous soundtrack using a long sound
---
 
**Beating heart**: [See inside](https://scratch.mit.edu/projects/435725413/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/435725413/?autostart=false" frameborder="0"></iframe>
</div>
 
You can use the `set size`{:class="block3looks"} or `change size`{:class="block3looks"} block to create a pulsing effect, such as a beating heart.
 
**Note:** The `set size`{:class="block3looks"} block sets size to a specific value, while the `change size`{:class="block3looks"} changes the value from what it previously was, e.g. `change size by 10`{:class="block3looks"} adds `10` to the value of size.
 
```blocks3
when green flag clicked
set size to (160) %
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
title: Continuous soundtrack using a sequence of short sounds
---
 
Some Scratch sprites have costumes that can be used to create a simple animation.
 
**Avery walking**: [See inside](https://scratch.mit.edu/projects/436256679/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/436256679/?autostart=false" frameborder="0"></iframe>
</div>
 
 
Use `next costume`{:class="block3looks"} inside a `forever`{:class="block3control"} loop with a `wait`{:class="block3control"} to create an animation:
 
```blocks3
when green flag clicked
forever
next costume
wait (0.3) seconds
```
 
One second is often too long to wait before changing to the next costume, so you need to use numbers smaller than `1` in the `wait` block. A wait of `0.1` is one tenth of a second, and `0.5` is half a second. If you wait `0.2` seconds then the sprite will change costumes five times every second.
 
When a sprite reaches its last costume,  the `next costume`{:class="block3looks"} block goes back to the first costume, so the sprite continues to move.
 
You can combine animation with movement to create sprites that walk or fly.
 
--- /collapse ---
 
Or you may just want to use sounds that happen at a certain time, such as when a user interacts with a sprite or when sprites interact with each other.
--- collapse ---
---
title: Incidental sounds
---
 
Some Scratch sprites just have one costume or have multiple sprites that don't work as an animation. If you choose one costume, then duplicate it and make a small change, it can create an animation effect.
 
**Robot animation**: [See inside](https://scratch.mit.edu/projects/436260207/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/436260207/?autostart=false" frameborder="0"></iframe>
</div>
 
Switch to the **Costumes** tab for your sprite.
 
The **Robot** sprite comes with costumes for three different robots and you only want to use one of them. Delete any costumes that you will not use in your animation.
 
Right-click on the costume, and choose **Duplicate**.
 
Make small changes to the costume such as moving, rotating, or changing all or part of the costume, or adding movement lines.
 
If your costume uses vector graphics, then you can select parts of a costume to change.
 
![Animated gif showing changes to Robot costume](images/edit-robot-costume.gif)
 
You can duplicate the costume again and make more changes to add more frames to your animation.
 
You can now use your costumes in a simple sprite animation.
 
--- /collapse ---
 
--- /task ---
 
--- task ---
Work on your animation until you get the effect you want.
 
You can change the timing of your animation if you change the value in the `wait`{:class="block3control"} block. You might also want to change the movement code for the sprite.
 
**Tip:** It is always good to try one change at a time and test what it does so that you can easily undo any changes that you do not like. You could also make little changes as you go along.
 
--- /task ---
 
 
--- save ---
