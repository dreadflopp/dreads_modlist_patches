# Where to find the guide
The Github version (this version) of the guide is the first version to get updates but the Mod Picker version should mirror the Github version. The Github version has extended comments and users should at least read through the Github version of the guide.
- [Github version of the guide](https://github.com/dreadflopp/dreads_modlist_patches/blob/master/README.md)
- [Mod Picker version]()
- [The guide section on STEP]()

# Introduction
This modlist a build for the [STEP: Core guide for Skyrim Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/31054). This means that this guide is based on the STEP Core build. Everything you need is in this guide, you do not have to install anything prior following this guide. Almost everything in this build is optional, meaning you can use parts of it if that is what you want.

**The mods featured in this build are chosen to be immersive and realistic. Realistic in a fantasy setting means believable. The mods should feel like they expand or enhances vanilla Skyrim, like they could have been there from the beginning**

**This build is made to be easy to install**
- No LOOT rules, every conflict is resolved with the patches. Run LOOT and you are done.
- No bashed patch. Every level list conflict is fixed in the patches.
- No merging of mods. Every patch is esl-flagged to make sure the plugin limit count is not reached.
- Advanced fomod installer for the patches. No need to actively choose patches, the fomod does the work for you.

Visit the [STEP forums](https://forum.step-project.com/topic/14603-dreads-step-se-core-addon/)  if you have any questions.

**With this modular STEP build you will get**
- New weapon textures
- New armors
- New weapons
- Realistic female body compatible with popular skin and armor mods
- Overhauled skills and perks
- Overhauled magic, races, standing stones, werewolves and vampires
- New, tougher bandits, dragons and enemies
- New NPC's and followers
- New experience system with slower leveling
- New class system
- New lands and quests
- New and altered towns and villages
- Lightweight survival mod, the survival mod from Bethesda Creation Club.
- Enhanced Lighting For ENB is replaced by Luminosity that has increased ambient lighting for those that think ELE is too dark.
- Bigger trees for truly immersive forrests
- …more

**The STEP guide is in beta and this mod list will remain in beta/WIP for as least as long as STEP is in beta. For now, consider this a work in progress.**

The patches comes with a neat FOMOD installer that automatically chooses what to install. The patches consists of a huge bunch of esl-flagged plugins. Since they are esl-flagged you do not have to worry about the old plugin count limit. Keeping the patches separated in different plugins helps during development when adding, testing and replacing mods. This also makes this mod list mostly modular. There are a few exceptions:
- You need to use the Unofficial Skyrim Special Edition Patch
- Cloaks of Skyrim and Winter is coming should be used together or not at all for the patches to work.


Note that records from the Particle patch is not forwarded since the plugin is obsolete. ENB users should use [ENB Helper](https://www.nexusmods.com/skyrimspecialedition/mods/23174)

**Acronyms that are used in the guide:**\
USSEP = Unofficial Skyrim Special Edition Patch\
WACCF = Weapons, Armor, Clothing & Clutter Fixes\
CCOR = Complete Crafting Overhaul Remade\
CFTO = Carriage and Ferry Travel Overhaul\
SMIM = Static Mesh Improvement Mod\
ICAIO = Immersive Citizens – AI Overhaul\


# Game & Tool Installation
>TODO

# Tool Configuration
>TODO

# Cleaning Vanilla Master Files 
>TODO

# DynDOLOD
>TODO

# Mod Configuration (MCM)
>TODO

# BethINI Customization 
>TODO

# Instructions
>TODO Revise
1. Install STEP SE: Core but do not install the STEP patch.
2. Install xEdit https://www.nexusmods.com/skyrimspecialedition/mods/164 and add it as an executable in Mod Organizer.
3. Install my mod list and place the mods after the STEP guide, letting my listed mods overwrite the STEP guide and DynDOLOD resources. When you install mods, always install the main file and update files if you are not explicitly told not to.
4. Run LOOT.
5. Run DynDOLOD following the instructions from the STEP guide,
6. Run FNIS and check the box for TK Dodge / Ultimate combat if any of those mods are used. Instructions are in the STEP guide.
5. Build body and armor meshes using BodySlide following these simple instructions:
>1. Run BodySlide through Mod Organizer
>2. In the *Outfit/Body* dropdown menu, choose *CBBE NeverNude* (this will also prevent NSFW images).
>3. In the preset menu, choose what suits you. The preset you choose should end with the word ‘outfit’. I recommended the presets *Pear (outfit), Natural (outfit), CBBE Slim (outfit), UNP Natural (outfit), Thief (outfit)* or *Warrior (outfit)*.
>4. Tick the checkbox *Build Morphs*.
>5. Click the button *Build* to build the body.
>6. Click on the spyglass at the field Group filter and choose *Choose groups*.
>7. Check the following and click ok: *CBBE vanilla outfits, Frankly HD, Immersive Armors SSE CBBE, WACCF*.
>8. Click the button *Batch build…*
>9. Click *build* to build armor meshes.
>10. Make sure no physics options are checked. Check all Frankly options. Click *ok* and close BodySlide. The meshes that has been built are placed in Mod Organizers overwrite folder and can be moved to a new mod folder if you choose to.
6. Install the mod [Unlimited Bookshelves Patch Generator](http://https://www.nexusmods.com/skyrimspecialedition/mods/19160). Follow the instructions on the Nexus page to build an Unlimited Bookshelves patch.

# The mod list

## Extenders
#### [SKSE64](http://www.nexusmods.com/skyrimspecialedition/mods/30379)
**Root Files Installation**
1. Download the most current archive for Skyrim SE.
2. Open the downloaded archive and extract the following files to the Skyrim Special Edition folder: (..\Steam\steamapps\common\Skyrim Special Edition\) 
    - skse64_X_X_X.dll
    - skse64_loader.exe
    - skse64_steam_loader.dll 

**Data Files Installation**
1. Open MO2 and right-click on the mod list.
2. Hover over All Mods and select Create empty mod.
3. Type in SKSE64, or anything similar.
4. Hold down the Ctrl key and double-click on the newly created mod in the mod list.
5. Keep this folder open for the next two steps below. 

**INI File**
1. In the new Explorer window, create a new folder named SKSE
2. Open that folder and create a new file named SKSE.ini
3. Open the new file and copy and paste the code in the box below
4. Save and close the file.
```
[Display]
iTintTextureResolution=2048

[General]
ClearInvalidRegistrations=1
```

**Scripts**
1. From the archive downloaded above, open the Data folder (..\skse64_X_X_X\Data\)
2. Extract the Scripts folder to the mod's folder.

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
>TODO install instructions
#### [Cathedral - Plants](http://www.nexusmods.com/skyrimspecialedition/mods/26104)
#### [Skyrim Realistic Overhaul](http://www.moddb.com/mods/skyrim-realistic-overhaul)
- Install Part 1-3, choosing to merge the files when asked.
- Install the update file, choosing to merge as well.
#### [Majestic Mountains - Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/11052)
Install a main file and a lod file, choose the version you like the most.
Main installer:
- Snow Mountain Type: Snow Mountain New version ESL
- Optionals: Moss Rocks ESL Version
- Sun Direction (choose one or none): None
- Compatibility Patches: SMIM
LOD installer:
- LOD Resolution: 1024 (2-4GB Vram)
#### [Cathedral landscapes](https://www.nexusmods.com/skyrimspecialedition/mods/21954)
In the installer, choose:
- Full Install, Brown Tundra
- Blended Roads
#### [Weapons Armor and Clothing - Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/20199)
Choose CBBE in the installer if you use CBBE.
Hide or delete the file _CalienteTools\BodySlide\ShapeData\CBBE Vanilla\Body\Ebony.nif_ since this mesh is causing issues.
#### [RUSTIC CLOTHING - Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/4703)
Recommendation: 2K
#### [Unofficial Material Fix](http://www.nexusmods.com/skyrimspecialedition/mods/21027)

## Audiovisual
### Audiovisual - Animations & Effects
#### [D13 Faster GET UP STAND UP Animation](http://www.nexusmods.com/skyrimspecialedition/mods/5890)
Install loose files
#### [No Spinning Death Animation (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/1432)
Install *No Spinning Death Animation MERGED*
#### [No Spinning Death Animation MERGED](http://www.nexusmods.com/skyrimspecialedition/mods/15881)
#### [XP32 Maximum Skeleton Special Extended - XPMSSE](http://www.nexusmods.com/skyrimspecialedition/mods/1988)
Install the main file using the following options:\
**Skeleton**
- Meshes: Skeleton meshes
- Animation Rig Map: Physics Extensions

**Character Creation**
- Character Creation: Racemenu

**Character Creation**
- Weapon Style Randomizer for NPCs: None

**Animation Variants**
- Choose none for all

**First Person Animation**
- Choose none or nothing for all

**Mounted Combat Animation**
- Choose none or nothing for all

**Compatibility Patches**
- Choose none or nothing for all

### Audiovisual - Models & Textures
#### [Arctic - Frost Effects Redux](http://www.nexusmods.com/skyrimspecialedition/mods/29817)
Install the main file using the following options:\
>TODO
#### [Armor and Clothing Extension](http://www.nexusmods.com/skyrimspecialedition/mods/19002)
Recommendation: 2K
#### [Barenziah's Glory SE](http://www.nexusmods.com/skyrimspecialedition/mods/6343)
Recommended intall options:\
- Desaturated Crown Texture - 1k
- Gamwich Jewelrybox Texture - 1k
- Gamwich Gem Texture - dark
#### [Bellyaches Animal and Creature Pack SSE](http://www.nexusmods.com/skyrimspecialedition/mods/6839)
Recommended install options:\
**Options**
- Options: Custom Install

**Custom**
- Bear (brown and black): Bear Replacers
- Chaurus: None
- Chicken: Brown
- Dog: HD Default
- Dragonfly: Select Nothing
- Deer: Select Nothing
- Fox (Red): Red
- Fox (Arctic): Arctic
- Frostbite Spider (Brown): None
- Frostbite Spider (Arctic): None
- Goat: None
- Hawk: None
- Highland Cow: Orange
- Horker: Grey

**Horse Options**
- Horse Tails: None
- Horse Textures: None

**More Custom Options**
- Mammoth: None
- Mudcrab: Grey
- Rabbit: Rabbit Replacer
- Sabre Cat (Brown): None
- Sabre Cat (Arctic): None
- Skeever (Grey): Mangy - Dark Grey
- Skeever (Arctic): Mangy - Grey Hooded
- Wolf (Black): Darker Black
- Wolf (Ice): White (Brown Eyes)
- Wolf (Red): Brown
- Werewolf: Dark Grey
- Werewolf Eyes: Normal Brown

#### [Bellyaches HD Dragon Replacer Pack (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2636)
#### [Better Dynamic Ash SE](http://www.nexusmods.com/skyrimspecialedition/mods/14644)
#### [Better Dynamic Snow SE](http://www.nexusmods.com/skyrimspecialedition/mods/9121)
In the installer, choose to install SMIM meshes and Snowy Farmhouses. No patches.
#### [BetterFalmerCaveCeilingGlow](http://www.nexusmods.com/skyrimspecialedition/mods/17232)
#### [Book Covers Skyrim (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/901)
Choose whatever options you like, desaturated books are recommended.
#### [Book Covers Skyrim - Lost Library (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/902)
Choose whatever options you like, desaturated books are recommended.
#### [CleverCharff's Photorealistic Ash Pile](http://www.nexusmods.com/skyrimspecialedition/mods/32720)
#### [Dark Brotherhood Tenets Restored (SE)](http://www.nexusmods.com/skyrim/mods/31087)
Recommendation: 1K
#### [Deadly Spell Impacts (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/12939)
Recommended install options:\
**Options**
- Options: Custom

**Custom**
- One Fire Impact (Default)

**One**
- Fire: Default

**Frost**
- Alternate 1

**Lightning**
- Default
#### [Deathbell HD](http://www.nexusmods.com/skyrimspecialedition/mods/10755)
Recommendation: 1K
#### [Detailing the Eldrich - Higher-Res Riekling Architecture](http://www.nexusmods.com/skyrim/mods/46741)
Recommendation: Higher Res
#### [Divine Amulets and Daedric Rings](http://www.nexusmods.com/skyrim/mods/92542)
Install main and optional files
#### [Dragon Glyphs HD - Fixed](http://www.nexusmods.com/skyrim/mods/27095)
Recommendation: Dragon Chiseled
#### [Dragon Masks Retextured SE (4K - 2K)](http://www.nexusmods.com/skyrimspecialedition/mods/22699)
Recommendation: 2K
#### [DRAGON PRIEST](http://www.nexusmods.com/skyrimspecialedition/mods/4974)
Recommendation: 2K full option
#### [Dragonbone Mastery - Weapons Retexture](http://www.nexusmods.com/skyrimspecialedition/mods/2056)
>TODO Check options and overwrites/conflicts
#### [DRAUGR](http://www.nexusmods.com/skyrimspecialedition/mods/5848)
Recommendation: 2K
#### [DROPS](http://www.nexusmods.com/skyrim/mods/63991)
#### [Dust Effects by HHaleyy](http://www.nexusmods.com/skyrimspecialedition/mods/2407)
#### [EASIER LOCKPICKING (SE)](http://www.nexusmods.com/skyrim/mods/53071)
#### [ElSopa HD - Ants SE](http://www.nexusmods.com/skyrimspecialedition/mods/26715)
Recommendation: 1K
#### [ElSopa HD - Briar Heart](http://www.nexusmods.com/skyrimspecialedition/mods/27983)
Recommendation: red 1k
#### [ElSopa HD - Dirt Blast SE](http://www.nexusmods.com/skyrimspecialedition/mods/22342)
Recommendation: 2K
#### [Embers HD](http://www.nexusmods.com/skyrimspecialedition/mods/14368)
Install using the following options:\
**Main Component**
- Embers HD 2k

**Embers HD Fireplaces Add-On Component**
- Fireplaces Add-On

**Embers HD Add-On Components**
- Forges Add-On
- Lave Crater Add-On

**Embers HD Compatibility Patches**
- Campfire

#### [Enhanced Blood Textures SE](http://www.nexusmods.com/skyrimspecialedition/mods/2357)
>TODO Switch to lite version
#### [ETHEREAL CLOUDS - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/2393)
Recommendation: 1K
#### [FALMER](http://www.nexusmods.com/skyrimspecialedition/mods/17224)
Recommendation: 2K
#### [Frankly HD Dawnguard Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/19663)
Recommendation: 2K\
Install the CBBE patch.
#### [Frankly HD Dragonbone and Dragonscale - Armor and Weapons HQ](https://www.nexusmods.com/skyrimspecialedition/mods/25110)
Recommendation: 2K\
Install both main and update file. 
#### [Frankly HD Imperial Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/20848)
Recommendation: 2K\
Install the *Pants and Sleeves* patch and the *Better-Shaped Weapons* patch.
#### [Frankly HD Masque of Clavicus Vile](https://www.nexusmods.com/skyrimspecialedition/mods/28565)
Recommendation: 2K
#### [Frankly HD Miraak](https://www.nexusmods.com/skyrimspecialedition/mods/19699)
Recommendation: 2K\
Install the CBBE patch.
#### [Frankly HD Nightingale Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/18560)
Recommendation: 2K\
Install the CBBE patch and the Better-Shaped Weapons patch.
#### [Frankly HD Shrouded Armor](https://www.nexusmods.com/skyrimspecialedition/mods/18785)
Recommendation: 2K\
Choose the color option you prefer
#### [Frankly HD Thieves Guild Armors HQ](https://www.nexusmods.com/skyrimspecialedition/mods/19953)
Recommendation: 2K\
#### [Gemling Queen Jewelry SE](http://www.nexusmods.com/skyrimspecialedition/mods/4294)
Install instructions:\
**Main modules:**
- Amulets
- Circlets
- Rings

**DLC Addons**
- Dawnguard Addon

**Amulet Textures**
- Gamwich Amulet Textures - 1024

**Ring Texture Options**
- Gamwich Ring Textures -Combined - 1k
- Optional Mesh Packs: Select Nothing
- Optional Mesh Packs Dawnguard: Select Nothing

#### [GIANT (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/6179)
Recommendation: 2K
#### [Gold Septim - Coins Retex](http://www.nexusmods.com/skyrimspecialedition/mods/1358)
Recommendation: 1K
#### [Greatsword Sheaths and Scabbards Redux SE](http://www.nexusmods.com/skyrimspecialedition/mods/325)
Install options:\
-Meshes Type: Meshes - Thin
- Sheath/Scabbard Type: Small - Default Textures
- Skyforge Weapons: Select Nothing

#### [HAGRAVEN](http://www.nexusmods.com/skyrimspecialedition/mods/7679)
Recommendation: 2K
#### [Hardy Hares](http://www.nexusmods.com/skyrimspecialedition/mods/27366)
#### [HD Dark brotherhood door](http://www.nexusmods.com/skyrim/mods/53059)
#### [HD Executioners Block SE](http://www.nexusmods.com/skyrimspecialedition/mods/22674)
#### [HD Misc](http://www.nexusmods.com/skyrim/mods/3595)
#### [HD Pondfish](http://www.nexusmods.com/skyrimspecialedition/mods/24731)
#### [HD Reworked Horses](http://www.nexusmods.com/skyrimspecialedition/mods/28249)
Recommendation: 2K-1K
#### [HD Road Signs](http://www.nexusmods.com/skyrimspecialedition/mods/2454)
Recommendation: 2K\
Install Main and both Optional files.
#### [HD Stone Quarry and Clay Deposit (SE)](http://www.nexusmods.com/skyrim/mods/38479)
Download and install the 1K Main File.\
Hide the following files:
- meshes\_byoh\clutter\resources\claypilem01.nif
- textures\_byoh\clutter\resources\claydeposit01_p.dds
- textures\_byoh\clutter\resources\StoneQuarry01.dds
- textures\_byoh\clutter\resources\StoneQuarry01_N.dds
- textures\_byoh\clutter\resources\StoneQuarry01_P.dds 

#### [High-Res Dartwing (Dragonfly) Texture](http://www.nexusmods.com/skyrim/mods/62809)
#### [High Quality Food and Ingredients SE](http://www.nexusmods.com/skyrimspecialedition/mods/10897)
Choose *custom* in the installer and choose the following:
- Baked Potatoes
- Boiled Creme Treat
- Bone Meal
- Bread
- Carrots
- Charred Skeever Hide and Meat
- Chicken Breast
- Dead Hare
- Dead Pheasant
- Garlic
- Green Apple
- Grilled Chicken Breast
- Grilled Leeks
- Honey Nut Treat
- Long Taffy Treat
- Mead
- Moon Sugar
- Mora Tapinella
- Pie
- Potatoes
- Powered Mannoth Tusk (it's misspelled)
- Raw Beef
- Red Apple
- Salmon Meat
- Salmon Steak
- Salt Pile
- Scaly Photiota
- Seared Slaughterfish
- Slaughterfish Scales
- Sweet Roll
- Venison
- Void Salts

#### [HORNCANDLES](http://www.nexusmods.com/skyrimspecialedition/mods/17285)
Recommendation: 2K-1K
#### [Hybrids HD Plants and Herbs Retexture (SE)](http://www.nexusmods.com/skyrim/mods/1546)
Hide the following files/folders:
- Textures\Plants\FloraNirnroot01.dds
- Textures\Plants\HangingMoss01.dds
- Textures\Plants\MountainFloweringPurple.dds
- Textures\Plants\MountainFloweringPurple_n.dds
- Textures\Plants\Snowberry01.dds
- Textures\Plants\SnowberrySnow01.dds
- Textures\Plants\TundraCotton01.dds 

#### [Iconic's Real Hay](http://www.nexusmods.com/skyrimspecialedition/mods/11133)
Recommendation: 2K alt
#### [Immersive Dragons](http://www.nexusmods.com/skyrimspecialedition/mods/18957)
#### [Immersive Smilodons](http://www.nexusmods.com/skyrimspecialedition/mods/18429)				
#### [Improved closefaced helmets (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/824)
#### [Improved Sparks](http://www.nexusmods.com/skyrimspecialedition/mods/19831)
Recommendation: Grindstones - 10X Sparks and Impact Effects - Vanilla Sparks
#### [Improved Weapon Impact EFFECTS Correct Metal SE](http://www.nexusmods.com/skyrimspecialedition/mods/8936)
#### [Inferno - Fire Effects Redux](http://www.nexusmods.com/skyrimspecialedition/mods/29316)
Recommended install options:\
- Main Installation: Core Files
- Resolution Options: Lite
- Glow Options: Normal
- Inferno Flame Color: Freeseia
- Tile Options: New
- Patch Options: Ember HD
- Patch Options: Select Nothing
- Patch Options: Select Nothing

#### [Just Ice (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/9444)
Recommendation: 2K
#### [LeanWolf's Improved Enchanter Candle Meshes SE](http://www.nexusmods.com/skyrimspecialedition/mods/7883)
#### [MAMMOTH](http://www.nexusmods.com/skyrimspecialedition/mods/6127)
Recommendation: 2K
#### [Metallurgy - Ingots and Ore HD](http://www.nexusmods.com/skyrimspecialedition/mods/30738)
Recommendation: Metallurgy - Ingots and Ore HD 1K (LOOSE)
#### [MM - REAL ELKS](http://www.nexusmods.com/skyrim/mods/94362)
Recommendation: 2K
#### [New Thinner Torch](http://www.nexusmods.com/skyrim/mods/6950)
Download and install the Ultimate HD Torch by rheadude compatible file. 
#### [Not Really HD Display Case](http://www.nexusmods.com/skyrim/mods/3693)
#### [Not Really HD Keys](http://www.nexusmods.com/skyrim/mods/2875)
#### [Rally's Hooks and Saws](http://www.nexusmods.com/skyrimspecialedition/mods/32652)
#### [Rally's Instruments HQ](http://www.nexusmods.com/skyrimspecialedition/mods/28193)
Recommendation: Rallys Instruments HQ - Version 2 Vanilla Lute
#### [Real Wood Textures - Farmhouses (SE)](http://www.nexusmods.com/skyrim/mods/50595)
Download and Install the Real Wood Textures - Farmhouses No Green Moss Version Optional File.\
\
Hide the following files/folders:
- textures\architecture\farmhouse\StoneWall01.dds
- textures\architecture\farmhouse\StoneWall01_n.dds
- textures\architecture\farmhouse\WovenFence01.dds
- textures\architecture\farmhouse\WovenFence01_n.dds 

#### [Realistic HD Baskets Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/22199)
#### [Realistic HD Pickaxe Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/20168)
#### [Realistic HD Woodcutter's Axe Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/20239)
#### [Realistic Water Two (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2182)
Choose no optional textures. Choose extended ambiance and patches for *Landscape Fixes for Grass Mods*,  *Falskaar* and *Wyrmstooth*.

#### [Rens HD Shrines (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/13572)
ChooseThe shrines that you think look the best, for example:\
- Akatosh: Sands of Time
- Arkay: Golden Shells
- Dibella: Springs of Love
- Julianos: Magic Circles
- Kynareth: Heavenly Air
- Mara: Gilded Saint
- Stendarr: Tusk of Mercy
- Talos: Rusted Steel
- Zenithar: Golden Circuit

#### [Retexture for Bread - Hearthfire](http://www.nexusmods.com/skyrim/mods/64980)
#### [Retexture for Soup](http://www.nexusmods.com/skyrim/mods/65238)
Install SMIM Mesh - Poor Version
#### [Ruins Clutter Improved](http://www.nexusmods.com/skyrimspecialedition/mods/5870)
Choose *Install Everything* in the installer. Hide or delete the following files or folders:
- meshes\furniture\workbenches
- meshes\furniture\enchantingworkbench.nif
- meshes\furniture\enchantingworkstation.nif
- meshes\loadscreenart\loadscreenenchantingworkbench.nif
- textures\clutter\candles 
#### [RUSTIC ANIMATED POTIONS and POISONS](http://www.nexusmods.com/skyrimspecialedition/mods/2276)
Recommendation: 1K
#### [RUSTIC ARMOR and WEAPONS SE](http://www.nexusmods.com/skyrimspecialedition/mods/19666)
Recommendation: 2K
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
Recommendation: 1K
#### [RUSTIC SPRIGGAN - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18107)
Recommendation: 2K
#### [RUSTIC WINDOWS - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/1937)
Recommendation: 2K
#### [SABRECAT](http://www.nexusmods.com/skyrimspecialedition/mods/5303)
Recommendation: 2K\
Install both options in the installer.
#### [SKELETON](http://www.nexusmods.com/skyrimspecialedition/mods/17282)
Recommendation: 2K\
Install selecting the Skin, clutter without sounds option. 
#### [Skygazer Moons SSE](http://www.nexusmods.com/skyrimspecialedition/mods/32057)
The *Glow* version (1.2) has some issues which should be fixed with later versions. For now, use the *No Glow* version
#### [Skyrim Redesigned WIP (SE)](http://www.nexusmods.com/skyrim/mods/8954)
Download and install the FOMOD Version and install using the STEP option. 
#### [Skyrim SE Improved Puddles](http://www.nexusmods.com/skyrimspecialedition/mods/1462)
Choose *2048x2048 Resolution* and *Skyrim Special Edition (all DLCs)* in the installer
#### [Skyrim SE Skill Interface Re-Texture](http://www.nexusmods.com/skyrimspecialedition/mods/1523)
Choose the options you prefer
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
Recommendation: 2K-1K\
Choose *Full version - skin with a linen fabric cloth* in the installer.

### Audiovisual - Trees & Vegetation
#### [HQ Tree Bark](http://www.nexusmods.com/skyrimspecialedition/mods/6556)
Choose the options you prefer. Install the Simply Bigger Trees patch.
#### [Landscape Fixes For Grass Mods](http://www.nexusmods.com/skyrimspecialedition/mods/9005)
#### [No More Hanging Moss](https://www.nexusmods.com/skyrimspecialedition/mods/16426)
Install _Hanging moss removal - partial - the moss around trees -_ mesh edits only. Without this mod you would get floating moss hanging from resized trees.
#### [Realistic Aspen Trees SE](http://www.nexusmods.com/skyrimspecialedition/mods/4423)
Choose 2k or 4k. Choose LodGen billboards (doesn't really matter, they will be overwritten by the next mod)
#### [Simply Bigger Trees SE](http://www.nexusmods.com/skyrimspecialedition/mods/5281)
Install the Realistic Aspen trees version of this mod.

## Audiovisual - Sounds & Music
#### [Audio Overhaul for Skyrim SE](http://www.nexusmods.com/skyrimspecialedition/mods/12466)
Do not install any patches. Delete the SKSE folder after installation.
#### [Better Animal Footsteps](https://www.nexusmods.com/skyrim/mods/24805)
Choose to install all footstep sounds. Do not install any patches.
#### [Better Horse Pain Sounds](http://www.nexusmods.com/skyrim/mods/12608)
#### [Heart of the Beast - Werewolf Sound and Texture Overhaul](http://www.nexusmods.com/skyrim/mods/13779)
Recommendation: *Feral Werewolf sounds - HIGH AGGRESSION*
#### [IHSS - Improved Horse Step Sounds](http://www.nexusmods.com/skyrimspecialedition/mods/848)
#### [Lower Sounding Thieves Guild Door](http://www.nexusmods.com/skyrim/mods/1826)
#### [Realistic wolf howls](http://www.nexusmods.com/skyrim/mods/30636)
Recommendation: *Realistic Wolf Howls more barks than howls*
#### [Sound Hammering Sounds](http://www.nexusmods.com/skyrimspecialedition/mods/5592)
#### [Thundering Shouts (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/14352)	
#### [Ultra Realistic Bow Shoot Sounds](https://www.nexusmods.com/skyrim/mods/27208)
#### [Ultra Realistic Crossbow Shoot Sounds](https://www.nexusmods.com/skyrim/mods/31274)



## Character Appearance
### Character Appearance - Female body
*This section replaces the vanilla female body with the CBBE body. The CBBE body is chosen because of its versatility. Recommended presets makes the body look realistic or vanilla-ish. Using a body replacer is the only way to make sure the female body is compatible both with skin texture replacers and with mods that add new armors to the game.*\
#### [Caliente’s Beautiful Bodies Enhancer -CBBE-](https://www.nexusmods.com/skyrimspecialedition/mods/198)
*NSFW warning*\
Install the main file, the update file and the optional file ‘CBBE ESL-flagged .esp’.
In the main installer, choose:
- Body Shape: Slim
- Underwear options: NeverNude
- Outfit options: Vanilla outfits
- SKEE (RaceMenu): RaceMenu Morphs
#### [BodySlide and Outfit Studio](https://www.nexusmods.com/skyrimspecialedition/mods/201)
Check the nexus page for the instructions to add this mod as an executable in Mod Organizer (in short, install as a normal mod and right click the executable in MO:s data tab. Choose add as executable).
#### [CBBE Presets Compendium](https://www.nexusmods.com/skyrimspecialedition/mods/11229)
*NSFW warning*\
Install the main file

### Character Appearance - Face Parts, textures and overhauls
#### [Beards](http://www.nexusmods.com/skyrimspecialedition/mods/1067)
Choose *Full Install* and *Low: 1024*
#### [Brows](http://www.nexusmods.com/skyrimspecialedition/mods/1062)
Choose *Full Install* and *Low: 512*
#### [Consistent Older People](http://www.nexusmods.com/skyrimspecialedition/mods/2977)
Install the loose version
#### [Coverkhajiits (SE)](http://www.nexusmods.com/skyrim/mods/5941)
Install both main files
#### [FAR - Forgotten Argonian Roots (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/1704)
The mod is not packaged correctly for mod managers. To install:

1. Open the archive in MO for installation.
2. Expand FAR-Forgotten Argonian Roots
3. Expand Females → CBBE Body → MAIN texture
4. Drag and drop the Textures folder onto < data > above
5. Expand Males → Better Males body
6. Drag and drop the Textures folder onto < data > above
7. Expand no glow skin → Female
8. Drag and drop the Textures folder onto '< data > above
9. Expand no glow skin → Male
10. Drag and drop the Textures folder onto < data > above
11. Untick FAR-Forgotten Argonian Roots and click OK

#### [Female Vampires Have Fangs](http://www.nexusmods.com/skyrimspecialedition/mods/1211)
#### [Immersive Spectral Assassin](http://www.nexusmods.com/skyrimspecialedition/mods/27051)	
Download and install the Immersive Spectral Assassin (Oblivion) file.

Some of this mod's features have been reverted in this builds patch in order to return it to a more vanilla-like replacement. The following was changed:

- The perks have been removed
    - The perks were added by the author and weren't present in vanilla so this was reverted. 
- Magic has been increased
    - Upon looking up the lore and Oblivion NPC, it was found that Lucien's magic was much higher than Skyrim has it. Therefore, it's been increased. 
- Nightingale gloves removed
    - In an effort to return the NPC back to as much a vanilla-like state as possible, he Nightingale gloves (too powerful) were switched out with the Jester gloves (more equivalent to vanilla). 

#### [KS Hairdos SSE](http://www.nexusmods.com/skyrimspecialedition/mods/6817)
#### [Maevan2’s Mature Skin Texture for CBBE – UNP](https://www.nexusmods.com/skyrimspecialedition/mods/26017)
*NSFW warning*\
In the installer, choose what you want, for example: high, CBBE slim, medium, lips, complexions, young, mature.
#### [RUSTIC CHILDREN (SE)](http://www.nexusmods.com/skyrim/mods/63353)
Recommendation: 2K
#### [Salt and Wind – Rough Hair for KS Hairdos SE](http://www.nexusmods.com/skyrimspecialedition/mods/16582)
#### [Superior Lore-Friendly Hair (SE)](http://www.nexusmods.com/skyrim/mods/36510)
Recommendation: Rough hair, 1K
#### [TDN Equipable Horns SE](http://www.nexusmods.com/skyrimspecialedition/mods/9224)
Yes, some Bosmer have antlers.\
*"It is also common among the Bosmer to wear decorative antlers on their foreheads, although rarely, individuals with real, magically-grown antlers can also be encountered."* [source](https://en.uesp.net/wiki/Lore:Bosmer) \
Skip this mod if you do not intend to use horns or antlers for your character.
#### [Tempered Skins for Males](http://www.nexusmods.com/skyrimspecialedition/mods/7902)
In the installer you can choose what you like but the following is recommended: A1, B6, C1, D2, E2, no facemarks or scars.\
\
Hide the following files:
- textures\actors\character\argonianmale (entire folder)
- textures\actors\character\khajiitmale\khajiitmalehead_s.dds
- textures\actors\character\male\maleunderwear.dds
- textures\actors\character\male\maleunderwear_n.dds
- textures\armor\briarheart\briarheart.dds
- textures\armor\briarheart\briarheart_n.dds

#### [Vanilla Makeup HD](http://www.nexusmods.com/skyrimspecialedition/mods/24482)
Recommendation: 2K for all races and update file.
#### [MHD - All Races - 2K Also install the 2K update file](http://www.nexusmods.com/skyrimspecialedition/mods/20751)
Recommendation: 2K.\
In the installer, choose the following:
**Main Files**
- Vanilla Replacers: 2K vanilla Replacers
- 2K RaceMenu All-In-One

**Variant Textures**
- Vanilla Variants General Watercolor: None
- Vanilla Variants Wood Elves Muddy: None
- Vanilla Variants Dark Elf Ashy: None
- Vanilla Variants Khajiit Stripes Furry: 2K Furry
- Vanilla Variants Nord Splattered: None
- Vanilla Variants Argonian Scaley: 2K Scaley
- RaceMenu Variants General Watercolor: None
- RaceMenu Variants Wood Elves Muddy: None
- RaceMenu Variants Dark Elf Ashy: None
- RaceMenu Variants Khajiit Stripes Furry: 2K Furry
- RaceMenu Variants Nord Splattered: None
- RaceMenu Variants Argonian Scaley: 2K Scaley

**SKSE Tintmask Configs**
- None

## Fixes
#### [(SKSE64) Havok Fix](http://www.nexusmods.com/skyrimspecialedition/mods/18160)
#### [1st Person Candlelight Fix](http://www.nexusmods.com/skyrimspecialedition/mods/9736)
#### [Bug Fixes SSE](http://www.nexusmods.com/skyrimspecialedition/mods/33261)
#### [Butterflies Land True](http://www.nexusmods.com/skyrimspecialedition/mods/29434)
#### [Butterflies Unchained](http://www.nexusmods.com/skyrimspecialedition/mods/29538)
Install esl version
#### [Critters Ain't Snitches - Animal and Monster Crime Reporting Fix - BETA](http://www.nexusmods.com/skyrimspecialedition/mods/15134)
#### [Dragon Stalking Fix](http://www.nexusmods.com/skyrimspecialedition/mods/14060)
#### [Enchantment Reload Fix SE](http://www.nexusmods.com/skyrimspecialedition/mods/21055)
#### [Eye Normal Map Fix SSE](http://www.nexusmods.com/skyrimspecialedition/mods/5445)
Install *Eye Normal Map Fix SSE BC7*
#### [Fuz Ro D-oh - Silent Voice](http://www.nexusmods.com/skyrimspecialedition/mods/15109)
Install main and optional files.
#### [Hearthfires Houses Building Fix](http://www.nexusmods.com/skyrimspecialedition/mods/27298)
#### [Invisibility and Eyes Mesh Fix by HHaleyy](http://www.nexusmods.com/skyrimspecialedition/mods/14464)
Choose *Eyes Mesh Fix* in the installer.
#### [Modern Brawl Bug Fix](http://www.nexusmods.com/skyrimspecialedition/mods/1473)
#### [Reasonable Movement Speed](http://www.nexusmods.com/skyrimspecialedition/mods/3422)
#### [Skyrim Landscape and Water Fixes](http://www.nexusmods.com/skyrimspecialedition/mods/26138)
In the installer, choose:
- Base Fixed Meshes: Base Meshes
- Main Plugin: 1. ESM
- Patches: Relighting Skyrim
- Walkway Wall FIX: Walkway Wall FIX SMIM

#### [Skyrim Project Optimization SE](http://www.nexusmods.com/skyrimspecialedition/mods/14084)
Choose ESM version
#### [SkyUI SE - Flashing Savegames Fix](http://www.nexusmods.com/skyrimspecialedition/mods/20406)
#### [SSE Engine Fixes (skse64 plugin)](http://www.nexusmods.com/skyrimspecialedition/mods/17230)
1. Download and install the (Part 1) Engine Fixes 4.11 for SSE 1.5.97 - skse64 plugin Main File.= in MO.
2. Download the (Part 2) Engine Fixes - skse64 Preloader and TBB Lib Main File.
3. Extract the contents of the second archive to the root Skyrim SE directory (i.e. ..\Steam\SteamApps\Common\Skyrim Special Edition\) 
Once installed open and ensure the EngineFixes.ini file is configured:
```
[Patches]
EnableAchievementsWithMods = true

FormCaching = true

MaxStdio = true

TreeLODReferenceCaching = true

WaterflowAnimation = true

WaterflowSpeed = 16.0
20.0 = default. Smaller = slower, larger = faster.

[Fixes]
ArcheryDownwardAiming = true

AnimationLoadSignedCrash = true

DoublePerkApply = true

LipSync = true

MemoryAccessErrors = true

MO5STypo = true

SlowTimeCameraMovement = true

TreeReflections = true

VerticalLookSensitivity = true
```
>Leave the remainder of the settings at their defaults, unless the changes are known and desired.
#### [Stay At The System Page - Updated](http://www.nexusmods.com/skyrimspecialedition/mods/19832)
#### [Unlimited Bookshelves (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2885)
#### [Waterbreathing Breathless Emerge SSE](http://www.nexusmods.com/skyrimspecialedition/mods/14485)
#### [Wiseman303's Critter Fixes (SE)](http://www.nexusmods.com/skyrim/mods/54485)
In the installer, choose *Monarch Wing Fix*.
#### [Wiseman303's Flora Fixes](https://www.nexusmods.com/skyrimspecialedition/mods/28197)
Install the main file and the patch for SMIM.

## Gameplay
### Gameplay - General
#### [GIST - Genuinely Intelligent Soul Trap SE](http://www.nexusmods.com/skyrimspecialedition/mods/15755)
Download and install the Main File and the GIST - Rustic Soul Gems patch Optional File. 

### Gameplay - AI & Combat
#### [Auto Hide Ammo](http://www.nexusmods.com/skyrimspecialedition/mods/1882)
Install the Simple Auto Unequip Ammo from the Old Files.
#### [Better Stealth AI for Followers](http://www.nexusmods.com/skyrimspecialedition/mods/17600)
#### [Follower Trap Safety](http://www.nexusmods.com/skyrimspecialedition/mods/2755)
#### [Immersive Citizens - AI Overhaul SE](http://www.nexusmods.com/skyrimspecialedition/mods/173)
Do not choose any patches in the main installer.
#### [Realistic AI Detection SE](http://www.nexusmods.com/skyrimspecialedition/mods/2345)
Choose *Realistic AI Detection 2 SE - Medium Interior Medium Exterior*
#### [Run For Your Lives (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2272)
#### [Tavern AI fix](http://www.nexusmods.com/skyrimspecialedition/mods/23107)
#### [TK Dodge SE](https://www.nexusmods.com/skyrimspecialedition/mods/15309)
#### [Ultimate Combat SE](http://www.nexusmods.com/skyrimspecialedition/mods/17196)

### Gameplay - Classes & Races
#### [Aetherius - A Race Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/26686)
#### [Class Overhaul Re-Imagined (SkyRem - Cori)](https://www.nexusmods.com/skyrimspecialedition/mods/24808)
#### [Experience](http://www.nexusmods.com/skyrimspecialedition/mods/17751)
Do not activate this mod yet. Wait until you have left the first cell of Alternate Start to avoid getting experience when different mods do their initial setup routines.
#### [Growl - Werebeasts of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/31245)
#### [Sacrosanct - Vampires of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/3928)

### Gameplay - Crafting
#### [Ars Metallica - Smithing Enhancement](https://www.nexusmods.com/skyrimspecialedition/mods/321)

### Gameplay - Economy & Item Balance
#### [Trade and Barter](http://www.nexusmods.com/skyrimspecialedition/mods/23081)
#### [Weapons Armor Clothing and Clutter Fixes](http://www.nexusmods.com/skyrimspecialedition/mods/18994)
Recommendation: 2K textures.
After installation, hide or delete the file *WACCF_BashedPatchLvlListFix.esp*

### Gameplay - Immersion & Role-playing
#### [Campfire - Complete Camping System](http://www.nexusmods.com/skyrimspecialedition/mods/667)
Hide or delete the file *SKSE/Plugins/PapyrusUtil.dll*. It is outdated and we need to use the newer one from PapyrusUtil SE.
#### [Campfire and Frostfall - Unofficial SSE Update](http://www.nexusmods.com/skyrimspecialedition/mods/17925)
#### [Carriage and Ferry Travel Overhaul](http://www.nexusmods.com/skyrimspecialedition/mods/8379)
Install patches for *Immersive Citizens - AI Overhaul* and *Dawnstar*.
#### [Convenient Horses (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/9519)
#### [Daedric Voices](https://www.nexusmods.com/skyrimspecialedition/mods/32090)
Install the main file and the Growl patch.
#### [Disease Descriptions for the Immersive Adventurer SE](http://www.nexusmods.com/skyrimspecialedition/mods/26992)
#### [ElSopa - Campfire HD SE](http://www.nexusmods.com/skyrimspecialedition/mods/24511)
#### [Get Snowy (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/22488)
When installing the mod, untick the following plugins:
- getSnowy_ObsidianWeathers_Patch.esp
- getSnowy_WnC-Ashes Patch.esp

#### [Go On Ahead](http://www.nexusmods.com/skyrimspecialedition/mods/4779)
#### [Guard Dialogue Overhaul SE](http://www.nexusmods.com/skyrimspecialedition/mods/22075)
#### [Improved Traps](http://www.nexusmods.com/skyrimspecialedition/mods/17592)
Install *Improved Traps and Mining Makes Noise*
#### [Lenient Survival](https://www.nexusmods.com/skyrimspecialedition/mods/13087)
For users of Survival Mode only. Do not install the optional file. A plugin to remove carry weight penalty is found in the guides patches.
#### [Lock Related Loot](http://www.nexusmods.com/skyrimspecialedition/mods/11342)
#### [Nether's Follower Framework](http://www.nexusmods.com/skyrimspecialedition/mods/18076)
Choose the following: 
- Followers avoid traps
- Interesting NPC support
- Relationship Dialogue Overhaul
- RDO Comments
#### [No Lockpick Activate (SKSE) - Updated](http://www.nexusmods.com/skyrimspecialedition/mods/26790)
#### [Point The Way (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/352)
#### [Ragdoll Paralysis Redux SE](https://www.nexusmods.com/skyrimspecialedition/mods/13575)
#### [Relationship Dialogue Overhaul - RDO SE](http://www.nexusmods.com/skyrimspecialedition/mods/1187)
#### [Simple Drop Lit Torches SE](http://www.nexusmods.com/skyrimspecialedition/mods/14490)
#### [Torches Ignite Oil](http://www.nexusmods.com/skyrimspecialedition/mods/13226)

### Gameplay - Magic & Abilities
#### [Mundus - A Standing Stone Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33411)
#### [Mysticism - A Magic Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/27839)
Install the main file and the Survival patch. Do not install the Audio Overhaul Skyrim patch.
#### [Thunderchild - Epic Shouts and Immersion](http://www.nexusmods.com/skyrimspecialedition/mods/1460)

### Gameplay - Quests & Stories
#### [Alternate Start - Live Another Life - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/272)	
#### [The Brotherhood of Old - Open Beta - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/15322)
#### [The Choice is Yours (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/3850)
#### [Clockwork (SSE)](http://www.nexusmods.com/skyrimspecialedition/mods/4155)
#### [Dawnguard and Clan Volkihar Epilogues](http://www.nexusmods.com/skyrimspecialedition/mods/12098)
#### [Even Better Quest Objectives](http://www.nexusmods.com/skyrimspecialedition/mods/159)
In the installer, choose the optional file *Dark Brotherhood Forever to Miscellaneous Quests* and patches for *Alternate Start, Book Covers Skyrim, Cutting room floor* and *The Paarthurnax Dilemma*.
#### [The Forgotten City](http://www.nexusmods.com/skyrimspecialedition/mods/1179)
#### [Gildergreen Regrown](http://www.nexusmods.com/skyrimspecialedition/mods/348)
#### [The Gray Cowl of Nocturnal SE](http://www.nexusmods.com/skyrimspecialedition/mods/4509)
#### [The Gray Cowl of Nocturnal SSE - HD pack](http://www.nexusmods.com/skyrimspecialedition/mods/7644)
#### [Gray Cowl of Nocturnal Alikr Flora Overhaul SE](http://www.nexusmods.com/skyrimspecialedition/mods/10141)
#### [The Gray Cowl of Nocturnal SE - Addons and Patches](http://www.nexusmods.com/skyrimspecialedition/mods/19724)
Install the WACCF patch. The USSEP-patch isn't needed if you use SMIM, CFTO or Realistic Water 2.
#### [Helgen Reborn](http://www.nexusmods.com/skyrimspecialedition/mods/5673)
#### [Moon and Star](http://www.nexusmods.com/skyrimspecialedition/mods/4301)
#### [Moonpath to Elsweyr SSE](http://www.nexusmods.com/skyrimspecialedition/mods/4341)
#### [Not So Fast - Mage Guild (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/5686)
#### [Not So Fast - Main Quest (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2475)
#### [The Paarthurnax Dilemma](http://www.nexusmods.com/skyrimspecialedition/mods/365)
#### [Timing is Everything SE](http://www.nexusmods.com/skyrimspecialedition/mods/25464)
Install the FISS version.

### Gameplay - Skills & Perks
#### [Adamant - A Perk Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/30191)
#### [Lock Overhaul (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/14927)

### Gameplay - User Interface
#### [Better Container Controls for SkyUI](http://www.nexusmods.com/skyrimspecialedition/mods/25271)
Do not install the main file, install the esl optional file only. If you play with a gamepad, skip this mod completely.
#### [Better Dialogue Controls](http://www.nexusmods.com/skyrimspecialedition/mods/1429)
#### [Better MessageBox Controls](http://www.nexusmods.com/skyrimspecialedition/mods/1428)
#### [Cathedral Weathers MCM](http://www.nexusmods.com/skyrimspecialedition/mods/24940)
#### [Font Overhaul - Natural Typefaces for Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/2880)
#### [Immersive HUD - iHUD Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/12440)
#### [Lore-Based Loading Screens (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/1185)
#### [MoreHUD Inventory Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18619)
#### [MoreHUD SE](http://www.nexusmods.com/skyrimspecialedition/mods/12688)
#### [RaceMenu](http://www.nexusmods.com/skyrimspecialedition/mods/19080)
#### [UIExtensions](https://www.nexusmods.com/skyrimspecialedition/mods/17561)
#### [Smaller Vanilla Cursors SE](http://www.nexusmods.com/skyrimspecialedition/mods/20617)
#### [Viewable Faction Ranks](http://www.nexusmods.com/skyrimspecialedition/mods/17924)
#### [Whose Quest Is It Anyway](http://www.nexusmods.com/skyrimspecialedition/mods/23581)
#### [Yes Im Sure](http://www.nexusmods.com/skyrimspecialedition/mods/24898)

## Items
### Items – Armor, Clothing, & Accessories
*Remember to use both *Cloaks of Skyrim* and *Winter is coming* if you want new cloaks in the game.
#### [Bandolier - Bags and Pouches Classic](http://www.nexusmods.com/skyrimspecialedition/mods/2417)
#### [Cloaks of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/6369)
Install the main version
#### [Cloaks of Skyrim Ultra HD SSE](http://www.nexusmods.com/skyrimspecialedition/mods/29258)
#### [Immersive Armors](http://www.nexusmods.com/skyrimspecialedition/mods/3479)
#### [Immersive Armours - SSE CBBE BodySlide](https://www.nexusmods.com/skyrimspecialedition/mods/22382)
Install if you use Immersive Armors with CBBE.
#### [Winter Is Coming SSE - Cloaks](http://www.nexusmods.com/skyrimspecialedition/mods/4933)
Install the patch for Cloaks of Skyrim only if you are not using Complete Crafting Overhaul Remade.

### Items – Weapons
#### [Faction Crossbows SE](http://www.nexusmods.com/skyrimspecialedition/mods/4047)
#### [Heavy Armory - New Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/6308)
#### [Immersive Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/16788)
#### [Royal Armory - New Artifacts](http://www.nexusmods.com/skyrimspecialedition/mods/6994)
#### [Ruin's Edge](http://www.nexusmods.com/skyrimspecialedition/mods/12792)
#### [The Staff Of Sheogorath](http://www.nexusmods.com/skyrimspecialedition/mods/14468)
#### [Unique Uniques SE](https://www.nexusmods.com/skyrimspecialedition/mods/3334)
Install main file

## Locations
### Locations - New Structures & Landmarks
#### [Bells of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/10495)
Install the patch for Immersive Citizens - AI overhaul.
#### [Cutting Room Floor](http://www.nexusmods.com/skyrimspecialedition/mods/276)
#### [Solitude Skyway](http://www.nexusmods.com/skyrimspecialedition/mods/8250)
#### [Windhelm Lighthouse](http://www.nexusmods.com/skyrimspecialedition/mods/8453)

### Locations - New Lands
#### [Falskaar](http://www.nexusmods.com/skyrimspecialedition/mods/2057)
#### [Wyrmstooth SSE](https://archive.org/details/wyrmstooth1.18SSE)

### Locations - Towns and villages
#### [Darkwater Crossing](https://www.nexusmods.com/skyrimspecialedition/mods/326)
#### [Dragon Bridge](https://www.nexusmods.com/skyrimspecialedition/mods/8683)
#### [Dawnstar](https://www.nexusmods.com/skyrimspecialedition/mods/13607)
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

### Locations - Overhauls
#### [Bring Out Your Dead (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/323)
#### [Immersive College of Winterhold](http://www.nexusmods.com/skyrimspecialedition/mods/17004)
Choose 
- desaturated book covers
- RLS SSE Patch
- Better Dynamic Snow Patch
- Skyrim Project Optimization SSE Patch.
#### [Immersive Dawnguard Dayspring Pass SE](http://www.nexusmods.com/skyrimspecialedition/mods/4126)
#### [Smooth Shores](http://www.nexusmods.com/skyrimspecialedition/mods/10624)
#### [Farmhouse Chimneys SE](http://www.nexusmods.com/skyrimspecialedition/mods/8766)
The installer auto detects which mods you have installed and automatically chosses the correct patches. Do not install any *Alternative Toppers* unless you prefer them.

### Audiovisual - Lighting & Weather
#### [Cathedral Weathers and Seasons](http://www.nexusmods.com/skyrimspecialedition/mods/24791)
Install the main file.
#### [Lanterns Of Skyrim II](http://www.nexusmods.com/skyrimspecialedition/mods/30817)
In the installer, choose no addons. Install *the LoS II - SMIM patch*. The installer will automatically select all patches you need.
#### [Luminosity Lighting Overhaul - The Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/16830)
#### [Relighting Skyrim - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/8586)
#### [Storm Lightning for SSE](http://www.nexusmods.com/skyrimspecialedition/mods/29243)
In the installer, choose *Skyrim Special Edition* and the latest game version. Choose esl flagged plugin. Recommended settings for halo are as follows:
- Night time sheet halo: Halo with dimmer lighting (level 0)
- Day time sheet halo: Halo dim (level 2)
- Night time fork halo: Halo dimmer (level 1)
- Day time fork halo: Halo dim (level 2)

#### [Wonders of Weather (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/13044)
In the installer, choose core files and *Less Opaque Splashes*.

## New Characters
### New Characters - Enemies
#### [Arena - An Encounter Zone Overhaul](Arena - An Encounter Zone Overhaul)
#### [Deadly Dragons](http://www.nexusmods.com/skyrimspecialedition/mods/23723)
Choose Loremonger version with patches for Diverse Dragons, Splender Dragons and Wyrmstooth.
#### [Diverse Dragons Collection SE](http://www.nexusmods.com/skyrimspecialedition/mods/695)
#### [OBIS SE - Organized Bandits In Skyrim Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/4145)
Install main file and OBIS SE Patrols addon.
#### [Skyrim Revamped - Complete Enemy Overhaul](http://www.nexusmods.com/skyrimspecialedition/mods/14598)
#### [Splendor – Dragon Variants SE](http://www.nexusmods.com/skyrimspecialedition/mods/9670)

### New Characters - Neutral
#### [Immersive Patrols SE](http://www.nexusmods.com/skyrimspecialedition/mods/718)
#### [Immersive World Encounters SE](https://www.nexusmods.com/skyrimspecialedition/mods/18330)
#### [Interesting NPCs SE](https://www.nexusmods.com/skyrimspecialedition/mods/29194)
#### [Interesting NPCs (3DNPC) character Zora Fairchild's voice boosted](http://www.nexusmods.com/skyrimspecialedition/mods/16090)

### New Characters - Allies
#### [INIGO](http://www.nexusmods.com/skyrimspecialedition/mods/1461)

## STEP SE: Core Changes
*Some updates to STEP mods are required to make them compatible with other mods in this list*
#### [Farmhouse Chimneys](http://www.nexusmods.com/skyrimspecialedition/mods/8766)
Reinstall and choose all relevant patches.
#### [FAR - Forgotten Argonian Roots](http://www.nexusmods.com/skyrimspecialedition/mods/1704)
Reinstall using the STEP instructions but choose CBBE body instead of default for females.
#### [Lanterns Of Skyrim II](https://www.nexusmods.com/skyrimspecialedition/mods/30817)
Reinstall using STEP options and patches for Arthmoor's villages.
#### [Enhanced Lighting for ENB (ELE) - Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/1377)
Install the patches for Helgen Reborn and Falskaar. No other patches are needed. Uninstall if you use *Luminosity*.
#### [Kryptopyr's Patch Hub](http://www.nexusmods.com/skyrimspecialedition/mods/19518)
Move this mod to my patches section. Refer to that section for install options.
#### [Landscape fixes for grass mods](https://www.nexusmods.com/skyrimspecialedition/mods/9005)
Reinstall and add patches for Helgen Reborn, Moon and Star and all Arthmoor's villages.

## Utilities
#### [Fores New Idles in Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/3038)

## Patches
#### [Better Dynamic Majestic Mountains](http://www.nexusmods.com/skyrimspecialedition/mods/20102)
#### [Falskaar - Addons and Patches](http://www.nexusmods.com/skyrimspecialedition/mods/19454)
Choose 
- Bug Fixes
- Boat Location Patch
- Fast Travel Addon
- Unique Region Names Addon
#### [Immersive College of Winterhold - Not so fast Mage Guild Patch](https://www.nexusmods.com/skyrimspecialedition/mods/18731)
#### [Improved Closedfaced Helmets](https://www.nexusmods.com/skyrim/mods/15927)
Download Improved Closefaced Helmets Patch v1 and choose SkyRealism Shiny in the installer. Install this as a new mod, making sure to not overwrite or merge it with the main Closefaced Helmets mod.
#### [Kryptopyr's Patch Hub](http://www.nexusmods.com/skyrimspecialedition/mods/19518)
The fomod installer will identify which patches you need and select them automatically. Do not install the *WACCF - Survival Mode Patch*.
#### [Moonpath to Elsweyr Sky and Lightning fix](http://www.nexusmods.com/skyrimspecialedition/mods/18683)
#### [Unofficial Moonpath to Elsweyr Patch](http://www.nexusmods.com/skyrimspecialedition/mods/15882)
#### [Unofficial Skyrim Creation Club Content Patches](http://www.nexusmods.com/skyrimspecialedition/mods/18975)
Choose the Unofficial Skyrim Survival Patch.
#### [Weapons Armor Clothing and Clutter Fixes - CBBE Patch](https://www.nexusmods.com/skyrimspecialedition/mods/19176)
#### [Dread's modlist patches](https://github.com/dreadflopp/dreads_modlist_patches)
To download, click the button *Clone or download* and choose *download zip*.
The fomod installer will automatically select all mods you use. Select the tweaks you want to use.