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

## Resources
#### [.NET Script Framework](http://www.nexusmods.com/skyrimspecialedition/mods/21294)
#### [Address Library for SKSE Plugins](http://www.nexusmods.com/skyrimspecialedition/mods/32444)
#### [FileAccess Interface for Skyrim SE Scripts - FISSES](http://www.nexusmods.com/skyrimspecialedition/mods/13956)
#### [PapyrusUtil SE - Modders Scripting Utility Functions](http://www.nexusmods.com/skyrimspecialedition/mods/13048)
#### [Scaleform Translation++](http://www.nexusmods.com/skyrimspecialedition/mods/22603)
#### [Skyrim Skill Uncapper](http://www.nexusmods.com/skyrimspecialedition/mods/8889)
#### [SkyUI](http://www.nexusmods.com/skyrimspecialedition/mods/12604)

## Foundational Mods
#### [Unofficial High Definition Audio Project](http://www.nexusmods.com/skyrimspecialedition/mods/18115)
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
#### [Landscapes - Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/21954)
In the installer, choose:
- Full Install, Brown Tundra
- Blended Roads
#### [Weapons Armor and Clothing - Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/20199)
Choose CBBE in the installer if you use CBBE.
Hide or delete the file _CalienteTools\BodySlide\ShapeData\CBBE Vanilla\Body\Ebony.nif_ since this mesh is causing issues.
#### [RUSTIC CLOTHING - Special Edition](https://www.nexusmods.com/skyrimspecialedition/mods/4703)
#### [Unofficial Material Fix](http://www.nexusmods.com/skyrimspecialedition/mods/21027)

## Audiovisual
### Audiovisual - Animations & Effects
#### [XP32 Maximum Skeleton Special Extended - XPMSSE](http://www.nexusmods.com/skyrimspecialedition/mods/1988)

### Audiovisual - Lighting & Weather 
#### [Luminosity Lighting Overhaul - The Cathedral Concept](https://www.nexusmods.com/skyrimspecialedition/mods/16830)

### Audiovisual - Models & Textures
#### [Barenziah's Glory SE](http://www.nexusmods.com/skyrimspecialedition/mods/6343)
#### [Bellyaches Animal and Creature Pack SSE](http://www.nexusmods.com/skyrimspecialedition/mods/6839)
#### [Bellyaches HD Dragon Replacer Pack (SE)](http://www.nexusmods.com/skyrimspecialedition/mods/2636)
#### [BetterFalmerCaveCeilingGlow](http://www.nexusmods.com/skyrimspecialedition/mods/17232)
#### [CleverCharff's Photorealistic Ash Pile](http://www.nexusmods.com/skyrimspecialedition/mods/32720)
#### [Deathbell HD](http://www.nexusmods.com/skyrimspecialedition/mods/10755)
#### [Detailing the Eldrich - Higher-Res Riekling Architecture](http://www.nexusmods.com/skyrim/mods/46741)
#### [Dragon Glyphs HD - Fixed](http://www.nexusmods.com/skyrim/mods/27095)
#### [Dragon Masks Retextured SE (4K - 2K)](http://www.nexusmods.com/skyrimspecialedition/mods/22699)
#### [DRAGON PRIEST](http://www.nexusmods.com/skyrimspecialedition/mods/4974)
#### [Dragonbone Mastery - Weapons Retexture](http://www.nexusmods.com/skyrimspecialedition/mods/2056)
#### [DRAUGR](http://www.nexusmods.com/skyrimspecialedition/mods/5848)
#### [DROPS](http://www.nexusmods.com/skyrim/mods/63991)
#### [Dust Effects by HHaleyy](http://www.nexusmods.com/skyrimspecialedition/mods/2407)
#### [ElSopa HD - Ants SE](http://www.nexusmods.com/skyrimspecialedition/mods/26715)
#### [ElSopa HD - Dirt Blast SE](http://www.nexusmods.com/skyrimspecialedition/mods/22342)
#### [Embers HD](http://www.nexusmods.com/skyrimspecialedition/mods/14368)
#### [Enhanced Blood Textures SE](http://www.nexusmods.com/skyrimspecialedition/mods/2357)
#### [FALMER](http://www.nexusmods.com/skyrimspecialedition/mods/17224)
#### [Frankly HD Dawnguard Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/19663)
Install the CBBE patch.
#### [Frankly HD Dragonbone and Dragonscale - Armor and Weapons HQ](https://www.nexusmods.com/skyrimspecialedition/mods/25110)
Install both main and update file. 
#### [Frankly HD Imperial Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/20848)
Install the *Pants and Sleeves* patch and the *Better-Shaped Weapons* patch.
#### [Frankly HD Masque of Clavicus Vile](https://www.nexusmods.com/skyrimspecialedition/mods/28565)
#### [Frankly HD Miraak](https://www.nexusmods.com/skyrimspecialedition/mods/19699)
Install the CBBE patch.
#### [Frankly HD Nightingale Armor and Weapons](https://www.nexusmods.com/skyrimspecialedition/mods/18560)
Install the CBBE patch and the Better-Shaped Weapons patch.
#### [Frankly HD Shrouded Armor](https://www.nexusmods.com/skyrimspecialedition/mods/18785)
#### [Frankly HD Thieves Guild Armors HQ](https://www.nexusmods.com/skyrimspecialedition/mods/19953)
#### [GIANT](http://www.nexusmods.com/skyrimspecialedition/mods/6179)
#### [Gold Septim - Coins Retex](http://www.nexusmods.com/skyrimspecialedition/mods/1358)
#### [HAGRAVEN](http://www.nexusmods.com/skyrimspecialedition/mods/7679)
#### [HD Dark brotherhood door](http://www.nexusmods.com/skyrim/mods/53059)
#### [HD Executioners Block SE](http://www.nexusmods.com/skyrimspecialedition/mods/22674)
#### [HD Misc](http://www.nexusmods.com/skyrim/mods/3595)
#### [HD Pondfish](http://www.nexusmods.com/skyrimspecialedition/mods/24731)
#### [High-Res Dartwing (Dragonfly) Texture](http://www.nexusmods.com/skyrim/mods/62809)
#### [High Quality Food and Ingredients SE](http://www.nexusmods.com/skyrimspecialedition/mods/10897)
#### [HORNCANDLES](http://www.nexusmods.com/skyrimspecialedition/mods/17285)
#### [Improved Sparks](http://www.nexusmods.com/skyrimspecialedition/mods/19831)
#### [Improved Weapon Impact EFFECTS Correct Metal SE](http://www.nexusmods.com/skyrimspecialedition/mods/8936)
#### [MAMMOTH](http://www.nexusmods.com/skyrimspecialedition/mods/6127)
#### [New Thinner Torch](http://www.nexusmods.com/skyrim/mods/6950)
#### [Not Really HD Display Case](http://www.nexusmods.com/skyrim/mods/3693)
#### [Not Really HD Keys](http://www.nexusmods.com/skyrim/mods/2875)
#### [Rally's Hooks and Saws](http://www.nexusmods.com/skyrimspecialedition/mods/32652)
#### [Rally's Instruments HQ](http://www.nexusmods.com/skyrimspecialedition/mods/28193)
#### [Realistic HD Pickaxe Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/20168)
#### [Realistic HD Woodcutter's Axe Remastered](http://www.nexusmods.com/skyrimspecialedition/mods/20239)
#### [Retexture for Bread - Hearthfire](http://www.nexusmods.com/skyrim/mods/64980)
#### [Retexture for Soup](http://www.nexusmods.com/skyrim/mods/65238)
#### [Ruins Clutter Improved](http://www.nexusmods.com/skyrimspecialedition/mods/5870)
#### [RUSTIC ANIMATED POTIONS and POISONS](http://www.nexusmods.com/skyrimspecialedition/mods/2276)
#### [RUSTIC ARMOR and WEAPONS SE](http://www.nexusmods.com/skyrimspecialedition/mods/19666)
#### [RUSTIC AZURA'S STAR - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18345)
#### [RUSTIC COOKING - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/6142)
#### [RUSTIC DAEDRA - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/19272)
#### [RUSTIC DEATH HOUND and GARGOYLE - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/17740)
#### [RUSTIC DRAGON CORPSE - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/17639)
#### [RUSTIC ELDERSCROLL - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/17757)
#### [RUSTIC FROSTBITE SPIDER - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18817)
#### [RUSTIC NORDIC MURALS](http://www.nexusmods.com/skyrim/mods/65602)
#### [RUSTIC SPRIGGAN - Special Edition](http://www.nexusmods.com/skyrimspecialedition/mods/18107)
#### [SABRECAT](http://www.nexusmods.com/skyrimspecialedition/mods/5303)
#### [SKELETON](http://www.nexusmods.com/skyrimspecialedition/mods/17282)
#### [Skyrim SE Skill Interface Re-Texture](http://www.nexusmods.com/skyrimspecialedition/mods/1523)
#### [Smooth Sky mesh - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/18350)
#### [Stalhrim](http://www.nexusmods.com/skyrimspecialedition/mods/9447)
#### [Sweet Mother - The Night Mother Improvement](http://www.nexusmods.com/skyrim/mods/4947)
#### [The Elder Scrolls V Rewritten - Arvak SE](http://www.nexusmods.com/skyrimspecialedition/mods/11999)
#### [TROLL](http://www.nexusmods.com/skyrimspecialedition/mods/4682)
#### [Ultimate HD Torch](http://www.nexusmods.com/skyrim/mods/28060)
#### [Vivid Landscapes - Tundra Moss Revised](http://www.nexusmods.com/skyrim/mods/43221)
#### [WEBS S.E.](http://www.nexusmods.com/skyrimspecialedition/mods/4873)
#### [WISPMOTHER](http://www.nexusmods.com/skyrimspecialedition/mods/7638)

### Audiovisual - Trees
#### [HQ Tree Bark](http://www.nexusmods.com/skyrimspecialedition/mods/6556)
Choose the options you prefer. Install the Simply Bigger Trees patch.
#### [No More Hanging Moss](https://www.nexusmods.com/skyrimspecialedition/mods/16426)
Install _Hanging moss removal - partial - the moss around trees -_ mesh edits only. Without this mod you would get floating moss hanging from resized trees.
#### [Realistic Aspen Trees SE](http://www.nexusmods.com/skyrimspecialedition/mods/4423)
Choose 2k or 4k. Choose LodGen billboards (doesn't really matter, they will be overwritten by the next mod)
#### [Simply Bigger Trees SE](http://www.nexusmods.com/skyrimspecialedition/mods/5281)
Install the Realistic Aspen trees version of this mod.

## Audiovisual - Sounds & Music
#### [Audio Overhaul for Skyrim SE](http://www.nexusmods.com/skyrimspecialedition/mods/12466)
#### [Better Animal Footsteps](https://www.nexusmods.com/skyrim/mods/24805)
#### [Better Horse Pain Sounds](http://www.nexusmods.com/skyrim/mods/12608)
#### [Heart of the Beast - Werewolf Sound and Texture Overhaul](http://www.nexusmods.com/skyrim/mods/13779)
#### [IHSS - Improved Horse Step Sounds](http://www.nexusmods.com/skyrimspecialedition/mods/848)
#### [Lower Sounding Thieves Guild Door](http://www.nexusmods.com/skyrim/mods/1826)
#### [Realistic wolf howls](http://www.nexusmods.com/skyrim/mods/30636)
#### [Sound Hammering Sounds](http://www.nexusmods.com/skyrimspecialedition/mods/5592)
#### [Ultra Realistic Bow Shoot Sounds](https://www.nexusmods.com/skyrim/mods/27208)
#### [Ultra Realistic Crossbow Shoot Sounds](https://www.nexusmods.com/skyrim/mods/31274)



## Character Appearance
### Character Appearance - Body Mods
*This section replaces the vanilla body with the CBBE body. The CBBE body is chosen because of its versatility. Recommended presets makes the body look realistic or vanilla-ish. Using a body replacer is the only way to make sure the female body is compatible both with skin texture replacers and with mods that add new armors to the game.*\
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

### Character Appearance - Face Parts
#### [Beards](http://www.nexusmods.com/skyrimspecialedition/mods/1067)
#### [Brows](http://www.nexusmods.com/skyrimspecialedition/mods/1062)
#### [Female Vampires Have Fangs](http://www.nexusmods.com/skyrimspecialedition/mods/1211)
#### [KS Hairdos SSE](http://www.nexusmods.com/skyrimspecialedition/mods/6817)
#### [Maevan2’s Mature Skin Texture for CBBE – UNP](https://www.nexusmods.com/skyrimspecialedition/mods/26017)
*NSFW warning*\
In the installer, choose what you want, for example: high, CBBE slim, medium, lips, complexions, young, mature.
#### [Salt and Wind – Rough Hair for KS Hairdos SE](http://www.nexusmods.com/skyrimspecialedition/mods/16582)
#### [TDN Equipable Horns SE](http://www.nexusmods.com/skyrimspecialedition/mods/9224)
Yes, some Bosmer have antlers.\
*"It is also common among the Bosmer to wear decorative antlers on their foreheads, although rarely, individuals with real, magically-grown antlers can also be encountered."* [source](https://en.uesp.net/wiki/Lore:Bosmer) \
Skip this mod if you do not intend to use horns or antlers for your character.

### Character Appearance - NPC Overhauls
#### [Consistent Older People](http://www.nexusmods.com/skyrimspecialedition/mods/2977)

## Fixes
#### [(SKSE64) Havok Fix](http://www.nexusmods.com/skyrimspecialedition/mods/18160)
#### [1st Person Candlelight Fix](http://www.nexusmods.com/skyrimspecialedition/mods/9736)
#### [Bug Fixes SSE](http://www.nexusmods.com/skyrimspecialedition/mods/33261)
#### [Butterflies Land True](http://www.nexusmods.com/skyrimspecialedition/mods/29434)
#### [Butterflies Unchained](http://www.nexusmods.com/skyrimspecialedition/mods/29538)
#### [Critters Ain't Snitches - Animal and Monster Crime Reporting Fix - BETA](http://www.nexusmods.com/skyrimspecialedition/mods/15134)
#### [Dragon Stalking Fix](http://www.nexusmods.com/skyrimspecialedition/mods/14060)
#### [Enchantment Reload Fix SE](http://www.nexusmods.com/skyrimspecialedition/mods/21055)
#### [Eye Normal Map Fix SSE](http://www.nexusmods.com/skyrimspecialedition/mods/5445)
#### [Fuz Ro D-oh - Silent Voice](http://www.nexusmods.com/skyrimspecialedition/mods/15109)
#### [Hearthfires Houses Building Fix](http://www.nexusmods.com/skyrimspecialedition/mods/27298)
#### [Invisibility and Eyes Mesh Fix by HHaleyy](http://www.nexusmods.com/skyrimspecialedition/mods/14464)
#### [Modern Brawl Bug Fix](http://www.nexusmods.com/skyrimspecialedition/mods/1473)
#### [Skyrim Landscape and Water Fixes](http://www.nexusmods.com/skyrimspecialedition/mods/26138)
#### [Skyrim Project Optimization SE](http://www.nexusmods.com/skyrimspecialedition/mods/14084)
#### [SkyUI SE - Flashing Savegames Fix](http://www.nexusmods.com/skyrimspecialedition/mods/20406)
#### [SSE Engine Fixes (skse64 plugin)](http://www.nexusmods.com/skyrimspecialedition/mods/17230)
#### [Stay At The System Page - Updated](http://www.nexusmods.com/skyrimspecialedition/mods/19832)
#### [Waterbreathing Breathless Emerge SSE](http://www.nexusmods.com/skyrimspecialedition/mods/14485)
#### [Wiseman303's Flora Fixes](https://www.nexusmods.com/skyrimspecialedition/mods/28197)
Install the main file and the patch for SMIM.

## Gameplay
### Gameplay - AI & Combat
#### [Better Stealth AI for Followers](http://www.nexusmods.com/skyrimspecialedition/mods/17600)
#### [Follower Trap Safety](http://www.nexusmods.com/skyrimspecialedition/mods/2755)
#### [Tavern AI fix](http://www.nexusmods.com/skyrimspecialedition/mods/23107)
#### [TK Dodge SE](https://www.nexusmods.com/skyrimspecialedition/mods/15309)
#### [Ultimate Combat SE](http://www.nexusmods.com/skyrimspecialedition/mods/17196)

### Gameplay - Classes & Races
#### [Aetherius - A Race Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/26686)
#### [Class Overhaul Re-Imagined (SkyRem - Cori)](https://www.nexusmods.com/skyrimspecialedition/mods/24808)
#### [Experience](http://www.nexusmods.com/skyrimspecialedition/mods/17751)
Do not activate this mod yet. Waith until you have left the first cell of Alternate Start to avoid getting experience when different mods do their initial setup routines.
#### [Growl - Werebeasts of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/31245)
#### [Sacrosanct - Vampires of Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/3928)

### Gameplay - Crafting
#### [Ars Metallica - Smithing Enhancement](https://www.nexusmods.com/skyrimspecialedition/mods/321)

### Gameplay - Economy & Item Balance
#### [Trade and Barter](http://www.nexusmods.com/skyrimspecialedition/mods/23081)
#### [Weapons Armor Clothing and Clutter Fixes](http://www.nexusmods.com/skyrimspecialedition/mods/18994)

### Gameplay - Immersion & Role-playing
#### [Campfire - Complete Camping System](http://www.nexusmods.com/skyrimspecialedition/mods/667)
Hide or delete the file _SKSE/Plugins/PapyrusUtil.dll_. It is outdated and we need to use the newer one from PapyrusUtil SE.
#### [Campfire and Frostfall - Unofficial SSE Update](http://www.nexusmods.com/skyrimspecialedition/mods/17925)
#### [Carriage and Ferry Travel Overhaul](http://www.nexusmods.com/skyrimspecialedition/mods/8379)
Install patches for Immersive Citizens - AI Overhaul and Dawnstar.
#### [Daedric Voices](https://www.nexusmods.com/skyrimspecialedition/mods/32090)
Install the main file and the Growl patch.
#### [Disease Descriptions for the Immersive Adventurer SE](http://www.nexusmods.com/skyrimspecialedition/mods/26992)
#### [ElSopa - Campfire HD SE](http://www.nexusmods.com/skyrimspecialedition/mods/24511)
#### [Improved Traps](http://www.nexusmods.com/skyrimspecialedition/mods/17592)
#### [Lenient Survival](https://www.nexusmods.com/skyrimspecialedition/mods/13087)
For users of Survival Mode only. Do not install the optional file. A plugin to remove carry weight penalty is found the guides patches.
#### [Lock Related Loot](http://www.nexusmods.com/skyrimspecialedition/mods/11342)
#### [Nether's Follower Framework](http://www.nexusmods.com/skyrimspecialedition/mods/18076)
Choose the following: 
- Followers avoid traps
- Interesting NPC support
- Relationship Dialogue Overhaul
- RDO Comments
#### [No Lockpick Activate (SKSE) - Updated](http://www.nexusmods.com/skyrimspecialedition/mods/26790)
#### [Ragdoll Paralysis Redux SE](https://www.nexusmods.com/skyrimspecialedition/mods/13575)
#### [Torches Ignite Oil](http://www.nexusmods.com/skyrimspecialedition/mods/13226)

### Gameplay - Magic & Abilities
#### [Mundus - A Standing Stone Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33411)
#### [Mysticism - A Magic Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/27839)
Install the main file and the Survival patch. Do not install the Audio Overhaul Skyrim patch.
#### [Thunderchild - Epic Shouts and Immersion](http://www.nexusmods.com/skyrimspecialedition/mods/1460)

### Gameplay - Quests & Stories
#### [The Brotherhood of Old - Open Beta - SSE](http://www.nexusmods.com/skyrimspecialedition/mods/15322)
#### [Clockwork (SSE)](http://www.nexusmods.com/skyrimspecialedition/mods/4155)
#### [Dawnguard and Clan Volkihar Epilogues](http://www.nexusmods.com/skyrimspecialedition/mods/12098)
#### [Even Better Quest Objectives](http://www.nexusmods.com/skyrimspecialedition/mods/159)
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
#### [The Paarthurnax Dilemma](http://www.nexusmods.com/skyrimspecialedition/mods/365)

### Gameplay - Skills & Perks
#### [Adamant - A Perk Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/30191)

### Gameplay - User Interface
#### [Better Container Controls for SkyUI](http://www.nexusmods.com/skyrimspecialedition/mods/25271)
#### [Better Dialogue Controls](http://www.nexusmods.com/skyrimspecialedition/mods/1429)
#### [Better MessageBox Controls](http://www.nexusmods.com/skyrimspecialedition/mods/1428)
#### [Font Overhaul - Natural Typefaces for Skyrim](http://www.nexusmods.com/skyrimspecialedition/mods/2880)
#### [RaceMenu](http://www.nexusmods.com/skyrimspecialedition/mods/19080)
#### [UIExtensions](https://www.nexusmods.com/skyrimspecialedition/mods/17561)
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

### Locations - Overhauls
#### [Immersive College of Winterhold](http://www.nexusmods.com/skyrimspecialedition/mods/17004)
Choose 
- desaturated book covers
- RLS SSE Patch
- Better Dynamic Snow Patch
- Skyrim Project Optimization SSE Patch.
#### [Immersive Dawnguard Dayspring Pass SE](http://www.nexusmods.com/skyrimspecialedition/mods/4126)

### Locations - Arthmoor's towns and villages
#### [Darkwater Crossing](https://www.nexusmods.com/skyrimspecialedition/mods/326)
#### [Dragon Bridge](https://www.nexusmods.com/skyrimspecialedition/mods/8683)
#### [Dawnstar](https://www.nexusmods.com/skyrimspecialedition/mods/13607)
#### [Falkreath](https://www.nexusmods.com/skyrimspecialedition/mods/21266)
#### [Karthwasten](https://www.nexusmods.com/skyrimspecialedition/mods/350)
#### [Ivarstead](https://www.nexusmods.com/skyrimspecialedition/mods/349)
#### [Keld-Nar](https://www.nexusmods.com/skyrimspecialedition/mods/14353)
#### [Kynesgrove](https://www.nexusmods.com/skyrimspecialedition/mods/351)
#### [Rorikstead](https://www.nexusmods.com/skyrimspecialedition/mods/16881)
#### [Shor's Stone](https://www.nexusmods.com/skyrimspecialedition/mods/354)
#### [Soljund's Sinkhole](https://www.nexusmods.com/skyrimspecialedition/mods/358)
#### [Telengard](https://www.nexusmods.com/skyrimspecialedition/mods/17423)
#### [The Fall of Granite Hill](https://www.nexusmods.com/skyrimspecialedition/mods/22512)
#### [Whistling Mine](https://www.nexusmods.com/skyrimspecialedition/mods/367)

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
#### [Embers HD](http://www.nexusmods.com/skyrimspecialedition/mods/14368)
Reinstall and add the Campfire patch.
#### [Realistic Water Two](http://www.nexusmods.com/skyrimspecialedition/mods/2182)
Reinstall and add patches for Falskaar and Wyrmstooth.
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