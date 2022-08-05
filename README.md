## Instructions for setting up Enemizer with AP

This guide is for setting up Enemizer to use alongside the Archipelago version of the DS3 Randomizer. Before we begin, there are a couple things you need: the DS3 Archipelago Client, and the Static Item and Enemy Randomizer (https://www.nexusmods.com/darksouls3/mods/361). Also, make sure that your Dark Souls III game is set up to “Start in offline mode”. Make sure to have those handy throughout this guide.

## Installation

- Take the DS3 Archipelago Client “dinput8.dll” file, rename it “aprando.dll”, and move it to the same directory as DarkSoulsIII.exe.
- Extract and open the DS3 Static Item and Enemy Randomizer zip file, and instead of following the README for installation, follow this guide instead:
- Move the randomizer folder from the extracted zip into the same directory as DarkSoulsIII.exe.
- Copy “dinput8.dll” and “modengine.ini'' from “randomizer\ModEngine\” into the game directory. Edit modengine.ini to set `modOverrideDirectory="\randomizer"` and `useModOverrideDirectory=1` and `blockNetworkAccess=0` (<-- this is why its important to make sure your game is set to “start in offline mode” in game settings to avoid any vanilla online bans). At the bottom of the modengine file, you will want to add “\aprando.dll” to the chain loader. 
![image info](/modengine.png)
- In the randomizer folder, run DS3Randomizer.exe to open the UI. At the top where it shows “Item Randomizer” and “Enemy Randomizer”, make sure to DESELECT/UNCHECK the “Item Randomizer” option (as items are now being randomized by Archipelago), and then move to the “Enemy Randomizer” tab and select your options. After choosing your options, navigate to the bottom right, SELECT/CHECK the box for “Reroll enemy seed separately” then click "Randomize/Reroll enemies" and wait for "Done" in the status bar. 
![image info](/enemizer.png)
- Now all that's left to do is roll your Dark Souls III Archipelago Rando/Multiworld seed, move your “AP.json” into the same directory as “DarksoulsIII.exe”, launch your game, connect to the server in the cmd prompt, and you’re all set!!
`Note: the two mods dont have full 100% compatibility, but it works for the most part. So you may experience a crash every now and then, which is fine because you can boot right back up and reconnect no problem.`