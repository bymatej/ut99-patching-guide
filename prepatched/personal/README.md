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
- download zip (see links below)
- extract zip
- download the latest patch for MacOS first: https://github.com/OldUnreal/UnrealTournamentPatches/releases/download/v469b/OldUnreal-UTPatch469b-macOS.dmg
- Open the patch dmg installer
- Place the app file to Applications folder (just use the installer window to drag and drop)
- close the installer
- open `~/Library/Application Support/` folder and create a new folder in it called "Unreal Tournament" (without quotes and with space between words)
- open `~/Library/Application Support/Unreal Tournament` folder
- Copy everything from the extracted zip EXCEPT the System folder into `~/Library/Application Support/Unreal Tournament` folder
- Go to your Textures folder (in `~/Library/Application Support/Unreal Tournament/Textures`) and remmove `LadderFonts.utx` and `UWindowFonts.utx`
- Run the UnrealTournament.app (it is in `/Applications/UnrealTournament.app`) and it should run the game now
- if you face any errors, check this file and try to fix it yourself `~/Library/Application Support/Unreal Tournament/System/UnrealTournament.log`
- Keep in mind that the User.ini and other files are still in `~/Library/Application Support/Unreal Tournament/System/`. You can also place maps, textures, sounds, etc. there, but I never tried it.
- more info: https://github.com/OldUnreal/UnrealTournamentPatches#macos-installation

#### Issue connecting to server: 'de' version mismatch
If you face the 'de version mismatch' error while connecting to servers, please do the following:
- open `/Applications/` and right-click on `UnrealTournament.app` and select "Show package content" and then go to `Contents/MacOS/` folder
- from the extracted zip go to System and copy `de.u` and `de.int` into `/Applications/UnrealTournament.app/Contents/MacOS/System` and replace


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


# Common issues

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

## I hate the new female announcer
Solution is to replace it with an old one.
Go to your `UnrealTournament/Sounds/` folder, and replace the `Announcer.uax` file with an old one (you may want to back up the current one).
- Old `Announcer.uax` file: https://github.com/bymatej/ut99-patching-guide/blob/4581a7ddcf9a5638784891237e0509aa377f2f62/prepatched/personal/files/Announcer.uax

# Server info
- My ini file: https://github.com/bymatej/contabo-vps-notes/blob/main/notes/installation/games/ut99/ut99server.ini (bugger off)
- URL: ut99.bymatej.com:7777
- Password: ask me for the password
- Admin console: https://ut99-admin.bymatej.com/
- Filebrowser: https://ut99-files.bymatej.com/

