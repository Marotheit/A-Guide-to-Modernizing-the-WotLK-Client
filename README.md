# A Guide to Modernizing the Wrath of the Lich King (3.3.5a) Client

**Hello there!** My name is _**Marotheit**_, and I wanted to share a guide on modernizing your World of Warcraft: Wrath of the Lich King (3.3.5a) client installation for private servers. This guide encompasses a lot of information I found spread out amongst the World of Warcraft forumverse, assembled in one location for my friends, family, and fellow nerds.

In this guide, we will discuss the basics of client-side patches, provide sources to popular patches, cover some additional visual settings, and end with some further steps to modernize the client. Let us begin.

> ### Note: This guide has not been endorsed or approved by any particular private servers or their moderation teams. You may encounter technical issues, game crashes, or even banishment. I _personally_ have not had any issues, but do continue at your own risk.

## Client-Side Patches:

Client-Side Patches are pre-compiled data packages for World of Warcraft that are initialized upon launching the game. Patches often contain enhancements for the game in the form of improved textures, updated models, and various interface changes (like custom loading screens or music). These patches are shared in `.MPQ` format and stored in the `World of Warcraft\Data` folder.

The best place to find patches you may be interested in includes [WoW  Modding](https://www.wowmodding.net/), the now defunct [Modcraft.io](https://web.archive.org/web/20210123222835/www.modcraft.io/index.php) through the [Wayback Machine](https://web.archive.org/web/20210123222835/www.modcraft.io/index.php), and various private server forums around the internet.

Applying certain patches may have an impact on your client's performance, so be wary of your framerate. In addition, running many (or large) patches has been known to max out the 2GB of available memory the Wrath of the Lich King client has access to, leading to random game crashes. You can (usually) remedy this problem by using [WoWPatcher](https://github.com/anzz1/WoWPatcher335) or [Large Address Aware](https://www.techpowerup.com/forums/threads/large-address-aware.112556/) (if you have enough memory) to allow the client access up to 4GB of available memory, but be sure to make a backup of the executable in the event you need to revert to it at a later date.

It is important to mention that because of the way many files are shared between different systems in the game, some patches may have unforeseen issues and not all patches are compatible with one another, so you must be careful about which ones you decide to add to your installation. As a general rule of thumb, patches that both effect the same item(s) (such as lighting, animations, models, textures, music, etc.) may not be compatible with one another.

## Installing Client-Side Patches:
After you have downloaded all components of a patch and ensured the game is fully closed, unzip all packages until you see `patch-X.MPQ`. All patches should be placed in `World of Warcraft\Data`, relative to your Wrath of the Lich King client location. If you have two patches with the same name, rename the number or letter following `patch-` to an available number or letter.

You should _**never**_ overwrite the original patches provided to you during the initial setup process (this being `common.MPQ`, `common-2.MPQ`, `expansion.MPQ`, `lichking.MPQ`, `patch.MPQ`, `patch-2.MPQ`, or `patch-3.MPQ`), otherwise your installation will cease to work.

Patches are initialized in numerical, then alphabetical order. In rare instances, some patches must load before others to ensure compatibility. You can find the recommended initialization order for the below patches [here](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/blob/main/PatchInitializationOrder.md), should you choose to install patches manually instead of utilizing [Reznik's WotLK Boost](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/tree/main?tab=readme-ov-file#rezniks-wotlk-boost), which is a high quality all-in-one solution.

If you wish to uninstall a patch, simply delete it from the `World of Warcraft\Data` folder.

## Patch Recommendations:
Below is a list of popular client-side patches for Wrath of the Lich King, game version 3.3.5a. The intent of most of these patches is to enhance your Wrath of the Lich King installation with assets from newer World of Warcraft releases.

While each source *should* contain the most up-to-date version of any given patch, the original threads are sometimes removed with no prior warning by their hosts, and have been mirrored when required. I did my best to include before and after examples for many of the patches, when applicable.

Any patches that are formatted using the `patch-RU-X.MPQ` file naming scheme should be renamed to `patch-X.MPQ` to ensure they work on English clients.

### Reznik's WotLK Boost:

[Reznik Shaman](https://reznik-fandom-com.translate.goog/wiki/Reznik_Wiki?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) has released v1.1.1 of his [WotLK Boost](https://reznik-fandom-com.translate.goog/wiki/WotLK_Boost?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) patch, which can be downloaded [here](https://reznik.fandom.com/wiki/WotLK_Boost#Download). This patch combines many of the patches listed below in a single patch, including updated character/creature/item models, spell animations, 8x upscaled environment/clothing textures, the blood mod, and updated liquid textures. This patch also features zero encryption, so adventurous players can modify the contents to their heart's content using tools such as [Ladik's MPQ Editor](https://www.hiveworkshop.com/threads/ladiks-mpq-editor.249562/).

*As a personal side note, I have switched to using Reznik's WotLK Boost patch almost exclusively (after making some [personal modifications](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/issues/10#issuecomment-2481002297) using [Ladik's MPQ Editor](https://www.hiveworkshop.com/threads/ladiks-mpq-editor.249562/)) instead of using individual patches. The quality of this patch is really impressive and Reznik has a strong history in modifying the game. This patch may not be supported on all servers, but I cannot recommend it enough.*

### Model Changes:
- [Updated Character Models](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-H.MPQ`) by [Leeviathan](https://www.wowmodding.net/topic/1133-release-wotlk-creature-models-for-wotlk-author-finsternis/#comment-7029) and [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the player and humanoid NPC models to use models introduced in Warlords of Draenor. [[Before/After](https://user-images.githubusercontent.com/26125775/147448601-a8460dcf-cde5-4a88-a135-94eab84f7997.png)]
  -  *As an **important** note, this patch will sometimes cause issues when interacting with Goblins. If you run into this issue, simply uninstalling the patch will allow you to converse with Goblins.*
- [Updated Creature Models](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-A.MPQ`) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the creature, enemy, and mount models to more closely resemble those introduced in Cataclysm and onward. [[Before/After 1](https://user-images.githubusercontent.com/26125775/147448664-ef2f8c5b-c705-42ee-806e-cffb8e690c0d.png)] | [[Before/After 2](https://user-images.githubusercontent.com/26125775/147448041-c0090ca9-0149-4f8a-8e1e-43a13afaa905.png)]
- [Updated Item Models](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-I.MPQ`) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates many item models to more closely resemble those introduced in Cataclysm and onward.
  -  *As a note, this patch is listed to be incompatible with Updated Character Models, but I have yet to personally run into any issues.*
- [Updated Spell Animations](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-S.MPQ`) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) reimagines many spell animations to feature a more modern feel.
  - *As a **VERY** important note, some servers feature an anti-cheat that flags players with modified spells databases. **Continue at your own risk!***

### Texture Changes:
- [Sunlight Alpha Texture](https://www.wowmodding.net/files/file/119-sun-light-alpha-wow/) by [Nicolas](https://www.wowmodding.net/files/file/119-sun-light-alpha-wow/) modifies the texture assigned to the sun to make it appear more realistic, resembling the texture used in the Alpha build of World of Warcraft.
- [Updated Battleground Textures](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-U.MPQ`) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the appearance of battleground models and textures to more closely resemble those introduced in Cataclysm and onward.
- [Updated Environment Textures](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-T.MPQ`) by [Finsternis](https://www.wowmodding.net/topic/1132-environment-and-city-textures-author-finsternis/#comment-7027) and [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the environment tileset textures used throughout the world. [[Before/After](https://user-images.githubusercontent.com/26125775/147499245-3d88d6b1-cb8e-42d2-a62e-d1faacb62ba8.png)]
- [Upscaled Clothing Textures](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-E.MPQ`) by [sh1tdev](https://www.wowmodding.net/files/file/199-vanilla-tbc-and-wotlk-clothing-textures-upscaled-for-335/page/2/?tab=comments#comment-1116) and [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) upscales all clothing textures by 4x to allow clothing to appear sharper and more detailed. [[Before/After 1](https://user-images.githubusercontent.com/26125775/147497660-8649706b-eea2-4f36-abbf-2da3da64c873.png)] | [[Before/After 2](https://user-images.githubusercontent.com/26125775/147450940-bd33dc24-d787-462b-b103-72c7c95f7f1f.png)]

### Other Patches:
- [Blood Mod](https://www.wowmodding.net/files/file/118-blood-mod-for-wotlk-and-cata-v3/) by [Inico](https://www.wowmodding.net/files/file/118-blood-mod-for-wotlk-and-cata-v3/) adds blood puddle animations to combat that disappear over time.
- [Clean Icons (Mechagnome Edition)](https://github.com/AcidWeb/Clean-Icons-Mechagnome-Edition/releases) by [suicidalkatt](https://www.wowinterface.com/downloads/info19844) and [AcidWeb](https://www.wowinterface.com/downloads/info25064-CleanIcons-MechagnomeEdition.html) upscales and homogenizes the icons to appear sharper and more detailed.
  - *Because this is not a patch, but texture replacements, they should be placed in `World of Warcraft\Interface\ICONS`, relative to your Wrath of the Lich King client location.*
- [Dungeon Maps](https://forum.warmane.com/showthread.php?t=424250) by [Trimitor](https://forum.warmane.com/showthread.php?t=424250) adds instance maps for Classic and Burning Crusade instances.
  - *Be sure to also install the included `WDM` AddOn.*
- [LoginTweaks](https://www.mediafire.com/file/vzw3282zdhe88ty/LoginTweaks.zip) by [Marotheit](http://web.archive.org/web/20220119220821/https://model-changing.net/files/file/307-logintweaks-wotlk/) removes much of the extra login screen clutter and adds a convenient 'Remember Password' option. Also available in an [ElvUI flavor](https://www.mediafire.com/file/bopbpw319m42uit/LoginTweaks_%2528ElvUI_Flavor%2529.zip).
  - *As a **VERY** important note, using the 'Remember Password' feature stores your password in plain text, so understand you would be forgoing security in exchange for convenience.*
- [Old World Music Rescore](https://www.mediafire.com/file/kw0059s4vfxxhwy/Old_World_Music_Rescore_Patch.zip) by [Leeviathan](https://model-changing.net/gc/12-leeviathans-old-world-music-rescore/) replaces the [older vanilla zone music](https://www.youtube.com/watch?v=CRa537H1B_4) with the [rescored music](https://www.youtube.com/watch?v=qAY0T6lbPr8) introduced in Cataclysm.
- [Shadowlands Menu](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Main Patches → `Patch-RU-L.MPQ`) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the login screen, character creation/selection menu, and loading screens to the ones introduced in Shadowlands. [My flavor](https://www.mediafire.com/file/tqbgboqevwueufo/Shadowlands_Menu_Patch_%2528Marotheit%2527s_Flavor%2529.zip) removes the loading screens and character creation icons. [[Before/After](https://user-images.githubusercontent.com/26125775/147440746-b7f79e9f-3ff8-40ea-aa02-0bb68dda7aec.png)]
- [Updated Loading Screens](https://forum-uwow-biz.translate.goog/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp) (Section 4 → Additional Patches → `Patch-RU-R.MPQ`) by [vvladoon](https://forum.uwow.biz/threads/cvpatch-collection-visual-patch-lich-king-3-3-5.296264/) updates the loading screens to use artwork introduced in Legion.
- [Project Epoch Water Patch](https://discord.gg/mzCSaZYWuC) (Project Epoch Discord → Announcements → `Patch-W.MPQ`) by [Intra](https://discord.gg/mzCSaZYWuC) replaces the water, lava, and slime textures to make them appear similar to textures introduced in later expansions, while also adhering to the limitations of the Vanilla client.

## Visual Settings
Beyond basic graphical settings (i.e., the standard graphical presets) there are console commands you can run in-game to increase graphical variables higher than Blizzard allowed through the in-game video settings menu. On that note, you should probably only perform these commands on a higher-end PC. Running the following commands will result in extra details around the world becoming more noticeable.

You should finalize your video settings _**before**_ attempting to use these macros, as modifying any graphical options through the video settings menu will reset all graphical variables to their default values. Similarly, if you try the below console commands and do not enjoy the extra graphical fidelity, simply change your graphical preset in the video settings menu to reset all graphical variables to default. You can use the [console variables wiki page](https://wowpedia.fandom.com/wiki/Console_variables) to see what each command changes individually.

The commands below have been seperated into three easy to use macros for your convenience, but can be performed individually if you prefer.

Ultra+ Graphics 1:
```
/console environmentDetail 150
/console farclip 1600
/console ffxnetherworld 1
/console ffxspecial 1
/console groundEffectDensity 256
/console groundEffectDist 140
/console groundEffectFade 1277
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
/console spellEffectLevel 150
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

## ReShade
[ReShade](https://reshade.me/) is a post-processing injector that can add ambient occlusion, anti-aliasing, color correction, film grain, depth of field effects, and more visual effects to games that do not normally include this functionality. This can provide graphical improvements that would normally be impossible using an unmodified World of Warcraft client.

> Through testing, I have discovered the Wrath of the Lich King client is only compatible with ReShade versions 4.9.1 and below. If someone is able to get the latest version of ReShade working with the client, feel free to message me and I'll update the guide to the latest version.

To install and configure ReShade, follow the step below.

>1.) Download [ReShade v4.9.1](https://www.mediafire.com/file/32o5pwxibc8m7rz/ReShade_Setup_v4.9.1.zip), and extract the zip to a location of your choosing.
>
>2.) Launch the downloaded ReShade Setup executable.
>
>3.) Click the 'Click here to select a game and manage its ReShade installation' button and navigate to (and select) the World of Warcraft executable.
>
>4.) Select 'Direct3D 9' as the rendering API.
>
>5.) You will be prompted to select the effects packages you wish to install. I recommend the default options (the full 'Standard effects' installation and the full 'SweetFX' installation). Click the 'OK' button when you have completed this step.
>
>6.) At this point, assuming the installation was successful, you may exit the ReShade Setup window.

Upon opening the World of Warcraft client, you will see a ReShade toast at the top of the screen, prompting you to press the `Home` key to begin the ReShade tutorial. Any changes are reflected in real time, so find a scenic spot in the world and adjust settings to what looks best for you.

## Extra Steps
At this point, your graphics should appear more in line with modern version of World of Warcraft. Below are a few extra steps you can use to take your installation even further.

### Using RCEPatcher to Remove the Remote Code Execution Vulnerability
[RCEPatcher](https://github.com/stoneharry/RCEPatcher) should be used to patch a remote code execution vulnerability within the World of Warcraft executable. This vulnerability could allow a malicious private server owner to run any code they may choose on your computer, even without your knowledge. While this could allow for some useful server features (such as attempting to detect hackers/botters) it is also a rather large security concern. Follow the steps below to use [RCEPatcher](https://github.com/stoneharry/RCEPatcher) to patch your World of Warcraft executable.

>1.) Download the latest [RCEPatcher](https://github.com/stoneharry/RCEPatcher/releases/) binary (or ideally, build the binary yourself after reviewing the code) from the RCEPatcher repository.
>
>2.) Extract the binary zip into a folder you can remember.
>
>3.) After ensuring you have made a backup of your original World of Warcraft executable, copy it into the same folder as the RCEPatcher binary.
>
>4.) Open Windows PowerShell as an administrator and use the `cd` command to navigate to the RCEPatcher folder.
>
>5.) Run `.\RCEPatcher.exe "<path-to-Wow.exe>"`
>
>6.) `Wow-patched.exe` will be created. This new executable will be patched against remote code executions on servers. You may now move the `Wow-patched.exe` executable into your World of Warcraft installation folder and delete any previously downloaded/extracted files.

You should now use the newly created `Wow-patched.exe` to join servers more safely, but as always, you should play on servers you can trust and verify. If a server attempts to employ remote code execution, the World of Warcraft client will exit with an `ERROR #132 (0x85100084) Fatal Exception` error code, at which point you should be asking questions.

### Using WoWPatcher to Disable the Creation of the `Cache` folder
[WoWPatcher](https://github.com/anzz1/WoWPatcher335) has the ability to disable the creation of the `Cache` folder, which is a good way to avoid common issues from appearing in-game. Simply download [WoWPatcher](https://github.com/anzz1/WoWPatcher335), place your `Wow.exe` executable into the same folder as `WoWPatcher.exe`, and run WoWPatcher. You will be presented with a few different options to modify your World of Warcraft executable, such as applying Large Address Aware to allow the client access up to 4GB of available memory, and allowing interface edits for use with [LoginTweaks](https://www.mediafire.com/file/vzw3282zdhe88ty/LoginTweaks.zip).

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
```

After your done, save the configuration file and open World of Warcraft to observe your changes. If the game has issues loading, you can simply delete `Config.wtf` (which will reset all your saved options) and try again.

### Install [VoiceOver](https://github.com/mrthinger/wow-voiceover/releases)
This adds text-to-speech support for gossip and quest texts. Be sure you install both the 3.3.5a `Voiceover` AddOn and the `Vanilla Sounds` pack into your `AddOns` folder.

### Install [Discord Rich Presence for World of Warcraft](https://github.com/wodim/wow-discord-rich-presence)
This enables World of Warcraft (with the help of Python) to interact with Discord Rich Presence to display gameplay information beside your user profile. Useful for guilds and friend circles who use Discord.

### Install [ElvUI-Glues-WotLK](https://github.com/Marotheit/ElvUI-Glues-WotLK)
This retextures the login, character selection, and character creation screens for use with ElvUI. This is included in the [ElvUI version of LoginTweaks](https://www.mediafire.com/file/bopbpw319m42uit/ElvUI-LoginTweaks.zip), so feel free to skip this step if you decide to use [LoginTweaks](https://www.mediafire.com/file/bopbpw319m42uit/ElvUI-LoginTweaks.zip).

## Conclusion
Thank you for your time. If you see anything that can be improved or expanded upon (or especially if you find a nice patch,) please let me know by creating an issue [here](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/issues). You can view the changelog [here](https://github.com/Marotheit/A-Guide-to-Modernizing-the-WotLK-Client/blob/main/CHANGELOG.md). I am always interested in improving the guide. Shoutouts to vvladoon, Leeviathan, Nicolas, Finsternis, sh1tdev, Inico, Trimitor, Milly, Elrena, vulpe, and Reznik for all their work. They inspired me to write this guide.

—Marotheit.
