JK SUCKos Mod - 1.6.1.1

:: NOTE ::
See the included PDF to help guide you through the installation process (it has pictures!)


:: WARNING ::
While the core portion of this mod is relatively benign – as all it does is change the coordinates of star systems to match up to the Sarna coordinates – the optional 16 extra star systems do impact new campaigns started with those extra worlds, making those save unviable if you remove the mod.

In order to use the new systems, you will need to replace mod.json with mod - Activated new systems and Coord fix.json.  

In my testing, the extra systems only seem to impact New Campaigns started after the systems are added.  But, those game saves are then dependent on the new star systems being in the game.  Removing the systems will break those saves.

If you choose to do a full uninstall of the extra systems portion of the mod at a future date, prior to uninstalling, you should perform the following actions:
•	Log on to the Load Screen: 
o	Delete any sessions where you were using the extra 16 systems and could see them on the map.
o	Older games that were saved before applying this mod should be safe.
If you have errors post uninstall, try replacing the mod files (including restoring the VersionManifest and MetadataDatabase), then look through your saves and make sure none of them have these 16 systems in them.

:: ADDITIONAL NOTES ::
If you do decide to use the 16 extra systems, please note that the borders for the various powers are not properly drawn.  This results in star systems looking like they are not part of the faction they should belong to (as the border does not encompass them).  But, clicking on the world will reveal the correct faction owner.

:: Discussion Threads / Bug Report ::
https://www.nexusmods.com/battletech/mods/24?tab=posts
https://forum.paradoxplaza.com/forum/index.php?threads/mod-release-jk_suckos-star-system-coordinates-mod-optional-16-new-systems.1091293/
https://www.reddit.com/r/BattleTechMods/comments/8foysx/extra_variants_mod_star_systems_mod_and_minor/

:: REQUIREMENTS ::
•	BattleTech game is up to date with current branch patch 1.6.1 (honestly, it should work with almost any version, as it only changes the coordinates)
•	ModTek


:: FEATURES ::
This mod is 2 mods in 1, and can be added piecemeal into your game, depending on which portion(s) you want to use.  By default, it only adjusts the existing system coordinates.

You can replace the mod.json in the folder with either of the other 2 files to change what appears:

mod - Activated fix of coords only.json
•	Adjusts the coordinates of 161 starsystem files to match the Sarna / SUCKos coordinates
•	Renames the planet Camadeirre in its description to reflect proper spelling of the Star Systems name to Camadeierre.


mod - Activated new systems and Coord fix.json
•	Includes 16 new star systems to the game.
•	These systems become available whenever their parent realm opens up for jump routes.
starsystemsNotAdded

:: GENERAL OTHER STUFF ::
•	Follows BattleTech Modder community standard of being placed in a “mods” folder within the BattleTech StreamingAssets folder.

:: GAME ELEMENTS IMPACTED ::
Currently the mod has 2 modes:
1 – Update all planets to match Sarna coordinates.  This gives a more ‘accurate’ version of the star map, which more closely matches what is seen in the sourcebooks.  See details on this system on the Sarna site: http://www.sarna.net/wiki/BattleTechWiki:System_coordinates
2 – Update all planets to match Sarna coordinates and add in 16 new systems to visit.






:: INSTRUCTIONS ::
::: Adjusting the Star System Coordinates ::: 
1 - Create a mods folder in your //BATTLETECH/BattleTech_Data/StreamingAssets/ folder.
 

2 - Copy the JK_SUCKos sub-fodlers into the BATTLETECH/BattleTech_Data/StreamingAssets/mods folder.
 


3 - Navigate to your BATTLETECH/BattleTech_Data/StreamingAssets/Data folder and rename VersionManifest.csv to VersionManifest_Orig.csv (so you can more easily revert back)
 

4 - Copy one of the 6 VersionManifest.csv files from the mods/ zip folder to that location.  Pick one of the below, then copy to your BATTLETECH/BattleTech_Data/StreamingAssets/Data folder and rename it to VersionManifest.csv.
•	VersionManifest-A-0-SUCKos.csv – Adds all new star system coordinates and makes no other changes.
•	VersionManifest-A-1.csv – Adds all new star system coordinates.  Also adds in the JK_Variants-1-JKVariant.csv (if you wish to use both mods).
•	VersionManifest-A-2.csv – Adds all new star system coordinates.  Also adds in the JK_Variants-2-JKVariant_WeapAmmo.csv (if you wish to use both mods).
•	VersionManifest-A-3.csv – Adds all new star system coordinates.  Also adds in the JK_Variants-3-JKAll.csv (if you wish to use both mods).
•	VersionManifest-A-4.csv – Adds all new star system coordinates.  Also adds in the JK_Variants-4-JKAll_GTComCon.csv (if you wish to use both mods).
•	VersionManifest-A-5.csv – Adds all new star system coordinates.  Also adds in the JK_Variants-5-Everything.csv (if you wish to use both mods).

 

5 - Restart the game.  You should notice a shift in multiple star systems on the star map – this will appear in any campaign (old or new).

Alternatively - there is a file in the main folder called "VersionManifest - Lines Added - ExistingSystems" which includes all the lines that need to be added in, if you want to apply this mod over another mod.  I highly recommend that you place the lines in the same area as others of its kind and sort those sections alphabetically to look for conflicts.
NOTE – if you manually add those lines, you need to delete ALL the old starsystemdef_ lines prior.  There are mostly together in 1 cluster, and I usually delete those, then past/insert these lines.  HOWEVER, there are 2 starsystemdef_ files that appear further down the sheet and need to also be deleted (Alamagordo and Landmark).
Technically, you could just copy the contents of the starsystem folder directly into your \\StreamingAssets\data\starsystem folder - overwriting those 161 files.  This is the quick and dirty way to do it – and doesn’t require any changes to the VersionManifest.csv.
::: Adding the 16 Additional Star Systems :::
Perform steps 1 through 3 as above.  Things change at step 4.
4 - Copy one of the 6 VersionManifest.csv files from the mods/ zip folder to that location.  Pick one of the below, then copy to your BATTLETECH/BattleTech_Data/StreamingAssets/Data folder and rename it to VersionManifest.csv.  Note which # you use, as you need to use the matching # for the MetadataDatabase.
•	VersionManifest-B-0-SUCKos_NewSystems.csv – Adds all new star system coordinates and the 16 new systems.
•	VersionManifest-B-1.csv – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-1-JKVariant.csv (if you wish to use both mods).
•	VersionManifest-B-2.csv – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-2-JKVariant_WeapAmmo.csv (if you wish to use both mods).
•	VersionManifest-B-3.csv – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-3-JKAll.csv (if you wish to use both mods).
•	VersionManifest-B-4.csv – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-4-JKAll_GTComCon.csv (if you wish to use both mods).
•	VersionManifest-B-5.csv – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-5-Everything.csv (if you wish to use both mods).

 

5 - Navigate to your BATTLETECH/BattleTech_Data/StreamingAssets/MDD folder and rename MetadataDatabase.db to MetadataDatabase_Orig.db (so you can more easily revert back)
 

6 - Copy one of the 6 MetadataDatabase.db files from the mods/ zip folder to that location.  Pick one of the below, then copy to your BATTLETECH/BattleTech_Data/StreamingAssets/Data folder and rename it to MetadataDatabase.db.  The number you use should match the VersionManifest # you picked in step 4.
•	MetadataDatabase-B-0-SUCKos_NewSystems.db – Adds all new star system coordinates and the 16 new systems.
•	MetadataDatabase -B-1.db – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-1-JKVariant.csv (if you wish to use both mods).
•	MetadataDatabase -B-2.db – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-2-JKVariant_WeapAmmo.csv (if you wish to use both mods).
•	MetadataDatabase -B-3.db – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-3-JKAll.csv (if you wish to use both mods).
•	MetadataDatabase -B-4.db – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-4-JKAll_GTComCon.csv (if you wish to use both mods).
•	MetadataDatabase -B-5.db – Adds all new star system coordinates and the 16 new systems.  Also adds in the JK_Variants-5-Everything.csv (if you wish to use both mods).  NOTE: Currently this is just a copy of the above, as the extra variants are not intended for Campaign mode.

 
7 - Restart the game.  You should immediately see the Star System coordinate changes for all systems in current game saves.  However, the new star systems only appear if you start a new campaign.  NOTE – there is a chance the when the game hits a map redrawn point, it may add these systems in.  Still playing a campaign to test if that occurs.

Alternatively - there is a file called " MetadataDatabase - Tag tab - Lines Added.csv", which outlines what was entered into the MetadataDatabase.db.  The entries only need to be added to the end of the TAB table.

:: RECOMMENDED MODS ::
- Want to add 'Mechs to the Campaign game?  There is a great mod from TheRealBMathis on Reddit and Nexusmods: https://www.reddit.com/r/BattleTechMods/comments/8hgd0z/metadatadabasedb_import_tool_testers_wanted/
https://www.nexusmods.com/battletech/mods/76

- Want more of a challenge?  Try out No Guts, No Galaxy!
https://www.nexusmods.com/battletech/mods/73

- Want to see where the GT Variants came from?  Try out the YAVM (note – this mod includes the Command Console and special rides from this mod)
https://www.nexusmods.com/battletech/mods/91

- Want a different take on adding these variants (and adding in some new ‘Mechs using the existing models)?
https://forum.paradoxplaza.com/forum/index.php?threads/mod-release-tetsuhara-heavy-industries-mod-thread.1087310/

- How about a compilation mod that really adds to the game (and already has JK_Variants integrated into it)?
https://forum.paradoxplaza.com/forum/index.php?threads/modpack-dz_consolidated_company_commander.1099514/#post-24267474

:: FIXED/ADDED ::
- 1.01 – Fixed some minor errors in the coordinates I typed in.
- 1.04 – added 6 more systems, bringing the total to 16 new star systems.
- 1.04 – Updated individual star system details on all 16 systems to make them more unique and interesting than the earlier generic versions.
- 1.04 – Corrected the spelling of Camadeierre system in the descriptions

::  KNOWN ISSUES ::
•	None

::  CREDITS ::
♦ Justin Kase (aka Justin Kase Too, Val_LS)
♦ Volt and the members of the Sarna Unified Cartography Society (http://www.sarna.net/wiki/BattleTechWiki:System_coordinates)
♦ Gruese and his work on the interactive atlas 
(https://forum.paradoxplaza.com/forum/index.php?threads/map-of-the-inner-sphere-3025-interactive-web-based.1075127/)
♦ Sarna in general, for being an awesome resource to point me to the right books about the various systems 
♦ Fasa, Catalyst Game Labs and HBS for making all of this possible over the years!
