## Soundtrack

In this step you are going to add some `sounds`{:class="block3sound"} to your project. Depending on your plans, this could be a continuous background soundtrack or sounds that happen at regular intervals.

--- task ---
 
Think about what kind of sound you want and when you want that sound to happen.
 
This project has a soundtrack that runs throughout, plus the **Hen** sprite makes a sound every three seconds:
 
**Hen and farmyard**: [See inside](https://scratch.mit.edu/projects/444559955/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe src="https://scratch.mit.edu/projects/444559955/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>
 
--- /task ---

There are two `sounds`{:class="block3sound"} blocks with very important differences that you need to understand.

+ When you `play sound until done`{:class="block3sound"}, the sound will play all the way through. tThe next line of code in the script will not run until the sound it finished.

+ When you `start sound`{:class="block3sound"}, the sound will play but the next line of code will run immediately and will not wait for the sound to finish first.

This means that if you had a series of `start sound`{:class="block3sound"} blocks the sounds would all play almost at the same time, layered on top of each other. The effect can be interesting and sometimes messy.

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

Start by selecting the sprite that you want to have the new sound and select the **Sounds** tab. Each sprite starts with a default sound.

![Sound tab](images/soundTab.png)

To get to Scratch's library of built-in sounds, click on the **Choose a Sound** button.

![Choose a sound button](images/chooseASoundButton.png)

If you hover your mouse over the play symbol of a sound, Scratch will preview the sound for you.

![Preview a sound](images/soundPreview.png)

Click on any sound to add it to your sprite. You will be taken straight back to the **Sounds** tab and you will be able to see the sound that you just added.

![Sounds tab with new sound](images/newSoundAdded.png)

If you switch to the **Code** tab and look at the `Sound`{:class="block3sound"} blocks menu, you will see you that the new sound is now available in the drop-down.
 
![New sound available](images/newSoundBlock.png)

--- /collapse ---
 
--- task ---
Add code to run `sounds`{:class="block3sound"} blocks where you want sound in your project.
  
--- collapse ---

---
title: Add continuous soundtrack using a long sound
---
 
Click the green flag to hear the sounds. 

**Radio soundtrack**: [See inside](https://scratch.mit.edu/projects/444581851/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444581851/?autostart=false" frameborder="0"></iframe>
</div>
 
Usually a continuous background soundtrack will start at the beginning `when green flag clicked`{:class="block3events"}, but you could have it starting at any time that suits your project.

To make a sound play continuously, use a `play sound until done`{:class="block3sound"} block inside a `forever`{:class="block3control"} loop. Once the sound has finished, the `forever`{:class="block3control"} loop makes the sound start again from the beginning.

This example uses a single long sound clip repeated as a soundtrack.
 
```blocks3
when green flag clicked
forever
play sound (Dance Snare Beat v) until done
end
```

**Note:** When choosing a new sound, if you select the **Loops** category, Scratch will only show you the sounds which are suitable for a single looping soundtrack.

![Loop sounds](images/loopSounds.png)

--- /collapse ---
 
--- collapse ---

---
title: Add continuous soundtrack using a sequence of short sounds
---
  
Click the green flag to hear the sounds. 

**Champ performance**: [See inside](https://scratch.mit.edu/projects/444673165/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444673165/?autostart=false" frameborder="0"></iframe>
</div>

Select a `forever`{:class="block3control"} block to create a looped sound. Select some sounds you like and/or experiment. You can either create:
+ a series of short sounds in a sequence of sounds i.e playing one after the other.
+ or compose a soundtrack using different instrument notes and effects.
 
```blocks3
forever
play sound (Low Boing v) until done
play sound (Low Boing v) until done
play sound (Drum Buzz v) until done
play sound (Pop v) until done
play sound (Bird v) until done
play sound (Bark v) until done
play sound (Glug v) until done
End
```
 
Click on the `forever`{:class="block3control"} block to play the sounds in the loop. Note, that your latest version of sounds and their order will only play when the old loop has finished.

**Note:** The example only uses `play sound until done`{:class="block3sound"} blocks, so that each sound finishes before the next begin. As you experiment, you might want to try adding some `start sound`{:class="block3sound"} blocks in where you want more than one sound to play at once. For instance you may want to have `start Bark sound`{:class="block3sound"} followed by `play Bird until done`{:class="block3sound"} to get a bird sound and a bark at the same time.

```blocks3
forever
play sound (Low Boing v) until done
start sound (Pop v)
start sound (Finger Snap v)
play sound (Drum Buzz v) until done
+ start sound (Bark v)
+ play sound (Bird v) until done
End
```
Once you have found a sequence that you are happy with and works for your project, add a `when green flag`{:class="block3events"} clicked `Event`{:class="block3events"} block to the top and your sequenced soundtrack will start when your project is run.

```blocks3
when green flag clicked
```
 
--- /collapse ---
 
Or you may just want to use sounds that happen at regular intervals.

--- collapse ---

---
title: Add regular interval sounds
---
 
**Football sounds**: [See inside](https://scratch.mit.edu/projects/450870079/editor){:target="_blank"}
 
Click the green flag to hear the sounds. 

<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/450870079/?autostart=false" frameborder="0"></iframe>
</div>
 
 In this project, the Stage has code to play a sound at regular intervals:

 ```blocks3
 when flag clicked
 forever
 wait (3) seconds
 play sound (Cheer v) until done
 end
 ```

 The **Whistle** sprite also plays a regular sound: 

 ```blocks3
 when this sprite clicked
 forever
 play sound (referee whistle v) until done
 wait (4) seconds
 end
 ```

--- /collapse ---

--- /task ---
 
--- task ---

Once you have chosen your sounds, you may want to change the `volume`{:class="block3sound"}, `pitch`{:class="block3sound"} blocks, or `pan`{:class="block3sound"} blocks (so you hear the sound from the left or the right).

--- collapse ---

---
title: Setting and changing the volume, pitch and pan effect
---

Click the green flag to hear the sounds. 

**Sound effects**: [See inside](https://scratch.mit.edu/projects/451697380/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451697380/?autostart=false" frameborder="0"></iframe>
</div>

The `pan`{:class="block3sound"} block allows you to control whether a sound comes out of the left or right speaker or headphone or both. A value of `-100` plays **all** of the sound through the left speaker, `100` plays **all** of the sound through the right speaker, values in between gradually shift the sound balance from the left to the right as the number increases.

If you have stereo headphones or speakers then the sound from the left speaker sprite will come from the left headphone/speaker and the sound from the right speaker sprite will come from the right headphone speaker. 

Left speaker:

```blocks3
set [pan left/right v] effect to (-100)
```

Right speaker:

```blocks3
set [pan left/right v] effect to (100)
```

**Tip**: Listen carefully to where the sound is coming from. 

The pitch of a sound is how high or low it is. Setting the pitch to a higher value also makes a sound faster. You can set the pitch to values between -360 (very low) and 360 (very high). 

This code sets the pitch of the guitar to 200 (high).

```blocks3
set [pitch v] effect to (200)
```

You can set the volume from 0 (silent) to 100 (full volume).

The volume of the guitar is lower than the volume of the speakers. This is useful if you want some sounds louder than others or if you want a sprite to appear further away. 

This code sets the volume of the guitar to 10 (quiet):

```blocks3
set volume to (10) %
```

Sound effects are cleared when the green flag is clicked.

--- /collapse ---
  
--- /task ---
 
 
--- save ---
