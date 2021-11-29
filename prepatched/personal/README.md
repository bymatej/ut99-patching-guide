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

### MacOS (tested on BigSur)
Steps:
- download the latest patch for MacOS first: https://github.com/OldUnreal/UnrealTournamentPatches/releases/download/v469b/OldUnreal-UTPatch469b-macOS.dmg
- Open the dmg installer
- Place the app file to Applications folder (just use the installer window to drag and drop)
- close the installer
- Run the UnrealTournament.app (it is in `/Applications/UnrealTournament.app`). It will fail, and that's OK (for now). Moving on...
- download zip (see links below)
- extract zip
- move the content of the folder named `UnrealTournament` that you just extracted to `/Applications/UnrealTournament.app/Contents/MacOS/` and if prompted do NOT replace any files/folders, but it will likely only complain about the Help folder (open `/Applications/` and right-click on `UnrealTournament.app` and select "Show package content" to be able to go to Contents/MacOS/ folder)
- while moving the files, the `System` folder will complain, because `~/Library/Application Support/Unreal Tournament/System/UnrealTournament.ini` file is already there - do NOT replace this ini file with the one from the zip
- Run the UnrealTournament.app (it is in `/Applications/UnrealTournament.app`)
- if you face any errors, check this file and try to fix it yourself `~/Library/Application Support/Unreal Tournament/System/UnrealTournament.log`
- Keep in mind that the User.ini and other files are still in `~/Library/Application Support/Unreal Tournament/System/`. You can also place maps, textures, sounds, etc. there, but I never tried it.


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

### Mac
Seem to work OK.

# Server info
- My ini file: https://github.com/bymatej/contabo-vps-notes/blob/main/notes/installation/games/ut99/ut99server.ini (bugger off)
- URL: ut99.bymatej.com:7777
- Password: ask me for the password
- Admin console: https://ut99-admin.bymatej.com/
- Filebrowser: https://ut99-files.bymatej.com/

