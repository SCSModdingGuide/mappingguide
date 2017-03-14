# Tutorial 1 -- Basic Editor Setup

## 0 -- Game Folders

This guide will refer to two folders used by ETS2/ATS. We'll be calling them the **user** folder and the **executable** folder.

The _user_ folder is the game folder located in the _Documents_ directory on Windows platforms. This folder contains the _mod_ folder, where we'll place our created maps.

```
C:\Users\<username>\Documents\Euro Truck Simulator 2
C:\Users\<username>\Documents\American Truck Simulator
```

The _executable_ folder is the game's main folder, which in it contains the game files and executables. Maps we create will be saved in a subfolder here

```
C:\Program Files (x86)\Steam\steamapps\common\Euro Truck Simulator 2
C:\Program Files (x86)\Steam\steamapps\common\American Truck Simulator
```

For the sake of brevity, only the paths for Euro Truck Simulator 2 will be repeated in this guide. All instructions are equivalent for both games.

## 1 -- Enabling the Editor

Navigate to your user folder -- ```C:\Users\<username>\Documents\Euro Truck Simulator 2``` by default -- and open ```config.txt``` in a text editor.

Find the line ```g_developer "0"``` and change the value to ```"2"```. Then find ```g_console "0"``` and change the value to ```"1"```.

Next time you launch the game, you'll be able to load the editor using the console command ```edit```. Before you do this however, you should make one more change to enable saving of maps.

## 2 -- Enabling Saves

The editor saves maps to a directory in the _executable_ folder, however this folder does not exist by default, and the editor produces an error rather than saving.

Go to your executable folder -- ```C:\Program Files (x86)\Steam\steamapps\common\Euro Truck Simulator 2``` by default -- and then create a folder called ```base```, then another folder inside this one called ```map```.

That's it! you're ready to start mapping.

### A Note on loading saved maps

The process for loading maps is somewhat laborious, as the editor can only use game files that are currently loaded by the game.

You should complete the next tutorial in a single sitting if possible, but if you need to load your saved process for any reason, skip to tutorial 3, where the process of loading your maps into the game is detailed.
