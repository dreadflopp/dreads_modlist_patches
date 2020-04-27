**Where to find Dread's Skyrim Build**

The main version of this guide is on the STEP website. A markdown version of the guide can be found on Github and is included with the patches.

- [Github version of the guide](https://github.com/dreadflopp/dreads_modlist_patches/blob/master/README.md)
- [The guide section on STEP TBA]()

Visit the [STEP forums](https://forum.step-project.com/topic/14888-dreads-skyrim-build-a-step-build/) if you have any questions, suggestions or other feedback.

# Introduction: Welcome to Dread's Skyrim Build

This guide is a STEP build based on the [STEP: Core build](https://www.nexusmods.com/skyrimspecialedition/mods/31054). The STEP team has built a base with mods that enhances and fixes Skyrim without breaking the vanilla look and feel. This guides further enhances Skyrim, adds to it and alters elements of it in several ways. 

**The mods featured in this build are chosen to be immersive and realistic. Realistic in a fantasy setting means believable. The mods should feel like they expand or enhances vanilla Skyrim, like they could have been there from the beginning.**

## What to expect

* Minimalistic survival mode with Creation Club Survival Mode or the mod The Frozen North which uses the same minimalistic and non-intrusive icons as the Creation Club Survival Mode does.
* HD textures for landscapes, structures and buildings that keeps the vanilla look and feel.
* HD textures for clutter, armors, weapons other items.
* Bigger trees for a truly immersive forest.
* Enhanced visuals with Cathedral Weather, Relighting Skyrim and Luminosity Lighting Overhaul.
* New unique armors are added to the game.
* New weapons types with custom animations.
* More adventures with new quests and new lands to visit.
* Overhauled cities, towns and villages.
* Expanded character creation with the CBBE female body with realistic presets.
* Overhauled character leveling and skill system:
    * Overhauled skill trees with new perks.
    * Overhauled magic with new spells.
    * A new class system.
    * New experience system that encourages exploration.
    * Slower leveling to allow you to experience the dlc-sized added content before maxing out your character.
* New, tougher bandits and dragons.
* New NPC's and followers.

## This build is made to be easy to install

* No LOOT rules, every conflict is resolved with the patches. Run LOOT and you are done.
* No bashed patch. All level list conflicts are resolved by the patches.
* No merging of plugins. Every patch is esl-flagged to make sure the plugin limit count is not reached.
* Advanced FOMOD installer for the patches. No need to choose which patches to use, the installer does the work for you.

## Almost all mods are optional

All mods in this build are optional, except for:

* *Unofficial Skyrim Special Edition Patch*.
* *Cloaks of Skyrim* and *Winter is Coming*. Use them both or not at all.

## Github and Changelog

To see a changelog, check the commit history of the [Github version](https://github.com/dreadflopp/dreads_modlist_patches/blob/master/README.md) of the guide. If you are unfamilliar with Git and Github, read the following section.

Git is a system for version control used during software development. A project that is version controlled using git is called a repository. A repository may have different branches, which are different development versions of the software. Branches may be merged, commonly into the master branch. I will only use the master branch. Saving file changes to git is called to commit. Git tracks all commits and lets you revert to previous commits. Github is a cloud based repository. I synchronize my local repository against Github. When users download the repository as a zip-file, it can be installed using Mod Organizer 2's fomod-installer (i.e. how you usually install mods). I am not providing a changelog since the commit history works as a changelog. To see the commit history in Github, make sure you are viewing the code tab and click on xxx commits (where xxx is a number) or click on [this link](https://github.com/dreadflopp/dreads_modlist_patches/commits/master).

## What about Weapons Armor Clothing and Clutter Fixes (WACCF) by Kryptopyr?

WACCF is a great mod that fixes bugs and inconsitencies among weapons, armors, etc. Even though it has the word fixes in its name, it could have been named Weapons Armor Clothing and Clutter *Overhaul*, because it overhauls the weapon and armor stats and progression. To avoid inconsitencies, all mods that add weapons and armors to the game needs to be checked and eventually rebalanced against WACCF. I have decided that isn't something that I want to do, it is just to much work. That said, I still might add it to the guide at a later time. I have had WACCF installed during development and there are unsupported patches for it in the included *old patches* folder.

# Preparations: Game Installation and modding setup

Follow the [system setup guide](https://wiki.step-project.com/Guide:SystemSetupGuide). The system setup guide ensures that all game files are fresh and prompts you to create a basic modding folder structure to install tools into. This guide uses the folder structure from the system setup guide in its instructions. Users that deviates from the system setup guide needs to be aware of this and adjust the instructions accordingly to their installation and modding paths.

**Folder structure**
````
c:\
└── Modding\
    │
    ├── Tools\
    │
    └── Steam\
        │
        └──steamapps\
            │
            └──common\
                │
                └──Skyrim Special Edition\
                    │
                    └──Data\

````

**Common folders refered to in this guide**

* Tools folder: c:\Modding\Tools\
* Main game folder: c:\Modding\Tools\Steam\Steamapps\common\Skyrim Special Edition
* Data folder: c:\Modding\Tools\Steam\Steamapps\common\Skyrim Special Edition\Data

# Tools: Tool Installation and setup

## [Creation Kit](http://download.cdp.bethesda.net/BethesdaNetLauncher_Setup.exe)

The Creation Kit is needed to convert plugins made for Skyrim to work with Skyrim Special Edition. The convertion is very simple and basically just means to open a plugin in the creation kit and resave it. The link above goes to the Bethesda Launcher install file. Installation of the Creation Kit will be done using the Bethesda Launcher.

1. Download and install the Bethesda.net Launcher
1. Run the Launcher and sign in (create an account if you don't have one).
1. Users should see the grey "Creation" icon on the left. Click on it and install.
1. Users should now launch the CK, choose no to extracting the scripts, and close the program. 

Create a new text file in the main game folder and name it *CreationKitCustom.ini*. Paste the following into the file:

````
[Audio]
bEnableAudio=1

[Grass]
bAllowCreateGrass=1
bAllowLoadGrass=0

[General]
bAllowMultipleMasterFiles=1
bAllowMultipleMasterLoads=1

[MESSAGES]
bBlockMessageBoxes=1

[Archive]
SResourceArchiveList2=Skyrim - Voices_en0.bsa, Skyrim - Textures0.bsa, Skyrim - Textures1.bsa, Skyrim - Textures2.bsa, Skyrim - Textures3.bsa, Skyrim - Textures4.bsa, Skyrim - Textures5.bsa, Skyrim - Textures6.bsa, Skyrim - Textures7.bsa, Skyrim - Textures8.bsa, Skyrim - Patch.bsa, Dawnguard.bsa, Hearthfires.bsa, Dragonborn.bsa
````

## [SSE CreationKit Fixes](https://www.nexusmods.com/skyrimspecialedition/mods/20061) 
Download and extract the contents to the main game folder.

## [DynDOLOD](https://www.nexusmods.com/skyrimspecialedition/mods/32382)
Download and extract into its own subfolder of the tools folder. The resources file will be installed later.

## [LOOT](https://github.com/loot/loot/releases)
Download and install the latest version. In the installer, change the installation path to the tools folder.

## [Microsoft Visual C++ 2017 Redistributable](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)
Install *vc_redist.x86.exe* and *vc_redist.x64.exe*.

## [SSEEdit](http://www.nexusmods.com/skyrimspecialedition/mods/164)
Download extract into its own subfolder of the tools folder.

## [Unlimited Bookshelves Patch Generator](https://www.nexusmods.com/skyrimspecialedition/mods/19160)
This is a script for SSEEdit. Unzip the archive and place the content in the SSEEdit script folder (i.e. ..Modding/Tools/SSEEdit/Scripts/).

## [Mod Organizer 2](http://www.nexusmods.com/skyrimspecialedition/mods/6194)
Download the *archive* version and extract into its own subfolder of the tools folder. Name the subfolder *Mod Organizer 2*.

### Initialization

1. Launch MO2
1. Upon launch, you  will have a choice between setting it up as portable or create a new Instance. Choose to create a new Instance.
1. Select SkyrimSE and choose OK.
    * A prompt will appear informing you about the option of changing the location of data stored. Read it and click past it. 
1. The installer should automatically detect the Skyrim SE installation (ie. ..Steam\steamapps\common\Skyrim Special Edition). Select it.
    * If it didn't find the location, browse to to the Skyrim SE installation path. 
1. Another prompt will appear for first time installers asking to run the tutorial or not. First time MO users should run it for a quick lesson on MO. Experienced MO users can skip it.
1. The last prompt will ask if MO can handle .NXM links from the browser. Allow it to do so.
1. MO2 is now set up and ready to use.

### Create mod listings for SSEEdit

To prevent backup and cache files from SSEEdit ending up in the overwrite folder, mixing with other files you might want to keep track of, it is advised to create two empty mod listingss in MO2 for these two types of files:

1. Right click in the mods section of Mod Organizer 2.
1. Select *All Mods/Create empty mod*.
1. Name the mod *SSEEdit Cache*.
1. Repeat the above steps to create another empty mod but name it *SSEEdit Backups* insead.

### Adding executables

All tools except BethINI should be launched through MO2. MO2 may have auto-detected some tool but you need to confirm this and manually add the rest of the tools. 

**Instructions to add tools as executables**

1. Click the Executables button at the top of the main Mod Organizer window.
1. In the Title field type name of the tool.
1. In the Binary field either type the path to the tools executable file or browse for it by selecting the ... button (i.e. ..Modding\Tools\[tool-folder]\[tool].exe).
1. Input arguments in the Argument field.
1. Check the Use Application’s Icon for shortcuts box.
1. Click the Apply button.

Repeat the steps for the executables listed below, filling in the appropriate data. The titles are suggestions.

**Tools**
* SSEEdit
    * Title: SSEEdit
	* Executable: SSEEdit.exe
	* Arguments: 
        * -IKnowWhatImDoing
        * -B:"c:\Modding\Tools\Mod Organizer 2\mods\SSEEdit Backups"
        * -C:"c:\Modding\Tools\Mod Organizer 2\mods\SSEEdit Cache"
* DynDOLOD SE
    * Title: DynDOLOD SE
	* Executable: DynDOLOD64.exe
	* Arguments: -SSE                         
* LOOT
    * Title: LOOT
	* Executable: LOOT.exe
	* Arguments: --game="Skyrim Special Edition"
* SSEEdit Quick Auto Clean (installed with SSEEdit)
    * Title: SSEEdit Quick Auto Clean
	* Executable: SSEEditQuickAutoClean.exe
	* Arguments:
* TexGen SE (installed with DynDOLOD)
    * Title: TexGen SE
	* Executable: TexGen64.exe
	* Arguments: -SSE                           |

*Note that you need to check that that the paths for SSEEdits backup and cache folders in the given arguments are valid for your install.*

## [BethINI SE](http://www.nexusmods.com/skyrimspecialedition/mods/4875)
Download extract into its own subfolder of the tools folder.

### Initialization

BethINI needs to be set up to run for the current profile in MO2 and ran to establish solid INIs before beginning the mod installations. To do this:

1. Close MO2 and run BethINI.
1. Select Skyrim Special Edition from the game selection box.
1. Allow BethINI to handle custom INIs, if prompted.
1. Go to the Setup tab
    * Ensure the Game Path is correct (i.e., ..\Modding\Steam\steamapps\common\Skyrim Special Edition).
    * Ensure the Mod Organizer path is correct (i.e., ..\Modding\Tools\Mod Organizer 2).
    * If the MO path is correct, the INI Path menu will find the user’s profiles in MO2. Select the profile you use in MO.
        * If BethINI does not automatically find the profiles, browse to MO2's Profile folder.
        * For Instance users the profile will be stored in the user's AppData folder (i.e. C:\Users\UserName\AppData\Local\ModOrganizer\SkyrimSE\profiles)
1. At this time BethINI should restart to grab the correct INIs. Continue to customization.

### Customiztion

Close MO2 and run BethINI if it isn't open already.

Use the following settings:

**Basic tab**

In the presets section:

1. Click **Default** button.
1. Click **High** button.
1. Click **BethINI Presets** selector.
1. Make sure **Recommended Tweaks** is checked.

Use the following settings:

* Resolution: set your system resolution
* Antialiasing: *TAA*
* Windowed Mode: *On*
* Borderless: *On*
* FXAA: *Off*
* VSync: *On*
* Lock Frame Rate: *On*

**View Distance tab**

* Object Fade: 25.0
* Actor Fade: 20.0
* Item Fade: 15.0
* Grass Fade: 18000
* Light Fade: 50000
    
On the *Basic* tab, click the **Save and Exit** button.


# Procedures: Common modding procedures

## Using Mod Organizer 2

This guide uses Mod Organizer 2 (MO2) but you may use whichever mod manager you are comfortable with as long as you know how to properly use it. To learn how to use MO2, watch the [tutorial videos by Gamerpoet](https://www.youtube.com/playlist?list=PLlN8weLk86Xh3ue76x2ibqtmMramwQmHB) or read the [STEP guide for Mod Organizer 2](https://wiki.step-project.com/Guide:Mod_Organizer).

## Sorting with LOOT

At any time during the mod installation process LOOT should be used to sort plugin load order before running the game. This is necessary to ensure proper plugin priority (load order), which can have a dramatic impact on the game. Users not running the game during the mod installation step of the Guide can wait to sort after this step is complete. To sort with LOOT:

1. Launch LOOT via Mod Organizer 2 from the executables drop-down menu.
1. Click the “Sort” button at the top of the LOOT window.
1. Examine the resulting order carefully and look for any alerts or warnings and take  note of these. Ignore warnings about patches being available. Patches are provided by this guide.
1. Click the “Apply” button, which has replaced the Sort button at the top.
1. Close LOOT.

## Standard cleaning procedure

Some mods, as well as the official vanilla game, contains plugins (.esp-files) or master plugins (.esm-files) that are dirty. LOOT warns you about such plugins. Clean all plugins that LOOT prompts you to clean. To clean a plugin:

1. Run xEdit64 Quick Auto Clean through Mod Organizer 2.
1. Select the plugin being cleaned (i.e., Update.esm, Dawnguard.esm, etc).
1. xEdit will now automatically clean the *Identical to master* and *deleted* records from the selected mod.
1. Once xEdit is done cleaning, click the X in upper right of the program window to close the program.

## Converting plugins

Many plugins made for classic Skyrim works without issues with Skyrim Special Edition but the plugin form format (form 43) should be updated to Skyrim SE's form format (form 44). To achieve this, simply open the plugin in the Creation Kit and resave it.

Whenever the guide prompts you to convert a plugin, follow these instructions:

1. Run the Creation Kit through Mod Organizer 2.
1. Select the *File* menu and choose *Data...*
1. Find the plugin to be converted and select *Set as Active File*.
1. Note the Parent Masters listed and ensure they are checked (double-click the plugin listing to check it).
1. Click *OK* and allow the Creation Kit to load the files.
1. Once complete, simply save the plug (icon on toolbar or Save from the File menu).
1. Close the Creation Kit.

Use SSEEdit to check that no errors were introduced in the plugin during the conversion:

1. Run SSEEdit through Mod Organizer 2
1. Right-click in the plugin pane and choose Select *None*.
1. Select the plugin being checked and click *OK*
1. Allow SSEEdit to load and process all plugins.
1. Right-click on the last plugin in the left pane (it should be the new plugin), and select Check for Errors.
    * The check should come back reading, *"All done!"*. If there are errors reported, reinstall the mod and redo the conversion.
1. Right-click on the plugin again and choose, *Sort Masters*.
1. Close xEdit and be sure the plugin is checked in the saving prompt.

# Cleaning: Cleaning vanilla master files

To remove redundancy and errors in Skyrims master plugins, it is recommended they be cleaned with SSEEdit before modding begins. This ensures maximum stability and compatibility within the modding experience. This section of the guide walks you through three steps; creating an empty mod in MO2 for the cleaned files, cleaning the files and lastly moving the cleaned files to the created empty mod.

## Create an empty mod

1. On the MO window, click the Open list options button at the top of the left pane, next to the profile selection drop-down.
1. Choose Create empty mod, name it *Cleaned Vanilla Masters*, and click OK.

## Clean the masters

Vanilla masters should be cleaned in the following order:

1. Update.esm
1. Dawnguard.esm
1. Hearthfires.esm
1. Dragonborn.esm 

Follow the standard cleaning procedures to clean Update.esm, followed by Dawnguard.esm. Once Dawnguard is cleaned, complete the manual cleaning below:

1. Run SSEEdit from MO2.
1. At the prompt, double-click on Dawnguard.esm.
1. Once loaded, type in 00016BCF in the FormID field (above the mod list) and hit **Enter/Return**.
1. In the right pane, find the **XEZN - Encounter Zone** record.
1. In the Dawnguard.esm column, right-click on the *RiftenRatwayZone \[ECZN:0009FBB9\]* entry and select Remove.
    - If a prompt appears select Yes for each of these removals. 
1. In the FormID field again, type in 0001FA4C and hit Enter/Return.
1. On the Dawnguard.esm column, right-lick on the Dawnguard.esm header and select Remove.
1. In the FormID field again, type in 0006C3B6 and hit Enter/Return.
1. On the Dawnguard.esm column, right-lick on the Dawnguard.esm header and select Remove.
1. Now close SSEEdit, ensuring Dawnguard.esm is checked on the prompt.

Once Dawnguard's manual cleaning is complete, follow the standard cleaning procedures to clean Hearthfires.esm, and then last, Dragonborn.esm.

## Moving the cleaned files

After the vanilla master files are cleaned, users should move them to their created mod listing in MO2 and restore the original files. This prevents users from having to re-clean the files after verifying their cache in Steam. To do this, complete the following:

1. In a new window, open the Skyrim Special Edition Data directory (e.g. ..\Modding\Steam\steamapps\common\Skyrim Special Edition\Data)
1. Drag and drop (or copy and paste) the four cleaned master files from Data to the *Cleaned Vanilla Masters* folder.
1. In the SSEEdit Backups folder, rename the files to their original names (e.g. *Update.esm*, etc).
    * If there are multiple copies of any of the files, use the one with the earliest timestamp. 
1. Drag and drop the renamed files from the xEdit Backups folder to the Data directory and choose to overwrite/replace, if asked.
1. Close the explorer windows.
1. Drag and drop the new Cleaned Vanilla Masters mod listing in the left pane directly below DLC: Dragonborn.esm.

At this point, the Bethesda masters should be cleaned and the mod list order should reflect: 

1. DLC: Dawnguard.esm
1. DLC: HearthFires.esm
1. DLC: Dragonborn.esm
1. Cleaned Vanilla Masters

# Mod Installation: The mod list

Some things needs to be considered before installing the mods:

* Skyrim master files should be clean, following the procedures in the cleaning plugins
* Mods should be installed in the order that they are listed. You can create separators in Mod Organizer to separate sections of mods, preferably using the names from the mod sections in the guide.
* Always install the main, update and hotfix file(s), unless the guide tells you otherwise.
* The recommended resolutions of textures are just recommendations. You may install higher resolution versions of the mods if your computer can handle it.
* If LOOT tells you to clean a mod, clean it.

The provided guide patches comes with a neat FOMOD installer that automatically chooses what to install. The patches consists of a huge bunch of esl-flagged plugins. Since they are esl-flagged you do not have to worry about the old plugin count limit. Keeping the patches separated in different plugins helps during development when adding, testing and replacing mods. This also makes this mod list mostly modular. There are a few exceptions:

* You need to use the Unofficial Skyrim Special Edition Patch
* Cloaks of Skyrim and Winter is coming should be used together or not at all for the patches to work.

Theoretically, you can leave out any mod from your install besides from those mentioned above.

## Extenders

#### [SKSE64](http://www.nexusmods.com/skyrimspecialedition/mods/30379)

**Root Files Installation**

1. Download the most current archive for Skyrim SE.
1. Open the downloaded archive and extract the following files to the Skyrim Special Edition folder: (..\Steam\steamapps\common\Skyrim Special Edition\) 
	* skse64_X_X_X.dll
	* skse64_loader.exe
	* skse64_steam_loader.dll 

**Data Files Installation**

1. Open MO2 and right-click on the mod list.
1. Hover over All Mods and select Create empty mod.
1. Type in SKSE64, or anything similar.
1. Hold down the Ctrl key and double-click on the newly created mod in the mod list.
1. Keep this folder open for the next two steps below. 

**INI File**

1. In the new Explorer window, create a new folder named SKSE
1. Open that folder and create a new file named SKSE.ini
1. Open the new file and copy and paste the code in the box below
1. Save and close the file.

```
[Display]
iTintTextureResolution=2048

[General]
ClearInvalidRegistrations=1
```

**Scripts**

1. From the archive downloaded above, open the Data folder (..\skse64_X_X_X\Data\)
1. Extract the Scripts folder to the mod's folder.

Once complete, the SKSE mod's folder structure should [look like this.](https://i.postimg.cc/hvWNwHh3/SKSEinMO.jpg)

## Resources

#### [.NET Script Framework](http://www.nexusmods.com/skyrimspecialedition/mods/21294)

#### [Address Library for SKSE Plugins](http://www.nexusmods.com/skyrimspecialedition/mods/32444)
Download and install the All-in-One Main File. 

#### [FileAccess Interface for Skyrim SE Scripts - FISSES](http://www.nexusmods.com/skyrimspecialedition/mods/13956)
Only the Main File is required. 

#### [PapyrusUtil SE - Modders Scripting Utility Functions](http://www.nexusmods.com/skyrimspecialedition/mods/13048)

#### [Scaleform Translation++](http://www.nexusmods.com/skyrimspecialedition/mods/22603)

#### [Skyrim Skill Uncapper](http://www.nexusmods.com/skyrimspecialedition/mods/8889)

#### [SkyUI](http://www.nexusmods.com/skyrimspecialedition/mods/12604)

## Foundational Mods

#### [Unofficial High Definition Audio Project](http://www.nexusmods.com/skyrimspecialedition/mods/18115)
Download and install all Main Files. Merge when asked. 

#### [Unofficial Skyrim Special Edition Patch](http://www.nexusmods.com/skyrimspecialedition/mods/266)

#### [Skyrim Particle Patch for ENB](https://drive.google.com/open?id=12tL3_kpm_KXlQvQqEnK3zOAl-sm_H3Fw)
Download and install the Special Edition PARTICLE PATCH ALL-IN-ONE INSTALLATION file. Do not install the plugin, it is not needed.

#### [Static Mesh Improvement Mod](http://www.nexusmods.com/skyrimspecialedition/mods/659)
Choose custom install in the installer and choose the following:

* Barrels: Modified Vanilla Barrels
* Bowl Ingredients: Improved Bowl Ingredients
* Bridges: Bridges
* Candelabras: Improved Candelabras
* Carriage Seats and Fixes: Improved Carriages
* Chains 3D - Misc: Chains 3D - Misc
* Chains 3D - Pull Levers: Chains 3D - Pull Levers Small Rings (Recommended)
* Chains 3D - Signs: Chains 3D - Signs
* Chains 3D - Whiterun: Chains 3D - Whiterun
* Chandeliers: Improved Chandeliers (Recommended)
* Clothing Fixes: Clothing Fixes
* Dawnguard Soulcairn Bone Piles: Bone Piles Yellow Bones (Recommended)
* Draugr Corpses: Draugr Corpses
* Dungeons Cliffs Snow Skirts: Snow Blending ESP (Recommended)
* Dwemer Animated Lifts: Dwemer Animated Lifts
* Dwemer Clutter: Dwemer Clutter
* Farmhouse Woven Fence: Woven Fence Dense Grey (NOTE: If heavy flickering occurs with the fences, either disable or a different option.)
* Food: Improved Food
* Food - Tomato Style: Default Heirloom
* Furniture Chests: Improved Furniture Chests
* Furniture Common: Improved Furniture SMIM Textures (Recommended)
* Furniture Noble: Improved Furniture Noble
* Hanging Rings: Hanging Rings
* Hawk: Hawk Improvements
* Hearthfires Stuff: Hearthfires Stuff
* Human Skull Fixes: Human Skull Fixes
* Imperial Jail: Improved Imperial Jail (Recommended)
* Jewelry Rings: Jewelry Rings CCO Remade or Jewelcraft
* Lanterns: Lanterns
* Nordic Tables and Benches: Nordic Tables and Benches
* Orc Longhouse: Orc Longhouse
* Poor Coffin: Poor Coffin
* Rabbit: Improved Rabbit
* Rocks - Blackreach: Rocks - Blackreach
* Rocks - Generic: Rocks - Generic
* Rocks - Mountains: Rocks - Mountains
* Ropes 3D - Dungeons: Dungeons 3D Ropes and Glorious Scaffolding
* Ropes 3D - Farmhouse: Farmhouse 3D Ropes No Fade (Recommended)
* Ropes 3D - Raven Rock Docks: Raven Rock Docks 3D Ropes
* Ropes 3D - Riften: Riften 3D Ropes Default Ropes Style (Recommended)
* Ropes 3D - Solitude Docks: Solitude Docks 3D Ropes
* Ropes 3D - Stockade: Stockade 3D Ropes
* Ruins Sarcophagus: Ruins Sarcophagus
* Shack Roofs: Improved Shack Roofs with Dragonborn
* Skeletal Remains 3D: Skeletal Remains 3D
* Smelters: Smelters
* Solitude Gate Doors: Solitude Gate Doors
* Tankards: Dark Brushed Metal Tankards
* Tree - Juniper Tree: Improved Juniper Tree
* Tree - Tundra Tree: Improved Tundra Tree
* Whiterun Castle Wood Carvings: Wood Carvings Improved Vanilla
* Whiterun Doors: Whiterun Doors
* Windmills: DynDOLOD/SkyMills Compatibility
* Xtra Options - Half-Size Textures Addon: None (NOTE: Low VRAM graphic card users can use the half-size textures.)
* Xtra Options - Ultra-Sized Textures Addon: Select Nothing
* Merged Plugin Special Edition Forced Install: Special Edition Merged Plugin Will Be Installed

#### [Forgotten Retex Project](https://www.nexusmods.com/skyrimspecialedition/mods/7849)
Install the main file.

#### [Cathedral - Plants](http://www.nexusmods.com/skyrimspecialedition/mods/26104)

#### [Skyrim Realistic Overhaul](http://www.moddb.com/mods/skyrim-realistic-overhaul)

* Install Part 1-3, choosing to merge the files when asked.
* Install the update file, choosing to merge as well.

#### [Majestic Mountains - Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/11052)
Install a main file, choose the version you like the most. A matching LOD will be installed later.

**Main installer:**
* Snow Mountain Type: Snow Mountain New version ESL
* Optionals: Moss Rocks ESL Version
* Sun Direction (choose one or none): None
* Compatibility Patches: SMIM

#### [Cathedral landscapes](https://www.nexusmods.com/skyrimspecialedition/mods/21954)
In the installer, choose:
* Full Install, Brown Tundra
* Blended Roads

#### [RUSTIC CLOTHING - Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/4703)
Recommendation: 2K

#### [Unofficial Material Fix](http://www.nexusmods.com/skyrimspecialedition/mods/21027)

## Level of Detail (LOD)

#### [DynDOLOD Resources](https://www.nexusmods.com/skyrim/mods/59721?)

Download and install *DynDOLOD Resources SE*. Install using the following options:

* Whiterun Exterior
* Solitude Exterior
* High Hrothgar Window Glow
* DLC2 Vvardenfell 3D Plume
* Desync Birds of Prey

#### [Majestic Mountains - Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/11052)
 
Install a LOD file under the Optional Files section that matches the main file you installed earlier in the guide. Make sure you install this as a new mod named *Majestic Mountains LODs* (or another fitting name).
Install using the following instructions:

* LOD Resolution: 1024 (2-4GB Vram)

## Audiovisual - Animations & Effects

#### [360 Walk and Run Plus](https://www.nexusmods.com/skyrimspecialedition/mods/7446)
In the installer, choose:
* Male
    * Male: 360 + cloak
    * Head Direction: Face towards the direction of movement
* Female
    * Female: 360 + cloak
    * Head Direction: Face towards the direction of movement
    * BBP Option: BBP Off
* Optional Patch: Choose nothing.
* Common: 360 swimming

#### [D13 Faster GET UP STAND UP Animation](http://www.nexusmods.com/skyrimspecialedition/mods/5890)
Install loose files.

#### [Dynamic Animation Replacer](https://www.nexusmods.com/skyrimspecialedition/mods/33746)

#### [EVG Conditional Idles](https://www.nexusmods.com/skyrimspecialedition/mods/34006)
Choose full install in the installer. The modular install is also supported.

#### [No Spinning Death Animation (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/1432)
Install *No Spinning Death Animation MERGED*

#### [Immersive Animations](https://www.nexusmods.com/skyrimspecialedition/mods/4254)
In the installer choose:

* Main Module
* Sneaking
* Strafe
* Greatsword Sprint
* Rogue Stab

#### [Blocking Animation Pack SSE](https://www.nexusmods.com/skyrimspecialedition/mods/4352)

#### [Dual Wield Improved Animation SSE](https://www.nexusmods.com/skyrimspecialedition/mods/5012)

#### [No heavy muscular walk and idle by Scot](https://www.nexusmods.com/skyrimspecialedition/mods/4746)

#### [XP32 Maximum Skeleton Special Extended - XPMSSE](http://www.nexusmods.com/skyrimspecialedition/mods/1988)

Install the main file using the following options:

* Skeleton
	* Meshes: Skeleton meshes
	* Animation Rig Map: Physics Extensions

* Character Creation
	* Character Creation: Racemenu

* Character Creation
	* Weapon Style Randomizer for NPCs: None

* Animation Variants
	* Choose none for all

* First Person Animation
	* Choose none or nothing for all

* Mounted Combat Animation
	* Choose none or nothing for all

* Compatibility Patches
	* Choose none or nothing for all

## Audiovisual - Models & Textures

#### [Arctic - Frost Effects Redux](http://www.nexusmods.com/skyrimspecialedition/mods/29817)

Install the main file using the following options:

* Resolution: Lite
* Color: Realistic hue
* Size: x.5
* Style: Standard
* Plugin option: Frost mesh patch (esl-tagged)

#### [aMidianBorn Book of Silence](https://www.nexusmods.com/skyrim/mods/24909)

Download and install:

* aMidianBorn book of silence_ARMORS
    * Custom
    * Iron and baded: Iron - Vanilla Cut
    * Steel: Steel
    * Steel Plate: Steel Plate
    * Leather: Leather
    * Hide and Studed: Hide
    * Fur: Fur
    * Elven: Gold
    * Dwarwen: Dwarwen
    * Ancient Nord: Ancient Nord
    * Orcish: Orcish
    * Scaled: Scaled
    * Wolf: Wolf - Grey Fur
    * Glass: Glass - Golden
    * Ebony - Ebony - Black
    * Blades: Blades
    * Falmer: Falmer

* aMidianBorn book of silence_Creatures
    * Custom
        * Charrus

* aMidianBorn book of silence_DRAGONBORN DLC
    * Custom
        * Nordic Carved Armor: Black Fur
        * Bonemold Armor
        * Acolyte Masks
        * Ash Spawn
        * Ash Guardians

* aMidianBorn book of silence_UNIQUE ITEMS
    * Custom:
        * Target of the blooded
        * Wuuthrad
        * Savior's hide: Savior's Hide
        * Helm of Yngol
        * Mace of Molag Bal
        * Mehrunez Razor
        * Volendrung
        * Tsun's Armor
        * Ebony Mail: Ebony Mail - Black
        * Staff of Magnus

* aMidianBorn book of silence_WEAPONS
    * Install all weapons

* Bonemold Hotfix
* Staff of Magnus Hotfix

 **Path Fix**

There is an incorrect file path in Book of Silence which needs to be fixed. If the 4K variant is used these steps can be skipped. The 4K variant must be installed manually and is found in the Book of Silence - Dragonborn DLC module.

1. After all files are installed, double-click on the Book of Silence - Dragonborn DLC mod
1. Click on the Filetree tab
1. Expand the file tree textures > actors > dlc02
1. Right-click on the ash folder and select *Rename*
1. Type in the name *ashman* and hit Enter/Return on the keyboard to save the new name
1. Close the window 

**Hide the following files/folders:**

* textures\clothes
* aMidianborn_Skyforge_Weapons.esp

#### [aMidianBorn Blades Armor SSE Patch](http://www.nexusmods.com/skyrimspecialedition/mods/12963)

#### [aMidianBorn stormcloak officer armour](https://www.nexusmods.com/skyrim/mods/45692)

#### [Arri's Snow Elf Ruins Retexture Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/7292)

#### [Barenziah's Glory SE](http://www.nexusmods.com/skyrimspecialedition/mods/6343)

Recommended intall options:

* Desaturated Crown Texture - 1k
* Gamwich Jewelrybox Texture - 1k
* Gamwich Gem Texture - dark

#### [Bellyaches Animal and Creature Pack SSE](http://www.nexusmods.com/skyrimspecialedition/mods/6839)

Recommended install options:
* Options
	* Options: Custom Install

* Custom
	* Bear (brown and black): Bear Replacers
	* Chaurus: None
	* Chicken: Brown
	* Dog: HD Default
	* Dragonfly: Select Nothing
	* Deer: Select Nothing
	* Fox (Red): Red
	* Fox (Arctic): Arctic
	* Frostbite Spider (Brown): None
	* Frostbite Spider (Arctic): None
	* Goat: None
	* Hawk: None
	* Highland Cow: Orange
	* Horker: Grey

* Horse Options
	* Horse Tails: None
	* Horse Textures: None

* More Custom Options
	* Mammoth: None
	* Mudcrab: Grey
	* Rabbit: Rabbit Replacer
	* Sabre Cat (Brown): None
	* Sabre Cat (Arctic): None
	* Skeever (Grey): Mangy - Dark Grey
	* Skeever (Arctic): Mangy - Grey Hooded
	* Wolf (Black): Darker Black
	* Wolf (Ice): White (Brown Eyes)
	* Wolf (Red): Brown
	* Werewolf: Dark Grey
	* Werewolf Eyes: Normal Brown

#### [Bellyaches HD Dragon Replacer Pack (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2636)

#### [Better Dynamic Ash SE](http://www.nexusmods.com/skyrimspecialedition/mods/14644)

#### [Better Dynamic Snow SE](http://www.nexusmods.com/skyrimspecialedition/mods/9121)
In the installer, choose to install SMIM meshes and Snowy Farmhouses. No patches.

#### [Better Dynamic Snow in New Worldspaces](http://www.nexusmods.com/skyrimspecialedition/mods/22741)
Install Better Dynamic Snow in New Areas - ESL. In the installer, chose patches for Falskaar and Wyrmstooth.

#### [BetterFalmerCaveCeilingGlow](http://www.nexusmods.com/skyrimspecialedition/mods/17232)

#### [Book Covers Skyrim (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/901)
Choose whatever options you like, desaturated books are recommended.

#### [Book Covers Skyrim - Lost Library (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/902)
Choose whatever options you like, desaturated books are recommended.

#### [CleverCharff's Photorealistic Ash Pile](http://www.nexusmods.com/skyrimspecialedition/mods/32720)
Install 2K option without bones.

#### [Dark Brotherhood Tenets Restored (SE)](http://www.nexusmods.com/skyrim/mods/31087)
Recommendation: 1K

#### [Deadly Spell Impacts (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/12939)

Recommended install options:

* Options: Custom
* Custom: One Fire Impact (Default)
* One: Fire: Default
* Frost: Alternate 1
* Lightning: Default
	
#### [Deathbell HD](http://www.nexusmods.com/skyrimspecialedition/mods/10755)
Recommendation: 1K

#### [Designs of the Nords SE](https://www.nexusmods.com/skyrimspecialedition/mods/8724/)
In the installer, install optionals if that is desired.

#### [Detailing the Eldrich - Higher-Res Riekling Architecture](http://www.nexusmods.com/skyrim/mods/46741)
Recommendation: Higher Res

#### [Dragon Glyphs HD - Fixed](http://www.nexusmods.com/skyrim/mods/27095)
Recommendation: Dragon Chiseled

#### [Dragon Masks Retextured SE (4K - 2K)](http://www.nexusmods.com/skyrimspecialedition/mods/22699)
Recommendation: 2K

#### [DRAGON PRIEST](http://www.nexusmods.com/skyrimspecialedition/mods/4974)
Recommendation: 2K full option

#### [DRAUGR](http://www.nexusmods.com/skyrimspecialedition/mods/5848)
Recommendation: 2K

#### [DROPS](http://www.nexusmods.com/skyrim/mods/63991)
Install DROPS v1 Optional File. In the installer, choose the *512 x* texture and no alternate textures.

#### [Dust Effects by HHaleyy](http://www.nexusmods.com/skyrimspecialedition/mods/2407)

#### [ElSopa HD - Ants SE](http://www.nexusmods.com/skyrimspecialedition/mods/26715)
Recommendation: 1K

#### [ElSopa HD - Briar Heart](http://www.nexusmods.com/skyrimspecialedition/mods/27983)
Recommendation: red 1k

#### [ElSopa HD - Dirt Blast SE](http://www.nexusmods.com/skyrimspecialedition/mods/22342)
Recommendation: 2K

#### [Embers HD](http://www.nexusmods.com/skyrimspecialedition/mods/14368)
Install using the following options:

* Main Component
	* Embers HD 2k

* Embers HD Fireplaces Add-On Component
	* Fireplaces Add-On

* Embers HD Add-On Components
	* Forges Add-On
	* Lave Crater Add-On

#### [Enhanced Blood Textures SE](http://www.nexusmods.com/skyrimspecialedition/mods/2357)
Download and install the lite version

#### [ETHEREAL CLOUDS - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/2393)
Recommendation: 1K

#### [ETHEREAL COSMOS - Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/5728)
The vivid version is recommended

#### [FALMER](http://www.nexusmods.com/skyrimspecialedition/mods/17224)
Recommendation: 2K

#### [RUSTIC ARMOR and WEAPONS SE](http://www.nexusmods.com/skyrimspecialedition/mods/19666)
Recommendation: 2K

#### [LeanWolf's Better-Shaped Weapons SE](https://www.nexusmods.com/skyrimspecialedition/mods/2017)
Install with the following options:

* All or Custom: Install everything
* Sheath Options:
    * Onehanded sheats
    * Greatsword Sheats
* Variants and Patches
    * FrankFamily HD Imperial Armor and Weapons
    * Keeining with refraction
* Glass
    * Refractive Glass Weapons
* Stalhrim
    * Stalhrim with Refraction
* Dawnbreaker Sheath
    * Dawnbreaker Sheath Elf
* Dawnbreaker ENB
    * Choose if you use ENB or not
* Dragonbone Options
    * DragonBoring Weapons
* Dual Sheath
    * No Dual Sheath
        
#### [Frankly HD Dawnguard Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/19663)
Recommendation: 2K

Install the CBBE patch.

#### [Frankly HD Dragonbone and Dragonscale - Armor and Weapons HQ](https://www.nexusmods.com/skyrimspecialedition/mods/25110)
Recommendation: 2K

Install both main and update file. 

#### [Frankly HD Imperial Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/20848)
Recommendation: 2K

Install the *Pants and Sleeves* patch and the *Better-Shaped Weapons* patch.

#### [Frankly HD Masque of Clavicus Vile](https://www.nexusmods.com/skyrimspecialedition/mods/28565)
Recommendation: 2K

#### [Frankly HD Miraak](https://www.nexusmods.com/skyrimspecialedition/mods/19699)
Recommendation: 2K

Install the CBBE patch.

#### [Frankly HD Nightingale Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/18560)
Recommendation: 2K

Install the CBBE patch and the Better-Shaped Weapons patch.

#### [Frankly HD Shrouded Armor](https://www.nexusmods.com/skyrimspecialedition/mods/18785)
Recommendation: 2K

Choose the color option you prefer

#### [Frankly HD Thieves Guild Armors HQ](https://www.nexusmods.com/skyrimspecialedition/mods/19953)
Recommendation: 2K

#### [GIANT (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/6179)
Recommendation: 2K

#### [Gold Septim - Coins Retex](http://www.nexusmods.com/skyrimspecialedition/mods/1358)
Recommendation: 1K

#### [Greatsword Sheaths and Scabbards Redux SE](http://www.nexusmods.com/skyrimspecialedition/mods/325)
Install options:

* Meshes Type: Meshes - Thin
* Sheath/Scabbard Type: Small - Default Textures
* Skyforge Weapons: Select Nothing

#### [HAGRAVEN](http://www.nexusmods.com/skyrimspecialedition/mods/7679)
Recommendation: 2K

#### [HD Executioners Block SE](http://www.nexusmods.com/skyrimspecialedition/mods/22674)

#### [HD Misc](http://www.nexusmods.com/skyrim/mods/3595)

#### [HD Pondfish](http://www.nexusmods.com/skyrimspecialedition/mods/24731)

#### [HD Reworked Horses](http://www.nexusmods.com/skyrimspecialedition/mods/28249)
Recommendation: 2K-1K

#### [HD Road Signs](http://www.nexusmods.com/skyrimspecialedition/mods/2454)
Recommendation: 2K

Install Main and both Optional files.

#### [HD Stone Quarry and Clay Deposit (SE)](http://www.nexusmods.com/skyrim/mods/38479)
Download and install the 1K Main File.

Hide the following files:

* meshes\_byoh\clutter\resources\claypilem01.nif
* textures\_byoh\clutter\resources\claydeposit01_p.dds
* textures\_byoh\clutter\resources\StoneQuarry01.dds
* textures\_byoh\clutter\resources\StoneQuarry01_N.dds
* textures\_byoh\clutter\resources\StoneQuarry01_P.dds 

#### [High-Res Dartwing (Dragonfly) Texture](http://www.nexusmods.com/skyrim/mods/62809)

#### [High Quality Food and Ingredients SE](http://www.nexusmods.com/skyrimspecialedition/mods/10897)

Choose *custom* in the installer and choose the following:

* Baked Potatoes
* Boiled Creme Treat
* Bone Meal
* Bread
* Carrots
* Charred Skeever Hide and Meat
* Chicken Breast
* Dead Hare
* Dead Pheasant
* Garlic
* Green Apple
* Grilled Chicken Breast
* Grilled Leeks
* Honey Nut Treat
* Long Taffy Treat
* Mead
* Moon Sugar
* Mora Tapinella
* Pie
* Potatoes
* Powered Mannoth Tusk (it's misspelled)
* Raw Beef
* Red Apple
* Salmon Meat
* Salmon Steak
* Salt Pile
* Scaly Photiota
* Seared Slaughterfish
* Slaughterfish Scales
* Sweet Roll
* Venison
* Void Salts

#### [HORNCANDLES](http://www.nexusmods.com/skyrimspecialedition/mods/17285)
Recommendation: 2K-1K

#### [Hybrids HD Plants and Herbs Retexture (SE)](http://www.nexusmods.com/skyrim/mods/1546)
Hide the following files/folders:

* Textures\Plants\FloraNirnroot01.dds
* Textures\Plants\HangingMoss01.dds
* Textures\Plants\MountainFloweringPurple.dds
* Textures\Plants\MountainFloweringPurple_n.dds
* Textures\Plants\Snowberry01.dds
* Textures\Plants\SnowberrySnow01.dds
* Textures\Plants\TundraCotton01.dds 

#### [Iconic's Real Hay](http://www.nexusmods.com/skyrimspecialedition/mods/11133)
Recommendation: 2K alt

#### [Improved closefaced helmets (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/824)

#### [Improved Sparks](http://www.nexusmods.com/skyrimspecialedition/mods/19831)
Recommendation: Grindstones - 10X Sparks and Impact Effects - Vanilla Sparks

#### [Improved Weapon Impact EFFECTS Correct Metal SE](http://www.nexusmods.com/skyrimspecialedition/mods/8936)

#### [Inferno - Fire Effects Redux](http://www.nexusmods.com/skyrimspecialedition/mods/29316)
Recommended install options:

* Main Installation: Core Files
* Resolution Options: Lite
* Glow Options: Normal
* Inferno Flame Color: Freeseia
* Tile Options: New
* Size Options: Regular
* Patch Options: Ember HD
* Patch Options: Select Nothing
* Patch Options: Select Nothing

#### [Just Ice (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/9444)
Recommendation: 2K

#### [LeanWolf's Improved Enchanter Candle Meshes SE](http://www.nexusmods.com/skyrimspecialedition/mods/7883)

#### [Luminous Atronachs](http://www.nexusmods.com/skyrimspecialedition/mods/27732)
Install Luminous Atronachs - ESPLite.

#### [MAMMOTH](http://www.nexusmods.com/skyrimspecialedition/mods/6127)
Recommendation: 2K

#### [Metallurgy - Ingots and Ore HD](http://www.nexusmods.com/skyrimspecialedition/mods/30738)
Recommendation: Metallurgy - Ingots and Ore HD 1K (LOOSE).

#### [MM - REAL ELKS](http://www.nexusmods.com/skyrim/mods/94362)
Recommendation: 2K

#### [New Thinner Torch](http://www.nexusmods.com/skyrim/mods/6950)
Download and install the Ultimate HD Torch by rheadude compatible file. 

#### [Not Really HD Display Case](http://www.nexusmods.com/skyrim/mods/3693)
#### [Not Really HD Keys](http://www.nexusmods.com/skyrim/mods/2875)

#### [Pilgrims Delight](http://www.nexusmods.com/skyrimspecialedition/mods/3273)

#### [Rally's Hooks and Saws](http://www.nexusmods.com/skyrimspecialedition/mods/32652)
Choose one main file, the version with shine is recommended. Fomod recommendation is *default*.

#### [Rally's Instruments HQ](http://www.nexusmods.com/skyrimspecialedition/mods/28193)
Recommendation: Rallys Instruments HQ - Version 2 Vanilla Lute

#### [Real Wood Textures - Farmhouses (SE)](http://www.nexusmods.com/skyrim/mods/50595)
Download and Install the Real Wood Textures - Farmhouses No Green Moss Version Optional File.

Hide the following files/folders:
* textures\architecture\farmhouse\StoneWall01.dds
* textures\architecture\farmhouse\StoneWall01_n.dds
* textures\architecture\farmhouse\WovenFence01.dds
* textures\architecture\farmhouse\WovenFence01_n.dds 

#### [Realistic HD Baskets Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/22199)

#### [Realistic HD Pickaxe Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/20168)

#### [Realistic HD Woodcutter's Axe Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/20239)

#### [Realistic Water Two (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2182)
Choose no optional textures. Choose extended ambiance and patches for *Landscape Fixes for Grass Mods*,  *Falskaar* and *Wyrmstooth*.

#### [Red Dog's Smaller Realistic Ice Spike and Ice Spear](http://www.nexusmods.com/skyrimspecialedition/mods/25519)

#### [Remove Small Rocks](http://www.nexusmods.com/skyrimspecialedition/mods/8733)

#### [Rens HD Shrines (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/13572)
Choose the shrines that you think looks the best, for example:

* Akatosh: Sands of Time
* Arkay: Golden Shells
* Dibella: Springs of Love
* Julianos: Magic Circles
* Kynareth: Heavenly Air
* Mara: Gilded Saint
* Stendarr: Tusk of Mercy
* Talos: Rusted Steel
* Zenithar: Golden Circuit

#### [Retexture for Bread - Hearthfire](http://www.nexusmods.com/skyrim/mods/64980)

#### [Retexture for Soup](http://www.nexusmods.com/skyrim/mods/65238)
Install SMIM Mesh - Poor Version

#### [RUGNAROK - Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/5436)

#### [Ruins Clutter Improved](http://www.nexusmods.com/skyrimspecialedition/mods/5870)
Choose *Install Everything* in the installer. Hide or delete the following files or folders:

* meshes\furniture\workbenches
* meshes\furniture\enchantingworkbench.nif
* meshes\furniture\enchantingworkstation.nif
* meshes\loadscreenart\loadscreenenchantingworkbench.nif
* textures\clutter\candles

#### [High Poly Project](http://www.nexusmods.com/skyrimspecialedition/mods/12029)
In the installer, choose install everything except the Windhelm throne and the patches.

#### [JS Dragon Claws SE](https://www.nexusmods.com/skyrimspecialedition/mods/1394)
Recommendation: 2K

#### [RUSTIC ANIMATED POTIONS and POISONS](http://www.nexusmods.com/skyrimspecialedition/mods/2276)
Recommendation: 1K

#### [RUSTIC AZURA'S STAR - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18345)
Recommendation: 2K

#### [RUSTIC COOKING - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/6142)
Recommendation: 1K

#### [RUSTIC DAEDRA - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/19272)
Recommendation: 2K

#### [RUSTIC DEATH HOUND and GARGOYLE - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/17740)
Recommendation: 2K

#### [RUSTIC DRAGON CORPSE - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/17639)
Recommendation: 2K

#### [RUSTIC ELDERSCROLL - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/17757)
Recommendation: 2K

#### [RUSTIC FROSTBITE SPIDER - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18817)
Recommendation: 2K

#### [RUSTIC NORDIC MURALS](http://www.nexusmods.com/skyrim/mods/65602)
Recommendation: 2K-1K

#### [RUSTIC SOULGEMS - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/5785)
Install *RUSTIC SOULGEMS - Special Edition - FOMOD - English Only*.

In the installer, choose:

* 1k Textures (recommended)
* Sorted + ESL

#### [RUSTIC SPRIGGAN - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18107)
Recommendation: 2K

#### [RUSTIC WINDOWS - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/1937)
Recommendation: 2K

#### [SABRECAT](http://www.nexusmods.com/skyrimspecialedition/mods/5303)
Recommendation: 2K

Install both options in the installer.

#### [SKELETON](http://www.nexusmods.com/skyrimspecialedition/mods/17282)
Recommendation: 2K

Install selecting the Skin, clutter without sounds option. 

#### [Skygazer Moons SSE](http://www.nexusmods.com/skyrimspecialedition/mods/32057)
The *Glow* version (1.2) has some issues which should be fixed in later versions. For now, use the *No Glow* version

#### [Skyrim Redesigned WIP (SE)](http://www.nexusmods.com/skyrim/mods/8954)
Download and install the FOMOD Version and install using the STEP option. 

#### [Skyrim SE Improved Puddles](http://www.nexusmods.com/skyrimspecialedition/mods/1462)
Install *Skyrim SE Improved Puddles FOMOD v1-4 for ENB users*, even if you're not using an ENB.
Choose *2048x2048 Resolution* and *Skyrim Special Edition (all DLCs)* in the installer

#### [Skyrim SE Skill Interface Re-Texture](http://www.nexusmods.com/skyrimspecialedition/mods/1523)
Choose the options you prefer

#### [Skyrim Textures Redone - Enhanced Night Sky](https://www.nexusmods.com/skyrimspecialedition/mods/5561)
Choose the 2k versions of textures, big and small stars. Hide or delete all files from this mod except:

* Textures/sky/skyrimconstellations01.dds
* Textures/sky/skyrimconstellations02.dds
* Textures/sky/skystars.dds

#### [Smooth Sky mesh - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/18350)

#### [Stalhrim](http://www.nexusmods.com/skyrimspecialedition/mods/9447)
Recommendation: 2K

#### [Sweet Mother - The Night Mother Improvement](http://www.nexusmods.com/skyrim/mods/4947)
Recommendation: Sweet Mother HD

#### [The Elder Scrolls V Rewritten - Arvak SE](http://www.nexusmods.com/skyrimspecialedition/mods/11999)
Recommendation: *High Definition* texture size and the *Soul Cairn* model.

#### [TROLL](http://www.nexusmods.com/skyrimspecialedition/mods/4682)
Recommendation: 2K

#### [Ultimate HD Torch](http://www.nexusmods.com/skyrim/mods/28060)
Recommendation: 2K

#### [Vivid Landscapes - Tundra Moss Revised](http://www.nexusmods.com/skyrim/mods/43221)
Recommendation: *Vivid Landscapes - Tundra Moss Revised - yellow 1024* main file and *SMIM compatibility patch* optional file. 

#### [WEBS S.E.](http://www.nexusmods.com/skyrimspecialedition/mods/4873)
Recommendation: 2K

#### [White Phial Replacer SE](http://www.nexusmods.com/skyrimspecialedition/mods/6113)
Recommendation: Install main file and *White Phial Replacer 0.5x size* optional file. 

#### [Whiterun Trellis Redesigned SE](http://www.nexusmods.com/skyrimspecialedition/mods/31905)
Recommendation: 2K

#### [WISPMOTHER](http://www.nexusmods.com/skyrimspecialedition/mods/7638)
Recommendation: 2K-1K

Choose *Full version - skin with a linen fabric cloth* in the installer.

## Audiovisual - Trees & Vegetation

#### [Enhanced Vanilla Trees SE](https://www.nexusmods.com/skyrimspecialedition/mods/11008)
In the installer, choose:

* Enhanced Vanilla Meshes
* Custom Trees (large is recommended)
* Enhanced Tree Clutter
* Skyrim Flora Overhaul - Branches: None
* Alternative Trees: Realistic Aspen Trees
* Greener Bark Textures: Choose nothing

#### [Alpine Forest of Whiterun Valley](https://www.nexusmods.com/skyrimspecialedition/mods/18866)

#### [Bent Pines II](https://www.nexusmods.com/skyrimspecialedition/mods/8306)

#### [Landscape Fixes For Grass Mods](http://www.nexusmods.com/skyrimspecialedition/mods/9005)
Install patches for

* Alternate Start - Live Anothe Life
* Helgen Reborn
* Moon And Star
* JK's Skyrim - Towns
* Arthmoors mods - everything except *Provincial Courier Sevice*

#### [Vanilla HD Tree Branches](https://www.nexusmods.com/skyrimspecialedition/mods/34631)
Install the main file.

## Audiovisual - Sounds & Music

#### [Audio Overhaul for Skyrim SE](http://www.nexusmods.com/skyrimspecialedition/mods/12466)
Do not install any patches. Delete the SKSE folder after installation.

#### [Better Animal Footsteps](https://www.nexusmods.com/skyrim/mods/24805)
Choose to install all footstep sounds. Do not install any patches.

#### [Better Horse Pain Sounds](http://www.nexusmods.com/skyrim/mods/12608)

#### [Heart of the Beast - Werewolf Sound and Texture Overhaul](http://www.nexusmods.com/skyrim/mods/13779)
Recommendation: *Feral Werewolf sounds - HIGH AGGRESSION*.

#### [IHSS - Improved Horse Step Sounds](http://www.nexusmods.com/skyrimspecialedition/mods/848)

#### [Lower Sounding Thieves Guild Door](http://www.nexusmods.com/skyrim/mods/1826)

#### [Realistic wolf howls](http://www.nexusmods.com/skyrim/mods/30636)
Recommendation: *Realistic Wolf Howls more barks than howls*

#### [Sound Hammering Sounds](http://www.nexusmods.com/skyrimspecialedition/mods/5592)

#### [Thundering Shouts (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/14352)
	
#### [Ultra Realistic Bow Shoot Sounds](https://www.nexusmods.com/skyrim/mods/27208)

#### [Ultra Realistic Crossbow Shoot Sounds](https://www.nexusmods.com/skyrim/mods/31274)

## Audiovisual - Creature Skeleton

#### [Absolute Arachnophobia](https://www.nexusmods.com/skyrimspecialedition/mods/24058)

#### [Astounding Flame Atronachs](https://www.nexusmods.com/skyrimspecialedition/mods/24836)

#### [Astonishing Frost Atronachs](https://www.nexusmods.com/skyrimspecialedition/mods/24641)

#### [Bristleback Boars](https://www.nexusmods.com/skyrimspecialedition/mods/22578)

#### [Bullish Bovine](https://www.nexusmods.com/skyrimspecialedition/mods/33888)

#### [Callous Dwemer Centurions](https://www.nexusmods.com/skyrimspecialedition/mods/34395)

#### [Dramatic Deer](https://www.nexusmods.com/skyrimspecialedition/mods/31010)

#### [Dreaded Dwarven Spiders](https://www.nexusmods.com/skyrimspecialedition/mods/27047)

#### [Grandiose Giants](https://www.nexusmods.com/skyrimspecialedition/mods/23889)

#### [Grave Gargoyles](https://www.nexusmods.com/skyrimspecialedition/mods/21907)

#### [Gritty Goats](https://www.nexusmods.com/skyrimspecialedition/mods/26665)

#### [Hardy Hares](http://www.nexusmods.com/skyrimspecialedition/mods/27366)

#### [Heartland Horses](https://www.nexusmods.com/skyrimspecialedition/mods/22083)

#### [Heinous Ash Hoppers](https://www.nexusmods.com/skyrimspecialedition/mods/22409)

#### [Hellish Hounds](https://www.nexusmods.com/skyrimspecialedition/mods/30344)

#### [Honored Hounds](https://www.nexusmods.com/skyrimspecialedition/mods/25563)

#### [Hulking Horkers](https://www.nexusmods.com/skyrimspecialedition/mods/28383)

#### [Immersive Dragons](http://www.nexusmods.com/skyrimspecialedition/mods/18957)

#### [Immersive Smilodons](http://www.nexusmods.com/skyrimspecialedition/mods/18429)

#### [Infamous Ice Wraiths](https://www.nexusmods.com/skyrimspecialedition/mods/29712)

#### [Looming Lurkers](https://www.nexusmods.com/skyrimspecialedition/mods/23122)

#### [Marvelous Mudcrabs](https://www.nexusmods.com/skyrimspecialedition/mods/21685)

#### [Mighty Mammoths](https://www.nexusmods.com/skyrimspecialedition/mods/24237)

#### [Nightmare Chaurus](https://www.nexusmods.com/skyrimspecialedition/mods/21488)

#### [Notorious Netches](https://www.nexusmods.com/skyrimspecialedition/mods/29323)

#### [Riekling Reavers](https://www.nexusmods.com/skyrimspecialedition/mods/22948)

#### [Riekling Roughriders](https://www.nexusmods.com/skyrimspecialedition/mods/22765)

#### [Salty Slaughterfish](https://www.nexusmods.com/skyrimspecialedition/mods/28005)

#### [Savage Bear](https://www.nexusmods.com/skyrimspecialedition/mods/16343)

#### [Sickening Skeevers](https://www.nexusmods.com/skyrimspecialedition/mods/24428)

#### [Sinister Spriggans](https://www.nexusmods.com/skyrimspecialedition/mods/23502)

#### [Supreme Chaurus Hunters](https://www.nexusmods.com/skyrimspecialedition/mods/22263)

#### [Supreme Seekers](https://www.nexusmods.com/skyrimspecialedition/mods/23349)

#### [Supreme Vampire Lords](https://www.nexusmods.com/skyrimspecialedition/mods/19706)
Install *Supreme Vampire Lords XP32 SE*

#### [Tyrannical Trolls](https://www.nexusmods.com/skyrimspecialedition/mods/23665)
Install *Tyrannical Trolls (Vanilla Size)*

#### [Wicked Werewolves](https://www.nexusmods.com/skyrimspecialedition/mods/31757)
Install *Wicked Werewolves SE XP32*.

## Character Appearance - Female body

*This section replaces the vanilla female body with the CBBE body. The CBBE body is chosen because of its versatility. Recommended presets makes the body look realistic or vanilla-ish.*

#### [Caliente’s Beautiful Bodies Enhancer -CBBE-](https://www.nexusmods.com/skyrimspecialedition/mods/198)
*NSFW warning*

Install the main file and the optional file ‘CBBE ESL-flagged .esp’.

In the main installer, choose:

* Body Shape: Slim
* Underwear options: NeverNude
* Outfit options: Vanilla outfits
* SKEE (RaceMenu): RaceMenu Morphs

#### [CBBE Presets Compendium](https://www.nexusmods.com/skyrimspecialedition/mods/11229)
*NSFW warning*

Install the main file

## Character Appearance - Face Parts, textures and overhauls

#### [Argonian Improvements SSE - Horns](https://www.nexusmods.com/skyrimspecialedition/mods/6104)

#### [Beards](http://www.nexusmods.com/skyrimspecialedition/mods/1067)
Choose *Full Install* and *Low: 1024*

#### [Bijin Skin UNP and CBBE SE](https://www.nexusmods.com/skyrimspecialedition/mods/20078)
*NSFW warning*

Install *Bijin Skin CBBE*. Choose default 2K options in the installer.

#### [Brows](http://www.nexusmods.com/skyrimspecialedition/mods/1062)
Choose *Full Install* and *Low: 512*

#### [Consistent Older People](http://www.nexusmods.com/skyrimspecialedition/mods/2977)
Install the loose version

#### [Coverkhajiits (SE)](http://www.nexusmods.com/skyrim/mods/5941)
Install both main files

#### [FAR - Forgotten Argonian Roots (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/1704)
The mod is not packaged correctly for mod managers. To install:

1. Open the archive in MO for installation.
1. Expand FAR-Forgotten Argonian Roots
1. Expand Females → CBBE Body → MAIN texture
1. Drag and drop the Textures folder onto < data > above
1. Expand Males → Better Males body
1. Drag and drop the Textures folder onto < data > above
1. Expand no glow skin → Female
1. Drag and drop the Textures folder onto < data > above
1. Expand no glow skin → Male
1. Drag and drop the Textures folder onto < data > above
1. Untick FAR-Forgotten Argonian Roots and click OK

#### [Female Vampires Have Fangs](http://www.nexusmods.com/skyrimspecialedition/mods/1211)

#### [KS Hairdos SSE](http://www.nexusmods.com/skyrimspecialedition/mods/6817)

#### [More Realistic Hair (SE)](http://www.nexusmods.com/skyrim/mods/3397)
#### [Natural Eyes SSE](http://www.nexusmods.com/skyrimspecialedition/mods/10099)

#### [Northborn Scars (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/720)

#### [RUSTIC CHILDREN (SE)](http://www.nexusmods.com/skyrim/mods/63353)
Recommendation: 2K

#### [Salt and Wind – Rough Hair for KS Hairdos SE](http://www.nexusmods.com/skyrimspecialedition/mods/16582)

#### [Superior Lore-Friendly Hair (SE)](http://www.nexusmods.com/skyrim/mods/36510)
Recommendation: Rough hair, 1K

#### [TDN Equipable Horns SE](http://www.nexusmods.com/skyrimspecialedition/mods/9224)
Yes, some Bosmer have antlers.

*"It is also common among the Bosmer to wear decorative antlers on their foreheads, although rarely, individuals with real, magically-grown antlers can also be encountered."* [source](https://en.uesp.net/wiki/Lore:Bosmer)

Skip this mod if you do not intend to use horns or antlers for your character.

#### [Tempered Skins for Males](http://www.nexusmods.com/skyrimspecialedition/mods/7902)
In the installer you can choose what you like but the following is recommended: A1, B6, C1, D2, E2, no facemarks or scars.

Hide the following files:

* textures\actors\character\argonianmale (entire folder)
* textures\actors\character\khajiitmale\khajiitmalehead_s.dds
* textures\actors\character\male\maleunderwear.dds
* textures\actors\character\male\maleunderwear_n.dds
* textures\armor\briarheart\briarheart.dds
* textures\armor\briarheart\briarheart_n.dds

#### [Vanilla Makeup HD](http://www.nexusmods.com/skyrimspecialedition/mods/24482)
Recommendation: 2K for all races and update file.

#### [Vanilla Warpaints Absolution](http://www.nexusmods.com/skyrimspecialedition/mods/20751)
Recommendation: 2K.

In the installer, choose the following:

* Main Files
	* Vanilla Replacers: 2K vanilla Replacers
	* 2K RaceMenu All-In-One

* Variant Textures
	* Vanilla Variants General Watercolor: None
	* Vanilla Variants Wood Elves Muddy: None
	* Vanilla Variants Dark Elf Ashy: None
	* Vanilla Variants Khajiit Stripes Furry: 2K Furry
	* Vanilla Variants Nord Splattered: None
	* Vanilla Variants Argonian Scaley: 2K Scaley
	* RaceMenu Variants General Watercolor: None
	* RaceMenu Variants Wood Elves Muddy: None
	* RaceMenu Variants Dark Elf Ashy: None
	* RaceMenu Variants Khajiit Stripes Furry: 2K Furry
	* RaceMenu Variants Nord Splattered: None
	* RaceMenu Variants Argonian Scaley: 2K Scaley
	
* SKSE Tintmask Configs
	* None

## Fixes
#### [(SKSE64) Havok Fix](http://www.nexusmods.com/skyrimspecialedition/mods/18160)

#### [1st Person Candlelight Fix](http://www.nexusmods.com/skyrimspecialedition/mods/9736)

#### [Bug Fixes SSE](http://www.nexusmods.com/skyrimspecialedition/mods/33261)

#### [Butterflies Land True](http://www.nexusmods.com/skyrimspecialedition/mods/29434)

#### [Butterflies Unchained](http://www.nexusmods.com/skyrimspecialedition/mods/29538)
Install esl version

#### [Closing time](https://www.nexusmods.com/skyrimspecialedition/mods/34169)

#### [Critters Ain't Snitches](http://www.nexusmods.com/skyrimspecialedition/mods/15134)

#### [Dragon Stalking Fix](http://www.nexusmods.com/skyrimspecialedition/mods/14060)

#### [Enchantment Reload Fix SE](http://www.nexusmods.com/skyrimspecialedition/mods/21055)

#### [Eye Normal Map Fix SSE](http://www.nexusmods.com/skyrimspecialedition/mods/5445)
Install *Eye Normal Map Fix SSE BC7*

#### [Fuz Ro D-oh - Silent Voice](http://www.nexusmods.com/skyrimspecialedition/mods/15109)
Install main and optional files.

The Fuz Ro D'oh.ini file needs to be created and edited manually. To do this:

1. In Mod Organizer, hold Ctrl and double-click the Fuz Ro Doh mod listing.
1. Navigate into the SKSE\Plugins folder.
1. Right-click within the folder and select the menu option New > Text Document.
1. Name the file Fuz Ro D'oh.ini

Open the new file and copy the below contents, pasting them into the file

```
[General]
WordsPerSecondSilence=2
```

Save and close the file.

#### [Hearthfires Houses Building Fix](http://www.nexusmods.com/skyrimspecialedition/mods/27298)

#### [Invisibility and Eyes Mesh Fix](http://www.nexusmods.com/skyrimspecialedition/mods/14464)
Choose *Eyes Mesh Fix* in the installer.

#### [Modern Brawl Bug Fix](http://www.nexusmods.com/skyrimspecialedition/mods/1473)

#### [Skyrim Landscape and Water Fixes](http://www.nexusmods.com/skyrimspecialedition/mods/26138)

In the installer, choose:

* Base Fixed Meshes: Base Meshes
* Main Plugin: 1. ESM
* Patches: Relighting Skyrim
* Walkway Wall FIX: Walkway Wall FIX SMIM

#### [Skyrim Project Optimization SE](http://www.nexusmods.com/skyrimspecialedition/mods/14084)
Choose ESM version

#### [SkyUI SE - Flashing Savegames Fix](http://www.nexusmods.com/skyrimspecialedition/mods/20406)

#### [SSE Engine Fixes (skse64 plugin)](http://www.nexusmods.com/skyrimspecialedition/mods/17230)

1. Download and install *(Part 1) Engine*
1. Download *(Part 2) Engine Fixes - skse64 Preloader and TBB Lib*.
1. Extract the contents of the second archive to the root Skyrim SE directory (i.e. ..\Steam\SteamApps\Common\Skyrim Special Edition\) 
Once installed open and ensure the EngineFixes.ini file is configured:

```
[Patches]
RegularQuicksaves = true
```

Leave the remainder of the settings at their defaults, unless the changes are known and desired.

#### [Stay At The System Page](http://www.nexusmods.com/skyrimspecialedition/mods/19832)

#### [Unlimited Bookshelves (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2885)

#### [Waterbreathing Breathless Emerge SSE](http://www.nexusmods.com/skyrimspecialedition/mods/14485)

#### [Wiseman303's Critter Fixes (SE)](http://www.nexusmods.com/skyrim/mods/54485)
In the installer, choose *Monarch Wing Fix*.

#### [Wiseman303's Flora Fixes](https://www.nexusmods.com/skyrimspecialedition/mods/28197)
Install the main file and the patch for SMIM.

## Gameplay - General

#### [Better Jumping SE](https://www.nexusmods.com/skyrimspecialedition/mods/18967)

#### [GIST - Genuinely Intelligent Soul Trap SE](http://www.nexusmods.com/skyrimspecialedition/mods/15755)
Download and install the Main File and the GIST - Rustic Soul Gems patch Optional File. 

## Gameplay - AI & Combat

#### [AI Overhaul SSE](https://www.nexusmods.com/skyrimspecialedition/mods/21654)

#### [Archery Gameplay Overhaul SE](https://www.nexusmods.com/skyrimspecialedition/mods/24296)

#### [Auto Hide Ammo](http://www.nexusmods.com/skyrimspecialedition/mods/1882)
Install the Simple Auto Unequip Ammo from the Old Files.

#### [Better Stealth AI for Followers](http://www.nexusmods.com/skyrimspecialedition/mods/17600)

#### [Blade and Blunt](https://www.nexusmods.com/skyrimspecialedition/mods/34549)
Install the main file and the optional file.

#### [Follower Trap Safety](http://www.nexusmods.com/skyrimspecialedition/mods/2755)

#### [Realistic AI Detection SE](http://www.nexusmods.com/skyrimspecialedition/mods/2345)
Choose *Realistic AI Detection 2 SE - Medium Interior Medium Exterior*

#### [Run For Your Lives (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2272)

#### [Tavern AI fix](http://www.nexusmods.com/skyrimspecialedition/mods/23107)

## Gameplay - Camping & Survival
The user can choose to use the offical Creation Club Survival Mode or the minimalistic mod The Frozen North.

#### [Camping Lite (Special Edition)](https://www.nexusmods.com/skyrimspecialedition/mods/2370)
>
#### [The Frozen North - Minimalistic survival overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33068)
Do not use this mod if you use Creation Club Survival Mode.

Install the main file *The Frozen North*.

To activate the mod in game, go into Skyrims settings menu, choose gameplay and make sure Survival Mode is ticked. If Survival Mode is missing, follow these instructions to remove the esl-tag from the Frozen North plugin:

1. From Mod Organizer 2, run SSEEdit.
1. The *Module Selection* window opens. Double click on *TheFrozenNorth.esp*.
1. Allow SSEEdit to load.
1. Select *TheFrozenNorth.esp* on the left side of the window.
1. Right click on *Record Flags*on the right side of the window and choose *Edit*.
1. Untick *ESL* and click *OK*.
1. Close SSEEdit and choose to save the changes.

#### [Lenient Survival](https://www.nexusmods.com/skyrimspecialedition/mods/13087)
Only use this mod if you use Creation Club Survival Mode.

Install the main file, the english version.

## Gameplay - Classes & Races

#### [Aetherius - A Race Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/26686)

#### [Class Overhaul Re-Imagined (SkyRem - Cori)](https://www.nexusmods.com/skyrimspecialedition/mods/24808)

#### [Experience](http://www.nexusmods.com/skyrimspecialedition/mods/17751)
Do not activate this mod yet. Wait until you have left the first cell of Alternate Start to avoid getting experience when different mods do their initial setup routines.

#### [Growl - Werebeasts of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/31245)

#### [Sacrosanct - Vampires of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/3928)

## Gameplay - Crafting

#### [Ars Metallica - Smithing Enhancement](https://www.nexusmods.com/skyrimspecialedition/mods/321)

#### [Crafting Skills Revamped]
Download the main file and the following optional files:

* Crafting Skills Revamped - Skyrim Skill Uncapper Patch
* Potions Restore Over Time

## Gameplay - Economy & Item Balance

#### [Trade and Barter](http://www.nexusmods.com/skyrimspecialedition/mods/23081)

## Gameplay - Immersion & Role-playing

#### [Carriage and Ferry Travel Overhaul](http://www.nexusmods.com/skyrimspecialedition/mods/8379)
>
#### [Daedric Voices](https://www.nexusmods.com/skyrimspecialedition/mods/32090)
Install the main file and the Growl patch.

#### [Disease Descriptions for the Immersive Adventurer SE](http://www.nexusmods.com/skyrimspecialedition/mods/26992)

#### [Go On Ahead](http://www.nexusmods.com/skyrimspecialedition/mods/4779)

#### [Guard Dialogue Overhaul SE](http://www.nexusmods.com/skyrimspecialedition/mods/22075)

#### [Immersive Horses](https://www.nexusmods.com/skyrimspecialedition/mods/13402)
Install main file and the 2K horse textures.

#### [Improved Traps](http://www.nexusmods.com/skyrimspecialedition/mods/17592)
Install *Improved Traps and Mining Makes Noise*.

#### [Lock Related Loot](http://www.nexusmods.com/skyrimspecialedition/mods/11342)

#### [Nether's Follower Framework](http://www.nexusmods.com/skyrimspecialedition/mods/18076)
Choose the following default settings in the installer.

#### [No Lockpick Activate (SKSE) - Updated](http://www.nexusmods.com/skyrimspecialedition/mods/26790)

#### [Point The Way (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/352)

#### [Ragdoll Paralysis Redux SE](https://www.nexusmods.com/skyrimspecialedition/mods/13575)

#### [Relationship Dialogue Overhaul - RDO SE](http://www.nexusmods.com/skyrimspecialedition/mods/1187)

#### [Spooky Philter of the Phantom](https://www.nexusmods.com/skyrimspecialedition/mods/32256)

#### [Simple Drop Lit Torches SE](http://www.nexusmods.com/skyrimspecialedition/mods/14490)

#### [Thugs Not Assassins](https://www.nexusmods.com/skyrimspecialedition/mods/34028)
Install the main file and the following optional files:

* Thugs Not Assassins - Book Covers Skyrim Patch
* Thugs Not Assassins - Timing Is Everything

#### [Torches Ignite Oil](http://www.nexusmods.com/skyrimspecialedition/mods/13226)

## Gameplay - Magic & Abilities

#### [Mundus - A Standing Stone Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33411)

#### [Mysticism - A Magic Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/27839)
Install the main file and the Survival patch. Do not install the Audio Overhaul Skyrim patch.

#### [Thunderchild - Epic Shouts and Immersion](http://www.nexusmods.com/skyrimspecialedition/mods/1460)

## Gameplay - Quests & Stories

#### [A Lovely Letter Alternate Routes](https://www.nexusmods.com/skyrimspecialedition/mods/21916)

#### [Alternate Start - Live Another Life - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/272)	

#### [The Brotherhood of Old - Open Beta - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/15322)

#### [The Choice is Yours (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/3850)

#### [Clockwork (SSE)](http://www.nexusmods.com/skyrimspecialedition/mods/4155)

#### [Dawnguard and Clan Volkihar Epilogues](http://www.nexusmods.com/skyrimspecialedition/mods/12098)

#### [The Forgotten City](http://www.nexusmods.com/skyrimspecialedition/mods/1179)

#### [Gildergreen Regrown](http://www.nexusmods.com/skyrimspecialedition/mods/348)

#### [The Gray Cowl of Nocturnal SE](http://www.nexusmods.com/skyrimspecialedition/mods/4509)

#### [The Gray Cowl of Nocturnal SSE - HD pack](http://www.nexusmods.com/skyrimspecialedition/mods/7644)

#### [Gray Cowl of Nocturnal Alikr Flora Overhaul SE](http://www.nexusmods.com/skyrimspecialedition/mods/10141)

#### [Helgen Reborn](http://www.nexusmods.com/skyrimspecialedition/mods/5673)

#### [Improved College Entry - Questline Tweaks](https://www.nexusmods.com/skyrimspecialedition/mods/22184)

#### [Improved Companions - Questline Tweaks](https://www.nexusmods.com/skyrimspecialedition/mods/22300)

#### [Moon and Star](http://www.nexusmods.com/skyrimspecialedition/mods/4301)

#### [Moonpath to Elsweyr SSE](http://www.nexusmods.com/skyrimspecialedition/mods/4341)

#### [More Radiant Quests for the Companions](https://www.nexusmods.com/skyrimspecialedition/mods/24144)
Choose *Option 1* in the installer (suggestion)

#### [Not So Fast - Mage Guild (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/5686)

#### [Not So Fast - Main Quest (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2475)

#### [Save the Icerunner - Lights Out Alternate Routes](https://www.nexusmods.com/skyrimspecialedition/mods/34681)

#### [The Paarthurnax Dilemma](http://www.nexusmods.com/skyrimspecialedition/mods/365)

#### [Timing is Everything SE](http://www.nexusmods.com/skyrimspecialedition/mods/25464)
Install the FISS version.

#### [Even Better Quest Objectives](http://www.nexusmods.com/skyrimspecialedition/mods/159)
In the installer, choose the optional file *Dark Brotherhood Forever to Miscellaneous Quests*. Let the installer choose the rest of the patches.

#### [The Tools of Kagrenac](https://www.nexusmods.com/skyrimspecialedition/mods/14168)

## Gameplay - Skills & Perks

#### [Adamant - A Perk Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/30191)

#### [Lock Overhaul (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/14927)

## User Interface

#### [A Quality World Map](https://www.nexusmods.com/skyrimspecialedition/mods/5804)
Install *8.4 A Quality World Map - Classic with Main Roads Only*. This version is the only one that is properly converted from Skyrim LE.

#### [Better Container Controls for SkyUI](http://www.nexusmods.com/skyrimspecialedition/mods/25271)
Do not install the main file, install the esl optional file only. If you play with a gamepad, skip this mod completely.

#### [Better Dialogue Controls](http://www.nexusmods.com/skyrimspecialedition/mods/1429)

#### [Better Falskaar and Wyrmstooth Map With Roads](https://www.nexusmods.com/skyrim/mods/51339)

#### [Better MessageBox Controls](http://www.nexusmods.com/skyrimspecialedition/mods/1428)

#### [Cathedral Weathers MCM](http://www.nexusmods.com/skyrimspecialedition/mods/24940)

#### [Easy Wheelmenu - SSE Conversion](https://www.nexusmods.com/skyrimspecialedition/mods/22934)

#### [Font Overhaul - Natural Typefaces for Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/2880)

#### [Immersive HUD - iHUD Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/12440)

#### [Lore-Based Loading Screens (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/1185)

#### [MoreHUD Inventory Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18619)

#### [MoreHUD SE](http://www.nexusmods.com/skyrimspecialedition/mods/12688)
Choose the light master version.

#### [RaceMenu](http://www.nexusmods.com/skyrimspecialedition/mods/19080)

#### [Smaller Vanilla Cursors SE](http://www.nexusmods.com/skyrimspecialedition/mods/20617)

#### [Undiscovered Means Unknown - Map Markers](https://www.nexusmods.com/skyrimspecialedition/mods/9762)
In the installer, use the default settings.

#### [UIExtensions](https://www.nexusmods.com/skyrimspecialedition/mods/17561)

#### [Viewable Faction Ranks](http://www.nexusmods.com/skyrimspecialedition/mods/17924)

#### [Whose Quest Is It Anyway](http://www.nexusmods.com/skyrimspecialedition/mods/23581)

#### [Yes Im Sure](http://www.nexusmods.com/skyrimspecialedition/mods/24898)

## Items – Armor, Clothing, & Accessories
*Remember to use both *Cloaks of Skyrim* and *Winter is coming* if you want new cloaks in the game.

#### [Bandolier - Bags and Pouches Classic](http://www.nexusmods.com/skyrimspecialedition/mods/2417)

#### [Black Sacrament Armor](https://www.nexusmods.com/skyrimspecialedition/mods/16687)
Install *Black Sacrament Armour - SSE CBBE BodySlide* and *Black Sacrament Armour - ESL version*. Delete the file *BlackSacramentArmor.esp* (keep *BlackSacramentArmor.esl*).

#### [Cloaks of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/6369)
Install the main version

#### [Cloaks of the Nords](https://www.nexusmods.com/skyrimspecialedition/mods/8886)

#### [Lustmord Vampire Armor](https://www.nexusmods.com/skyrimspecialedition/mods/16676)
Install the main file.

#### [Scout Armor SE](https://www.nexusmods.com/skyrimspecialedition/mods/18910)
This mod needs to be cleaned using the standard cleaning procedure.

#### [Scout Armor SE - Meshes Fix](https://www.nexusmods.com/skyrimspecialedition/mods/26817)

#### [Talos Housecarl Armor Pack](https://www.nexusmods.com/skyrimspecialedition/mods/5540)

#### [Volkihar Knight - Vampire Armor](https://www.nexusmods.com/skyrimspecialedition/mods/4806)

#### [Wayfarer's Coat](https://www.nexusmods.com/skyrimspecialedition/mods/10194)
Install main file and *Wayfarers Coat CBBE UUNP Bodyslide HDT Patch(Installer)*.
In the patch installer, choose *CBBE Bodyslide HDT*.

#### [Winter Is Coming SSE - Cloaks](http://www.nexusmods.com/skyrimspecialedition/mods/4933)
Install main file and the patch for Cloaks of Skyrim.

## Items – Weapons

#### [Animated Armoury - New Weapons with animations SSE Version](https://www.nexusmods.com/skyrimspecialedition/mods/15394)
Download main file and update file.

#### [Artifacts - The Tournament of the ten Bloods](https://www.nexusmods.com/skyrimspecialedition/mods/15264)
In the installer, 2K is recommended.

#### [Faction Crossbows SE](http://www.nexusmods.com/skyrimspecialedition/mods/4047)

#### [Heavy Armory - New Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/6308)

#### [Oblivion Artifact Pack SE](https://www.nexusmods.com/skyrimspecialedition/mods/10644)

#### [Royal Armory - New Artifacts](http://www.nexusmods.com/skyrimspecialedition/mods/6994)

#### [Ruin's Edge](http://www.nexusmods.com/skyrimspecialedition/mods/12792)

#### [The Staff Of Sheogorath](http://www.nexusmods.com/skyrimspecialedition/mods/14468)

#### [Unique Uniques SE](https://www.nexusmods.com/skyrimspecialedition/mods/3334)
Install main file

## New Characters - Enemies

#### [Arena - An Encounter Zone Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33487)

#### [Deadly Dragons](http://www.nexusmods.com/skyrimspecialedition/mods/23723)
Choose Loremonger version with patches for Diverse Dragons, Splender Dragons and Wyrmstooth.

#### [Diverse Dragons Collection SE](http://www.nexusmods.com/skyrimspecialedition/mods/695)

#### [OBIS SE - Organized Bandits In Skyrim Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/4145)
Install main file and OBIS SE Patrols addon.

#### [Splendor – Dragon Variants SE](http://www.nexusmods.com/skyrimspecialedition/mods/9670)

## New Characters - Neutral

#### [DIVERSE SKYRIM SSE](https://www.nexusmods.com/skyrimspecialedition/mods/7707)

#### [Immersive College NPCs](https://www.nexusmods.com/skyrimspecialedition/mods/9252)
Use the default settings in the installer.

#### [Interesting NPCs SE](https://www.nexusmods.com/skyrimspecialedition/mods/29194)
Install BSA version and the hotfix. Install the following optional files:

* Interesting NPCs SE - AI Overhaul SSE Patch
* Interesting NPCs SE - Alternative Locations - Flagged ESL
* Interesting NPCs SE - Cutting Room Floor SSE Patch
* Interesting NPCs SE - Don't Call Me Dragonborn
* Interesting NPCs SE - Karthwasten Patch
* Interesting NPCs SE - Kynesgrove Patch

#### [Interesting NPCs (3DNPC) character Zora Fairchild's voice boosted](http://www.nexusmods.com/skyrimspecialedition/mods/16090)

## New Characters - Allies

#### [Lucien - Fully Voiced Follower](https://www.nexusmods.com/skyrimspecialedition/mods/20035)
Install main file and patches for *Moon and Star* and *Moonpath to Elsweyr*.

#### [INIGO](http://www.nexusmods.com/skyrimspecialedition/mods/1461)

## Audiovisual - Lighting & Weather

#### [Cathedral Weathers and Seasons](http://www.nexusmods.com/skyrimspecialedition/mods/24791)
Install the main file.

#### [Luminosity Lighting Overhaul - The Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/16830)

#### [Obsidian Mountain Fogs](https://www.nexusmods.com/skyrimspecialedition/mods/13539)

#### [Relighting Skyrim - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/8586)

#### [Storm Lightning for SSE](http://www.nexusmods.com/skyrimspecialedition/mods/29243)
In the installer, choose *Skyrim Special Edition* and the latest game version. Choose esl flagged plugin. Recommended settings for halo are as follows:

* Night time sheet halo: Halo with dimmer lighting (level 0)
* Day time sheet halo: Halo dim (level 2)
* Night time fork halo: Halo dimmer (level 1)
* Day time fork halo: Halo dim (level 2)

## Locations - New Structures & Landmarks

#### [Bells of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/10495)

#### [Cutting Room Floor](http://www.nexusmods.com/skyrimspecialedition/mods/276)

#### [Northern Marsh Bridges](https://www.nexusmods.com/skyrimspecialedition/mods/9107/)

#### [Solitude Skyway](http://www.nexusmods.com/skyrimspecialedition/mods/8250)

#### [Solstheim Lighthouse](https://www.nexusmods.com/skyrimspecialedition/mods/14329)
Install *Solstheim Lighthouse v1.2 ESL* and *HD Raven Rock Brick Texture Replacer*

#### [Solstheim - Skaal Fishing Camp](https://www.nexusmods.com/skyrimspecialedition/mods/14450)

#### [Windhelm Lighthouse](http://www.nexusmods.com/skyrimspecialedition/mods/8453)

## Locations - New Lands

#### [Falskaar](http://www.nexusmods.com/skyrimspecialedition/mods/2057)

#### [Midwood Isle SE](https://www.nexusmods.com/skyrimspecialedition/mods/28120)

#### [Wyrmstooth SSE](https://archive.org/details/wyrmstooth1.18SSE)

## Locations - Towns & villages

#### [Darkwater Crossing](https://www.nexusmods.com/skyrimspecialedition/mods/326)

#### [Dawnstar](https://www.nexusmods.com/skyrimspecialedition/mods/13607)

#### [Dragon Bridge](https://www.nexusmods.com/skyrimspecialedition/mods/8683)

#### [Falkreath](https://www.nexusmods.com/skyrimspecialedition/mods/21266)

#### [Helarchen Creek](http://www.nexusmods.com/skyrimspecialedition/mods/4043)

#### [Karthwasten](https://www.nexusmods.com/skyrimspecialedition/mods/350)

#### [Ivarstead](https://www.nexusmods.com/skyrimspecialedition/mods/349)

#### [Keld-Nar](https://www.nexusmods.com/skyrimspecialedition/mods/14353)

#### [Kynesgrove](https://www.nexusmods.com/skyrimspecialedition/mods/351)

#### [Oakwood](http://www.nexusmods.com/skyrimspecialedition/mods/27564)

#### [Rorikstead](https://www.nexusmods.com/skyrimspecialedition/mods/16881)

#### [Shor's Stone](https://www.nexusmods.com/skyrimspecialedition/mods/354)

#### [Soljund's Sinkhole](https://www.nexusmods.com/skyrimspecialedition/mods/358)

#### [Telengard](https://www.nexusmods.com/skyrimspecialedition/mods/17423)

#### [The Fall of Granite Hill](https://www.nexusmods.com/skyrimspecialedition/mods/22512)

#### [Whistling Mine](https://www.nexusmods.com/skyrimspecialedition/mods/367)

## Locations - Overhauls

#### [Bring Out Your Dead (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/323)

#### [Castle Volkihar Rebuilt - SSE](https://www.nexusmods.com/skyrimspecialedition/mods/324)

#### [Immersive Dawnguard Dayspring Pass SE](http://www.nexusmods.com/skyrimspecialedition/mods/4126)

#### [JK's Arcadia's Cauldron](https://www.nexusmods.com/skyrimspecialedition/mods/33565)

#### [JK's The Bannered Mare.](https://www.nexusmods.com/skyrimspecialedition/mods/33845)

#### [JK's Belethor's General Goods.](https://www.nexusmods.com/skyrimspecialedition/mods/33636)

#### [JK's Dragonsreach](https://www.nexusmods.com/skyrimspecialedition/mods/34000)

#### [JK's The Drunken Huntsman.](https://www.nexusmods.com/skyrimspecialedition/mods/33783)

#### [JK's Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/6289)
Install main file and the following patches:

* JK's Skyrim - Arthmoor's Patch Pack
    * Choose individual patches and let the installer choose patches for you.
* JK's Skyrim - Carriage and Ferry Travel (CFTO) Patch
* JK's Skyrim - Clockwork Patch
* JK's Skyrim - Realistic Water Two Patch
* JK's Skyrim - Thunderchild Patch

#### [Smooth Shores](http://www.nexusmods.com/skyrimspecialedition/mods/10624)

#### [Tactical Valtheim SSE](https://www.nexusmods.com/skyrimspecialedition/mods/9101)
In the installer. choose *Radiant Exclusions*.

#### [Farmhouse Chimneys SE](http://www.nexusmods.com/skyrimspecialedition/mods/8766)
The installer auto detects which mods you have installed and automatically chosses the correct patches. Do not install any *Alternative Toppers* unless you prefer them.

#### [Obscure's College of Winterhold](https://www.nexusmods.com/skyrimspecialedition/mods/20514)
The installer will automatically choose the correct patches to use.

#### [Lanterns Of Skyrim II](http://www.nexusmods.com/skyrimspecialedition/mods/30817)
In the installer, choose no addons. Choose *the LoS II - SMIM patch* in the installer. The installer will automatically select all other patches you need.

Install the optional *Lanterns Of Skyrim II - Midwood Isle patch*

## ENB

#### [ENB](http://enbdev.com/download_mod_tesskyrimse.htm)
Download the latest version by clicking on the version number in the lower left side of the screen. This open a new page that has the download link on the bottom.

Open the downloaded archive and extract the files 'd3d11.dll* and *d3dcompiler_46e.dll* to the main game folder.

#### [ENB Helper SE](https://www.nexusmods.com/skyrimspecialedition/mods/23174)

#### [A Cathedralist's ENB](https://www.nexusmods.com/skyrimspecialedition/mods/25296)
Download *A Cathedralist's ENB* or *A Cathedralist's ENB - High Quality*. Extract the contents of the downloaded archive to the main game folder.

Download *Reduced Mist Brightness* and install as a normal mod.

## Patches

#### [Better Dynamic Majestic Mountains](http://www.nexusmods.com/skyrimspecialedition/mods/20102)

#### [College of Winterhold The Missing Apprentices Quest Fix](https://www.nexusmods.com/skyrimspecialedition/mods/6677)

#### [Falskaar - Addons and Patches](http://www.nexusmods.com/skyrimspecialedition/mods/19454)
Choose

* Bug Fixes
* Boat Location Patch
* Fast Travel Addon
* Unique Region Names Addon

#### [JS Dragon Claws - Patches](https://www.nexusmods.com/skyrimspecialedition/mods/23833)
Install:

* JS Dragon Claws - Amethyst Patch
* JS Dragon Claws - Helgen Reborn Patch
* JS Dragon Claws - Wyrmstooth Patch

#### [kryptopyr's Patch Hub](https://www.nexusmods.com/skyrimspecialedition/mods/19518)
Install *Book Covers Skyrim __ TCIY* and *Cutting Room Floor __ TCIY*.

#### [Luminosity - A Quality Worldmap Compatibility Patch](https://www.nexusmods.com/skyrimspecialedition/mods/30162)

#### [Moonpath to Elsweyr Sky and Lightning fix](http://www.nexusmods.com/skyrimspecialedition/mods/18683)

#### [Unofficial Moonpath to Elsweyr Patch](http://www.nexusmods.com/skyrimspecialedition/mods/15882)

#### [Unofficial Skyrim Creation Club Content Patch](https://www.nexusmods.com/skyrimspecialedition/mods/18975)
Only use this mod if you use the Creation Club Survival Mode.

In the installer, choose the default option. The installer will identify the mods you use.

#### [Dread's modlist patches](https://github.com/dreadflopp/dreads_modlist_patches)

To download, click the button *Clone or download* and choose *download zip*.

The fomod installer will automatically select all mods you use. Select the tweaks you want to use.

If you have chosen to install ENB tweaks, these will have to be manually moved to the main game folder.

1. In Mod Organizer 2, right click on the just installed mod, *Dread's modlist patches*, and choose to open in explorer.
1. In the explorer window, navigate to *ENB Tweaks* and then to the chosen ENB preset.
1. Move the file *enbseries.ini* and the folder *enbseries* to the main game folder, overwriting the files installed by the ENB.

## Utilities

#### [BodySlide and Outfit Studio](https://www.nexusmods.com/skyrimspecialedition/mods/201)

Download and install as a normal mod.

**Instructions to add tool as executable**

1. In Mod Organizer 2, click in the *Data* tab
1. Right click on *CalienteTools\BodySlide\BodySlide x64.exe* and choose *Add as Executable*.
1. A dialog box opens asking for a name of the executable. Accept the default name by clicking *OK*.

#### [Nemesis](https://github.com/ShikyoKira/Project-New-Reign---Nemesis-Main/releases)
Download latest SSE version and install as a normal mod.

**Instructions to add tool as executable**

1. In Mod Organizer 2, click in the *Data* tab
1. Right click on *Nemesis_Engine\Nemesis Unlimited Behavior Engine.exe* and choose *Add as Executable*.
1. A dialog box opens asking for a name of the executable. Accept the default name by clicking *OK*.

# Post Installation: Final steps

## Create output data listings

Some tools used during the post installation steps outputs data. To keep the data seperated, output mod listings will be created.

**Instructions to create output data mods**

Create a seperator to keep things tidy:

1. Right click in the mods section of Mod Organizer 2.
1. Select *All Mods/Create Seperator*.
1. Name the seperator *Output Data*.

Create the output data folders

1. Right click in the mods section of Mod Organizer 2.
1. Select *All Mods/Create empty mod*.
1. Name the mod.

Repeat step 1-3 above and create the following empty mods:

* TextGen_Output
* DynDOLOD_Output
* Nemesis_Output
* BodySlide _Output
* Unlimited_Bookshelves_Patch_Generator_Output

Some tools can be set to output data to these mods.

1. Click the Executables button at the top of the main Mod Organizer window.
1. Select the tool to add an argument to.
1. Input argument in the Argument field.
1. Click the Apply button.

Repeat the steps for the tools listed below. Arguments should be seperated by spaces.

* Textgen SE: **-o:C:\Modding\Tools\Mod Organizer 2\mods\TextGen_Output**
* Dyndolod SE: **-o:C:\Modding\Tools\Mod Organizer 2\mods\DynDOLOD_Output**

Users that deviate from the recommended install paths need to adjust the instructions accordingly.

To set BodySlide to output data to its output mod:

1. Run BodySlide x64 through Mod Organizer
1. Click *Settings*
1. Click *Advanced*
1. Click *Browse* and browse to the *BodySlide _Output* folder.
1. Click *Select folder*
1. Click *OK* and close BodySlide

## Sorting and cleaning the new load order

Before moving on, sort the load order with LOOT. Take note of any plugins that LOOT reports as needing to be cleaned and perform the standard cleaning procedures on these mods. Ignore any reported missing compatibility patches. The guides patches take care of all the patching, thus eliminating the need for those additional plugins.

## Generating body and armor meshes

Build body and armor meshes using BodySlide following these instructions:

1. Run BodySlide x64 through Mod Organizer
1. In the *Outfit/Body* dropdown menu, choose *CBBE NeverNude* (this will also prevent NSFW images).
1. In the preset menu, choose what suits you. The preset you choose should end with the word ‘outfit’. I recommended the presets *Pear (outfit), Natural (outfit), CBBE Slim (outfit), UNP Natural (outfit), Thief (outfit)* or *Warrior (outfit)*.
1. Tick the checkbox *Build Morphs*.
1. Click the button *Build* to build the body.
1. Click on the spyglass at the field Group filter and choose *Choose groups*.
1. Check the following and click ok: *Black Sacrament, CBBE vanilla outfits, Frankly HD, Lustmord, WTF Wayfare Coat CBBE*.
1. Click the button *Batch build…*
1. Click *build* to build armor meshes.
1. Make sure no physics options are checked. Check all Frankly options. Click *ok* and close BodySlide.
1. Right click any mod in Mod Organizer 2 and choose *All Mods/Refresh*.
1. Ensure the BodySlide_Output mod is active (checked).

## Generating Animation Files
Once Nemesis is installed, the animation files need to be generated.

1. Sort the load order with LOOT.
1. Run Nemesis Unlimited Behaviour Engine via Mod Organizer 2.
1. Check the boxes adjacent to *Animated Armoury FPA* and *Archery Gameplay Overhaul*.
1. Click *Update Engine* and wait for the update to finish.
1. Click *Launch Nemesis Behaviour Engine* and wait for the generation to finish indicated by the message *Behaviour generation complete*.
1. Close Nemesis.

After closing Nemesis, there will be files in Overwrite:

1. Double-click on Overwrite. A window will open.
1. Drag the following folders and files from Overwrite to Nemesis_Output:
    * meshes
    * Nemesis_Engine
    * scripts
    * FNIS.esp
1. Close the window.
1. Ensure the Nemesis_Output mod is active (checked).

Nemesis may have generated a new plugin, *FNIS.esp*. Activate it and sort all plugins using LOOT.

## Generating Unlimited Bookshelves patch

1. Sort the load order with LOOT
1. Run SSEEdit via Mod Organizer 2.
1. Make sure all plugins are selected and click ok.
    - A second window asking the user to select modgroups might show up. Simply click *ok*.
1. Wait for SSEEdit to load. It may take a couple of minutes.
1. Right-click in the tree view on the left side of the window. Choose *Apply Script*.
1. Choose *Unlimited Bookshelves Patch Generator* and click *ok*.
1. Anytime the script asks whether a file should be added as a master, click on *ok*".
1. When the scipt is finished, close SSEEdit and make sure that the new patch is saved.

After closing SSEEdit, the patch will be in Overwrite:

1. Right-click Overwrite and select Create Mod
1. Name it *Unlimited Bookshelves Patch* and click *ok*.
    - This will create a new mod listing in the left pane for the FNIS SE generated files. 
1. Check the new mod entry to enable it.

1. Double-click on Overwrite. A window will open.
1. Drag the file *UnlimitedBookshelvesPatch.esp* from Overwrite to Unlimited_Bookshelves_Patch_Generator_Output.
1. Close the window.
1. Ensure the Unlimited_Bookshelves_Patch_Generator_Output mod is active (checked).

## DynDOLOD

### Run TextGen

1. Run TexGen from the MO2 executable drop-down list.
1. Keep the default output location and and choose one of the follow two options:
    1. Option 1: Keep the default settings. This is for the average system.
    1. Option 2: Users who have the a bit more performance room, change the *LOD Texture Size* to *512*. This will result in higher resolution LOD textures. 
1. Once the option has been chosen click Start.
1. Once the completed message has appeared, click *Save & Exit*.
1. Right click any mod in Mod Organizer 2 and choose *All Mods/Refresh*.
1. Ensure the TexGen_Output mod is active (checked).

### Run DynDOLOD

1. Open the root DynDOLOD folder (i.e., ..\Modding\Tools\DynDOLOD\).
1. Open the DynDOLOD_SSE.ini file (i.e., ..\DynDOLOD\Edit Scripts\DynDOLOD\DynDOLOD_SSE.ini)
1. Set *TreeLOD=0*
1. Set *TreeFullFallBack=0*. 
1. Open the DynDOLOD_SSE_childworldlod_Tamriel.txt file (i.e., ..\DynDOLOD\Edit Scripts\DynDOLOD\DynDOLOD_SSE_childworldlod_Tamriel.txt)
1. Add the following lines:
    ````
    JKs Skyrim.esp;00023840;MrkCWextTowerPlatform01
    JKs Skyrim.esp;00001FA9;MrkCWextTowerPlatform01
    JKs Skyrim.esp;00002033;MrkCWextTowerPlatform01
    JKs Skyrim.esp;00001FE3;MrkCWextTowerPlatform01
    ````
1. Run DynDOLOD from the MO2 executable drop-down list.
1. Select all worldspaces.
1. Ensure the *Candles, FXGlow, Generate static LOD, Windows,* and *High* boxes are checked.
1. Keep the default Output location and settings, click *High preset* button, and run it. This takes ~40 minutes.
1. Once the completed message has appeared, click Save & Exit.
1. Right click any mod in Mod Organizer 2 and choose *All Mods/Refresh*.
1. Ensure the DynDOLOD Output mod is active (checked).
1. Ensure the DynDOLOD esm and esp files are checked in the right pane.
1. Sort with LOOT.
1. Ensure DynDOLOD.esp is the last plugin in the load order.

# Mod Configuration (MCM)

These are suggested settings. It is recommended to tweak these settings yourself.

## AGO (Archery Gameplay Overhaul)

* Turn off *Arm Fatigue*

## Cathedral Weather

* Turn off *Configuration Spell*

## Farmhouse Chimneys

Under *Mod Support*, turn on support for all Arthmoor's villages. Turn on support for *Helarchen Creek*, *Oakwood* and *Cutting Room Floor*.

## Immersive Hud

Turn on *Key press toggles*.

## Lock Overhaul

Activate the mod

## More Hud

Under *Enemy's Level*, turn off *Show Magicka Meter* and *Show Stamina Meter*.

## OBIS

Enable the mod. Under *Special*, enable *Minotaurs* and *Spiders*.

## OBIS - Patrols

Enable the mod.

## Realistic Water Two

Enable *Blacksmith Forge Water* for *The Fall of Granite Hill, *Kynesgrove* and *Rorikstead*. After Granite Hill has been destroyed, uncheck the option for it.