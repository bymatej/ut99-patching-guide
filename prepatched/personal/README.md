# My personal prepatched copy
No installation, just download, extract and play. 


## Running the game
### Windows
Steps: 
- download zip (see links below)
- extract zip
- go to `UnrealTournament/System/` and open `UnrealTournament.exe`
- Select Direct3D rendering (usually the first option)
- In case of trouble (bad graphics, or whatever) tweak the settings - either in-game, or in `UnrealTournament/System/UnrealTournament.ini` file

### Linux (Ubuntu)
Steps: 
- download and install wine: `sudo apt -y install wine`
- download zip (see links below)
- extract zip
- open terminal and run `wine UnrealTournament/System/UnrealTournament.exe` (note: ensure the correct path is used when running the `wine` command)
- Select Direct3D rendering (usually the first option)
- In case of trouble (bad graphics, or whatever) tweak the settings - either in-game, or in `UnrealTournament/System/UnrealTournament.ini` file


## UT99 prepatched game download
### Unreal Tournament 2000
- GDrive link: https://drive.google.com/file/d/1WUhA-5Zvpm_tLMAlrxtdevihQoK1WXZA/view?usp=sharing
- Alternative (mirror) link: https://private-downloads.bymatej.com/games/UT99/UnrealTournament2000_prepatched_469_v3.rar

### Monsterhunt mod
- GDrive link: https://drive.google.com/file/d/1wjYE1QyXIhov3dncO77qMFkQN809F-WN/view?usp=sharing
- Alternative (mirror) link: https://private-downloads.bymatej.com/games/UT99/maps-and-mods/monsterhunt.zip

#### Note for installing mods (such as Monsterhunt)
Extract the archive and place the content of all folders into respective game folders. 
For example, everything from `monsterhunt/System/` (files from the archive) should be copied to `UnrealTournament/System/` (folder where your UT99 is installed)


## Gamma/Brightness issue
Issue: You Unreal Tournament is too dark. 
Solution: 
- Increase your screen brightnes
- Adjust the brightness in the in-game menu (Preferences -> Brigthness)

### Windows
If the in-game settings do not work, adjust your graphics card brightness and gamma in the respective card settings. For example, NVIDIA and IntelHD graphic cards have their separate apps for tweaking the color schemes, contrast, brightness, gamma, etc. Use that to your advantage.

### Linux
The in-game menu might mess up your gamma in your OS after you set the brightness and exit the game. If that's the case, run this command in your terminal: `xgamma -gamma 1` (tested on Ubuntu)

If the in-game settings do not work, adjust your graphics card gamma by executing this in terminal `xgamma -gamma 3`

Note: `gamma` value must be between `0.100` and `10.000`