## Sound

Now you're going to add some `sounds`{:class="block3sound"} to your project. Depending on your plans, this could be a continuous background soundtrack or sounds that happen at a specific time, such as when a new sprite appears.

--- task ---
 
Think about what kind of sound you want and when you want that sound to happen.
 
This project has a soundtrack that runs throughout, plus the **Hen** sprite makes a sound every three seconds:
 
**Hen and farmyard**: [See inside](https://scratch.mit.edu/projects/444559955/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe src="https://scratch.mit.edu/projects/444559955/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>
 
--- /task ---

There are two `sounds`{:class="block3sound"} blocks with very important differences that you need to understand.

+ When you `play a sound until done`{:class="block3sound"}, the sound will play all the way through until Scratch runs the next line of code in that script. 
+ When you `start a sound`{:class="block3sound"}, the sound will play but the next line of code will run immeadiately and will not wait for the sound to finish first.

This means that if you had a series of `start a sound`{:class="block3sound"} blocks the sounds would all play almost at the same time, layered on top of each other. The effect can be interesting and sometimes messy.

Have a play with it sometime!

```blocks3
when green flag clicked
start sound (meow v)
start sound (alien Creak2 v)
start sound (Boing v)
start sound (Boom Cloud v)
start sound (Baa v)
```

--- collapse ---

---
title: Adding a sound
---

Start by selecting the sprite that you want to have the new sound and select the Sounds tab. Each sprite starts with a default sound.

![Sound tab](images/soundTab.png)

To get to Scratch's library of built-in sounds, click on the **Choose a sound** button.

![Choose a sound button](images/chooseASoundButton.png)

If you hover your mouse over the play symbol of a sound, Scratch will preview the sound for you.

![Preview a sound](images/soundPreview.png)

Click on any sound to add it to your sprite. You will be taken straight back to the Sounds tab and you will be able to see the sound that you just added.

![Sounds tab with new sound](images/newSoundAdded.png)

If you switch to the Code tab and look at the `Sound`{:class="block3sound"} blocks, you will see you the new sound available in the sound playing blocks.
 
![New sound available](images/newSoundBlock.png)

--- /collapse ---
 
--- task ---
Add code to run `sounds`{:class="block3sound"} blocks where you want sound in your project.
 
Have a look at the how to’s below that will help you to add the kind of sounds that you want for your project:
 
--- collapse ---

---
title: Continuous soundtrack using a long sound
---
 
**Radio soundtrack**: [See inside](https://scratch.mit.edu/projects/444581851/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444581851/?autostart=false" frameborder="0"></iframe>
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

Once you have your sounds, you may want to change some details such as setting the `volume`{:class="block3sound"}, the `pitch`{:class="block3sound"} or the balance, or `panning`{:class="block3sound"}, from left to right.
 
--- /task ---
 
 
--- save ---
