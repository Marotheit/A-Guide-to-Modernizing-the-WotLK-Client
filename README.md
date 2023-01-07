# A Guide to Modernizing the Wrath of the Lich King (3.3.5a) Client

**Hello there!** My name is _**Marotheit**_, and I wanted to share a guide on modernizing your World of Warcraft: Wrath of the Lich King (3.3.5a) client installation for private servers. This guide encompasses a lot of information I found spread out amongst the World of Warcraft forumverse, assembled in one location for my friends, family, and fellow nerds.

In this guide, I will discuss the basics of client-side patches, provide sources (and mirrors) to popular patches, cover some additional visual settings, and end with some additonal steps. Let us begin.

> ### Note: This guide has not been endorsed or approved by any particular private servers or their moderation teams. You may encounter technical issues, game crashes, or even banishment. I _personally_ have not had any issues, but do continue at your own risk.

## Client-Side Patches:

Client-Side Patches are pre-compiled data packages for World of Warcraft that are initialized upon launching the game. Patches often contain enhancements for the game in the form of improved textures, updated models, and various interface changes (like custom loading screens or music). These patches are shared in `.MPQ` format and stored in the `World of Warcraft\Data` folder.

The best place to find patches you may be interested in includes the [Model Changing Network](https://model-changing.net/), the now defunct [Modcraft.io](https://web.archive.org/web/20210123222835/www.modcraft.io/index.php) through the [Wayback Machine](https://web.archive.org/web/20210123222835/www.modcraft.io/index.php), and various private server forums around the internet.

Applying certain patches may have an impact on your client's performance, so be wary of your framerate. In addition, running many patches has been known to max out the 2GB of available memory the Wrath of the Lich King client has access to, leading to random game crashes. You can fix this problem by using [Large Address Aware](https://www.techpowerup.com/forums/threads/large-address-aware.112556/) (if you have enough memory) to allow the client access up to 4GB of available memory.

It is important to mention that because of the way many files are shared between different systems in the game, some patches may have unforeseen issues and not all patches are compatible with one another, so you must be careful about which ones you decide to add to your installation. As a general rule of thumb, patches that both effect the same item(s) (such as lighting, animations, models, textures, music, etc.) may not be compatible with one another.

## Installing Client-Side Patches:
After you have downloaded all components of a patch and ensured the game is fully closed, unzip all folders until you see `patch-X.MPQ`. All patches should be placed in `World of Warcraft\Data`, relative to your Wrath of the Lich King client location. If you have two patches with the same name, rename the number or letter following `patch-` to an available number or letter.

You should _**never**_ overwrite the original patches provided to you during the initial setup process (this being `common.MPQ`, `common-2.MPQ`, `expansion.MPQ`, `lichking.MPQ`, `patch.MPQ`, `patch-2.MPQ`, or `patch-3.MPQ`), otherwise your installation will cease to work.

Patches are initialized in numerical, then alphabetical order. In rare instances, some patches must load before others to ensure compatibility. You can find the initialization order I use for the below patches [here](https://gist.github.com/Marotheit/3e20a4bf1153f539de65852be46192b8).

If you wish to uninstall a patch, simply delete it from the `World of Warcraft\Data` folder.

## Patch Recommendations:
Below is a list of popular client-side patches for Wrath of the Lich King, game version 3.3.5a. The intent of most of these patches is to enhance your Wrath of the Lich King installation with assets from newer World of Warcraft releases.

While each source *should* contain the most up-to-date version of any given patch, the original threads are sometimes removed with no prior warning by their hosts, and have been mirrored here for ease-of-access and archival purposes. I did my best to include before and after examples for many of the patches, when applicable.

### Model Changes:
- [Updated Battleground Models](https://www.mediafire.com/file/9twr8os3e20ug8d/Updated_Battleground_Models_Patch.zip) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the appearance of battleground models and textures to more closely resemble those introduced in Cataclysm and onward.
- [Updated Character Models](https://www.mediafire.com/file/95a79ypkpjuszt6/Updated_Character_Models_Patch.zip) by [Leeviathan and vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the player and humanoid NPC models to use models introduced in Warlords of Draenor. [[Before/After](https://user-images.githubusercontent.com/26125775/147448601-a8460dcf-cde5-4a88-a135-94eab84f7997.png)]
- [Updated Creature Models](https://www.mediafire.com/file/opuh1c62i8a1kuc/Updated_Creature_Models_Patch.zip) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the creature, enemy, and mount models to more closely resemble those introduced in Cataclysm and onward. [[Before/After 1](https://user-images.githubusercontent.com/26125775/147448664-ef2f8c5b-c705-42ee-806e-cffb8e690c0d.png)] | [[Before/After 2](https://user-images.githubusercontent.com/26125775/147448041-c0090ca9-0149-4f8a-8e1e-43a13afaa905.png)]
- [Updated Item Models](https://www.mediafire.com/file/9qpcs95zlkex3ft/Updated_Item_Models_Patch.zip) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates many item models to more closely resemble those introduced in Cataclysm and onward.
- [Updated Spell Animations](https://www.mediafire.com/file/4qh6pghqwbhovvm/Updated_Spell_Animations_Patch.zip) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) reimagines many spell animations to feature a more modern feel. _**As an important note, some servers feature an anti-cheat that flags players with modified spells databases. Continue at your own risk!**_

### Texture Changes:
- [Sunlight Alpha Texture](https://www.mediafire.com/file/o89be66zjk8l7m2/Sunlight_Alpha_Texture_Patch.zip) by [Nicolas](https://model-changing.net/files/file/129-sun-light-alpha-wow/) modifies the texture assigned to the sun to make it appear more realistic, resembling the texture used in the Alpha build of World of Warcraft. This is included in [YetAnotherWaterPatch](https://www.mediafire.com/file/91els1b3hafmnln/YetAnotherWaterPatch.zip) thanks to [vulpe](https://model-changing.net/files/file/212-improved-water-for-335a-working/).
- [Updated Environment Textures](https://www.mediafire.com/file/kv8jddcbvmcm1iv/Updated_Environment_Textures_Patch.zip) by [Finsternis and vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the environment tileset textures used throughout the world. [[Before/After](https://user-images.githubusercontent.com/26125775/147499245-3d88d6b1-cb8e-42d2-a62e-d1faacb62ba8.png)]
- [Upscaled Clothing Textures](https://www.mediafire.com/file/ayjw08lwtrqzbd1/Upscaled_Clothing_Textures_Patch.zip) by [sh1tdev and vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) upscales all Classic, Burning Crusade, and Wrath of the Lich King clothing textures by 4x to allow clothing to appear sharper and more detailed. [[Before/After 1](https://user-images.githubusercontent.com/26125775/147497660-8649706b-eea2-4f36-abbf-2da3da64c873.png)] | [[Before/After 2](https://user-images.githubusercontent.com/26125775/147450940-bd33dc24-d787-462b-b103-72c7c95f7f1f.png)]

### Other Patches:
- [Blood Mod](https://www.mediafire.com/file/joqnhqjvx2ya6fw/Blood_Mod_Patch.zip) by [Inico](https://model-changing.net/files/file/128-blood-mod-for-wotlk-and-cata-v3/) adds blood puddle animations to combat that disappear over time.
- [Dungeon Maps](https://www.mediafire.com/file/c7xzo65mlrpbrks/Dungeon_Maps_Patch.zip) by [Trimitor](https://forum.warmane.com/showthread.php?t=424250) adds instance maps for Classic and Burning Crusade instances. Be sure to also install the included `WDM` AddOn.
- [LoginTweaks](https://www.mediafire.com/file/vzw3282zdhe88ty/LoginTweaks.zip) by [Marotheit](https://model-changing.net/files/file/307-logintweaks-wotlk/) removes much of the extra login screen clutter and adds a convenient 'Remember Password' option. Also available in an [ElvUI flavor](https://www.mediafire.com/file/bopbpw319m42uit/LoginTweaks_%2528ElvUI_Flavor%2529.zip). _**As an important note, using the 'Remember Password' feature stores your password in plain text, so understand you would be forgoing security in exchange for convenience.**_
- [Old World Music Rescore](https://www.mediafire.com/file/kw0059s4vfxxhwy/Old_World_Music_Rescore_Patch.zip) by [Leeviathan](https://model-changing.net/gc/12-leeviathans-old-world-music-rescore/) replaces the [older vanilla zone music](https://www.youtube.com/watch?v=CRa537H1B_4) with the [rescored music](https://www.youtube.com/watch?v=qAY0T6lbPr8) introduced in Cataclysm.
- [Shadowlands Menu](https://www.mediafire.com/file/0mudf3dsq14ba1f/Shadowlands_Menu_Patch.zip) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the login screen, character creation/selection menu, and loading screens to the ones introduced in Shadowlands. [My flavor](https://www.mediafire.com/file/tqbgboqevwueufo/Shadowlands_Menu_Patch_%2528Marotheit%2527s_Flavor%2529.zip) removes the loading screens and character creation icons. [[Before/After](https://user-images.githubusercontent.com/26125775/147440746-b7f79e9f-3ff8-40ea-aa02-0bb68dda7aec.png)]
- [Updated Loading Screens](https://www.mediafire.com/file/sp9jz047xyrtrh2/Updated_Loading_Screens_Patch.zip) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the loading screens to use artwork introduced in Legion.
- [YetAnotherWaterPatch](https://www.mediafire.com/file/91els1b3hafmnln/YetAnotherWaterPatch.zip) by [Milly](https://web.archive.org/web/20160902001729/http://modcraft.superparanoid.de/viewtopic?f=59&t=8483), [Elrena](https://model-changing.net/files/file/3-cata-water-for-wrath-of-the-lich-king/), [Inico](https://model-changing.net/tutorials/article/90-wotlk-procedural-water-understanding-and-improving-it/), [vulpe](https://model-changing.net/files/file/212-improved-water-for-335a-working/?tab=comments), and [Marotheit](https://github.com/Marotheit) replaces the water, lava, and slime textures to make them appear similar to textures introduced in later expansions. I've experimented with many of the popular water mods out there and compiled the assets I liked most from all of them. [[Before/After](https://user-images.githubusercontent.com/26125775/147507984-625a77c0-867b-40be-9a35-c83ebc7880ca.png)]

## Visual Settings
Beyond basic graphical settings (i.e., the standard graphical presets) there are console commands you can run in-game to increase graphical variables higher than Blizzard allowed through the in-game video settings menu. On that note, you should probably only perform these commands on a higher-end PC. Running the following commands will result in extra details around the world becoming more noticeable.

You should finalize your video settings _**before**_ attempting to use these macros, as modifying any graphical options through the video settings menu will reset all graphical variables to their default values. Similarly, if you try the below console commands and do not enjoy the extra graphical fidelity, simply change your graphical preset in the video settings menu to reset all graphical variables to default. You can use the [console variables wiki page](https://wowpedia.fandom.com/wiki/Console_variables) to see what each command changes individually.

The commands below have been seperated into three easy to use macros for your convenience, but can be performed individually if you prefer.

Ultra+ Graphics 1:
```
/console environmentDetail 150
/console farclip 777
/console ffxnetherworld 1
/console ffxspecial 1
/console groundEffectDensity 192
/console groundEffectDist 140
/console groundEffectFade 1000
/console gxmultiesample 8
/console horizonFarclipScale 6
```

Ultra+ Graphics 2:
```
/console particleDensity 100
/console reflectionMode 3
/console shadowmode 3
/console shadowtexturesize 2048
/console skycloudlod 3
/console spellEffectLevel 200
/console ssao 2
/console terrainMipLevel 0
/console textureFilteringMode 5
```

Ultra+ Graphics 3:
```
/console violencelevel 5
/console waterDetail 3
/console weatherDensity 3
```

## Extra Steps
At this point, your graphics should appear more in line with modern version of World of Warcraft. Below are a few extra steps you can use to take your installation even further.

### Using a Batch File to Clear Your Cache Before Startup
You can use a batch file to clear your cached files before you launch World of Warcraft. This is a good way to avoid common issues from appearing in-game. Simply download [this batch file](https://www.mediafire.com/file/u2zcm0y5clhis1q/Clear_Cache_Batch.zip) (or create a batch file with the text below) and place it into your Wrath of the Lich King client install location. You should launch the game using this batch file from now on.
```
@echo off
rd /s /q "Cache"
start WoW.exe
exit
```

### Push Your Graphical/Performance Configuration Further
You can set some graphical and performance settings even higher by editing your configuration file. Navigate to `World of Warcraft\WTF` and open `Config.wtf` in a notepad. Add the lines below to push your World of Warcraft settings even further.
```
SET M2Faster "3"
SET gxTextureCacheSize "512"
SET objectFade "0"
SET screenshotQuality "10"
```

Additionally, you can overwrite the lines below to enable Windowed Fullscreen, which many players are unable to enable successfully from within the client.
```
SET gxWindow "1"
SET gxMaximize "1"
SET windowResizeLock "1"
```

After your done, save the configuration file and open World of Warcraft to observe your changes. If the game has issues loading, you can simply delete `Config.wtf` (which will reset all your saved options) and try again.

### Install [Discord Rich Presence for World of Warcraft](https://github.com/wodim/wow-discord-rich-presence)
This enables World of Warcraft (with the help of Python) to interact with Discord Rich Presence to display gameplay information beside your user profile. Useful for guilds and friend circles who use Discord.

### Install [ElvUI-Glues-WotLK](https://github.com/Marotheit/ElvUI-Glues-WotLK)
This retextures the login, character selection, and character creation screens for use with ElvUI. This is included in the [ElvUI version of LoginTweaks](https://www.mediafire.com/file/bopbpw319m42uit/ElvUI-LoginTweaks.zip), so feel free to skip this step if you decide to use [LoginTweaks](https://www.mediafire.com/file/bopbpw319m42uit/ElvUI-LoginTweaks.zip).

## Conclusion
Thank you for your time. If you see anything that can be improved or expanded upon (or especially if you find a nice patch,) please let me know by creating an issue [here](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/issues). You can view the changelog [here](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/blob/main/CHANGELOG.md). I am always interested in improving the guide. Shoutouts to vvladoon, Leeviathan, Nicolas, Finsternis, sh1tdev, Inico, Trimitor, Milly, Elrena, and vulpe for all their work. They inspired me to write this guide.

I use these settings on [ChromieCraft](https://www.chromiecraft.com/en/), so if you appreciate this guide and decide to discover your new home, add me as a friend and feel free to use me as a Recruit-a-Friend. My Account ID is `40720`.

—Marotheit.
