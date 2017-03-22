# Tutorial 1 --- Basic Editor Setup

This tutorial will help you set up your game correctly for using the map editor.

## 1. Enabling the Editor

Navigate to your user folder -- ```C:\Users\<username>\Documents\Euro Truck Simulator 2``` by default -- and open ```config.cfg``` in a text editor.

Find the line ```g_developer "0"``` and change the value to ```"2"```. Then find ```g_console "0"``` and change the value to ```"1"```.

Next time you launch the game, you'll be able to load the editor using the console command ```edit```. Before you do this however, you should make one more change to enable saving of maps.

## 2. Enabling Saves

The editor saves maps to a directory in the _executable_ folder, however this folder does not exist by default, and the editor produces an error rather than saving.

Go to your executable folder -- ```C:\Program Files (x86)\Steam\steamapps\common\Euro Truck Simulator 2``` by default -- and then create a folder called ```base```, then another folder inside this one called ```map```.

That's it! you're ready to start mapping.

### A Note on loading saved maps

The process for loading maps is somewhat laborious, as the editor can only use game files that are currently loaded by the game.

You should complete the next tutorial in a single sitting if possible, but if you need to load your saved process for any reason, skip to tutorial 3, where the process of loading your maps into the game is detailed.

[<- Back to Index](../index.md) --- [ Tutorial 2 - Creating a basic map ->](2_firstmap.md)
