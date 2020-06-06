# CnC_Remastered_Collection

This code is the game logic for Command and Conquer: Tiberian Dawn, and Command and Conquer: Red Alert. EA did not open source any assets beyond this source and only this source is under GPLv3. In order to obtain the rest of the game you must purchase from Steam or Origin. Once you have purchased the game you can play it and mod it to your heart's content.

## Building this source

This source has been updated to be built in Visual Studio 2019. Simply load the project (CnCRemastered.sln) in VS 2019 and build.

## Artifacts

The artifacts (what you get after building) of this source are RedAlert.dll and TiberianDawn.dll.

## Creating a mod

To create a mod that includes either of the artifacts follow these steps:

1. Create a directory with the name you want for your mod. This directory should go in ~/Documents/CnCRemastered/Mods. If this is a Red Alert mod then put it in  ~/Documents/CnCRemastered/Mods/Red_Alert
2. Inside your new mod directory, create a json file called ccmod.json. Below is an example for a mod named "Test".

`
{
  "name": "Test",
  "description": "Just a test",
  "author": "alexlk42",
  "load_order": 1,
  "version_low": 2,
  "version_high": 1,
  "game_type": "RA"
}
`

3. Create a directory inside your mod directory called Data.
4. Put either the RedAlert.dll or the TiberianDawn.dll in this new Data directory.

## Loading the mod

Open CnC and in the options go to the "Mod" tab. You should see a checkbox for your mod. Simply check it to activate the mod. The game will need to restart.
