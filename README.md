# Instructions to run 
download LOVE from https://www.love2d.org/
from the parent directory of the project, run 
``` <path to your love executable> CelesteTAS <cartname>.p8``` 
where cartname is the name of the cart you want to TAS which should be in the carts folder

# Usage
First of all, you will see a timer in the top-left corner, which tracks the time, and a black rectangle right next to it, the black rectangle is an input viewer, where you can see what keys are being pressed on that frame. The input viewer will be blacked out because you can't input anything yet, as you are in the spawning state, once the spawning state is over (around 26 frames after loading the level, depends on the level) you will be able to see the keys.

Each time you press a key (up, down, right, left, x, c, or z) that key will toggle on/off for that frame.

To go to the next level press F and to go to the previous level press S, note that this will reset the inputs.

To step forward in time press L, which will advance the game one frame, and the keys that were inputted for that frame will be executed.

To step backwards in time press K, which will step 1 frame backwards, and you can change what was pressed before.

To change the number of dashes you have press 0,1,2,3 or -, pressing a number will set your number of dashes, and pressing - will activate default mode (1 dash before 2300, and 2 dashes after).

To see the TAS in real time press P, which will start reproducing the inputs from the frame you are currently on. (Note: you shouldn't input anything while the TAS is reproducing)

To go back to the first frame press D, which will restart the game but still keep your inputs.

To reload the level and delete your inputs press R.

To hide/unhide the timer and input viewer press E.

To save a clean version of the TAS press U, which will playback the tas, then automatically create a file called 'TAS1.tas' (replacing the 1 with the level number you are on) in the love2d folder (check the [love2d page](https://love2d.org/wiki/love.filesystem) for more information), or check the console message that appears when you save the TAS, which specifies the directory it gets saved to.
this can be interrupted at any time by pressing P. 
Note: a clean version will only be saved if the level can be finished. If it can't (because of an incomplete TAS, etc.) only a raw version will be saved

To save a raw version of the TAS press M, which will save the file in the same place as U, but it won't cut off inputs after the end of the level. it is recommended you use this only for saving WIP TASes

To open a TAS file, simply drag the file into the window, note that this won't change the current state of the game, so you should always press D after loading a file.

To edit the RNG of the balloons or chests (the balloons initial position is determined by RNG and the x position of the berry coming out of a chest is also determined by RNG) press B, which will toggle RNG manipulation mode (note that you can't toggle it on the first frame of a room being loaded), while in RNG manipulation you can press the right and left arrow keys to change the selected balloon or chest, to change the position of the selected balloon or chest use the up and down arrow keys, you will see a number under the balloon or chest changing, that's the balloon's or chest's seed. When you save a file the RNG seeds will get saved and will also get saved when you press D.
In RNG manipulation mode you can also offset clouds 1 frame forwards or backwards. Don't use this feature unless you know what you're doing, you don't know what you're doing, don't use this feature.

Press Y to see the current position, rem values (sub-pixels) and speed of the player on the console.

To reproduce a full game TAS, create a folder named 'TAS' inside the love2d folder, inside this folder there should be a TAS file for each level, named TAS1, TAS2, ...., TAS31 (you can't TAS level 31, so you should download the TAS31 file from the existing TASes), and to reproduce it press N.

You can press F1 or F6 to save a screenshot, F3 or F8 to start a recording and F4 or F9 to save the recording, both saved to the love2d folder, and the console output will show what that directory is.

# Mod Compatability list
| Mod | Compatibility |
| ------ | ------ |
| Celeste | fully supported |
| Everred | fully supported |
| Caligo |fully supported |
| Arielle | supported, custom cart needed |
| Noeleste | supported, custom cart needed |
| Old Site | supported, custom cart needed |
| Perisher | supported, custom cart needed |
| Funklost | supported, custom cart needed |
| Terra Australis | supported, custom cart needed |
| Adelie | not supported, crashes on launch |
# TAS Database 
https://celesteclassic.github.io/tasdatabase/
