# UT99 Patching instructions
Patching is required so you have the latest version of Unreal Tournament 99.
It also helps this ancient game run on modern versions of Windows, such as Windows 10.

## Disclaimer
I did not "invent" any of this. I just gathered all the information in one place for myself. 

This is based on these links/tutorials: 
- https://www.epicgames.com/unrealtournament/forums/past-unreal-tournament-games/unreal-tournament-%E2%80%9899/10649-ut99-not-working-properly-in-windows-10?p=224273#post224273
- https://ut99.org/viewtopic.php?f=6&t=373
- https://steamcommunity.com/sharedfiles/filedetails/?l=german&id=272924930

All credits go to people that created UT, patches, bonus packs, posts on the forums, etc.

## How to use these instructions? 
Each step is prefixed with a number. And each step has a correpsonding folder that contains some files. 
For example, the step "2 Install the latest patch for clients" has a folder named "2" and the files referred to in this step are in that particular folder.


## 1 Install Unreal Tournament
Install your copy of UT. This is, basically, a prerequisite.


## 2 Install the latest patch for clients
Patch is 436.

First install 1_UTPatch436nodelta.exe, then 2_utpatch436creative.


## 3 Install all the bonus packs

### 0_umod_browser_1_1_.3.exe
This is a small program for browsing inside of umod files. Install it, as you'll need it later.

#### How to use UMod Browser
Instal it by double-clicking the 0_umod_browser_1_1_.3.exe and hecticly clicking "Next", as usual. :) 

Open umod browser, go to File -> Open and open the umod file (they are inside of the bonus pack zip files).

After you've opened the umod, you'll see kind-of-like-a table. First column (Files) contains the file name. Second column (Folder) tells you where in the UnrealTournament directory structure this file needs to be placed. This is very important if you copy the files manually! Third column is just a file size.

However, you don't have to copy the files manually. Just go to Action -> Install current UMod. Then, click on "Browse" and navigate to your UnrealTournament directory. Then hit "Install".

After that, the setup will open. You will be prompted to put the Destination Folder. Again, put the path to your UnrealTournament folder. Click "Next" and then "Finish".

### 1_UTBonusPack.zip
This is the first bonus pack. Extract it. It is an umod file. Just install it as mentioned above.

### 2_utbonuspack2.zip
This is the second bonus pack. Extract it. It is an umod file and two unr files. Install the umod as mentioned above. The two unr files are actually maps. Copy and paste them in your UnrealTournament/Maps directory.

### 3_UTInoxxPack.zip
This is the first bonus pack. Extract it. It is an umod file. Just install it as mentioned above.

### 4_UTBonusPack4.zip
This is the first bonus pack. Extract it. It is an umod file. Just install it as mentioned above.


## 4 OPTIONAL: Install high resolution textures (I, personally, did not bother installing this)
Now install the higher resolution S3TC textures. 
Before you do that be sure to back up your current City.utx, ShaneSky.utx and SkyBox.utx files from your UnrealTournament\Texures folder. 
They're improperly masked and you get some malformed skyboxes. Put those three files into some temporary folder until you need them (for example, UnrealTournament\Texures\backup).

Now install the S3TC texures from CD2.

Right after you have installed S3TC texures, go to your UnrealTournament\Texures folder. 
Take out (cut and paste) the following files and put them besides other previously backed up files (for example, in UnrealTournament\Texures\backup) - Female1Skins.utx, Female2Skins.utx, Male1Skins.utx, Male2Skins.utx, Male3Skins.utx and SkTrooperSkins.utx.
The reason you'll do that is because sometimes you get „sliding zombie players“ effect in some improperly configured servers which is visually really annoying bug.

Now extract the 2_S3TC_Fix.zip, extract it to UnrealTournament\Texures folder and run S3Fix.exe (Depending on your UT install location, for example Program Files folder, you might need to run this utility as administrator (right click and select „Run as administrator“ option). 
This utility will correct that „sliding zombie players“ bug by patching some textures.

After the process is complete (Command Prompt window closes after patching is finished), be sure to take all your previously backed up files and move them into Textures folder answering „Yes“ to overwrite existing ones.


## 5 Update your graphics card and install new OpenGL Renderer
### Update your graphics card.
Do it. Google it.

### Install DirectX runtime libs
Download them from here: https://www.microsoft.com/en-us/download/details.aspx?id=35

Or, just use the 1_dxwebsetup.exe I provided.

### Get OpenGL version 3.7
Download it from: http://www.cwdohnal.com/utglr

Or, just use the 2_utglr37.zip that I provided.

Extract it, and after that, extract its contents to UnrealTournament\System and overwrite existing one.

Now it is time to start up UT and configure it to use just installed OpenGL renderer. 
If you have already passed first run configuration screen, you can change video renderer by going Options -> Preferences -> Video and click on Change button.


## 6 Apply the modified UnrealTournament.ini file
Extract the UnrealTournament.zip. UnrealTournament.ini file will appear. Copy it to UnrealTournament\System folder and overwrite the existing one.

### More configuration
If you want to know more about the configuration, please check out this link: https://ut99.org/viewtopic.php?f=6&t=373 

See the first post, and find this section: "Advanced Engine and OpenGL Settings" and read on.

### Run the game
If it does not work use the Compatibility Troubleshooter from Windows. Also, if it gets stuck in Precaching, then do the following: 
- Go to UnrealTournament\System
- Open UnrealTournament.ini
- Find the section [D3DDrv.D3DRenderDevice]
- Find the attribute UsePrecache
- Change it from True to False
- Restart the game


## Troubleshooting
If something does not work, check the links in the "Disclaimer". Or just Google it. Or reinstall the game and start over.

## Additional links
I found this much later: 
- https://www.reddit.com/r/unrealtournament/comments/evv9hd/unreal_tournament_99_for_macos/
- https://mega.nz/#!tigC1JhJ!EHbt26RWd7eX6v81-S0zVPuKLaREaAyY75OHawtunqs
