---
layout: post
author: JayDi85
title: Reworked GUI, HiDPI support, new downloader, 400+ new cards and other
---
New release contains ~400 newly implemented cards from ACR, BLB, BLC, M3C, WHO and other sets. It also includes new mechanics like Pawprint, Freerunning, Offspring, Promise a gift, etc.

New version introduced many improves in GUI like new Preferences dialog, HiDPI monitors support, better sizeable settings, resizeable hand/stack zones and tons of other features. New images downloader works x10 faster now.

**Warning**, new version require to re-download mana symbols from main menu.

## New images downloader
* reworked images download from scryfall source;
* now it works x10 faster without threads or API limits (thanks to direct images downloader);
* added normal size option for scryfall (10 Gb, good quality, it's a default option now);
* fixed wrong errors on searching broken images files (#12430);
* fixed Star Wars images download, added Star Wars tokens (#12602, #10411);
* added missing reprints in Secret Lairs;

## New preferences, GUI size options and HiDPI monitors support
* reworked preferences dialog (removed some useless options, reorganized other, added new sizeable settings);
* added fast size settings and recommended option for your system (depends on screen resolution);
* added small screen support, no more hidden hand and scrolls - users can change any element of battlefield;
* added new option to control player panel size (#12455, #12451, #7563);
* added new option to control skip and phase buttons size (depends on dialogs font settings);
* improved fonts, menus and dialogs for better HiDPI support (not finished yet);
* improved runtime settings update (if you change themes, colors, sizes and other GUI settings then will see result immediately);
* fixed memory leaks and improved performance for long running app;
* fixed that that auto-target settings doesn't save;
* ![357654918-5acde595-70d8-42af-8cc2-205017dc08f9](https://github.com/user-attachments/assets/b50354db-aa42-438c-8681-7542dd9a73f8)

## New resizeable hand/stack zones
* users can resize or hide hand/stack zones on battlefield now;
* resize it by mouse drag;
* hide/minimize zone by mouse clicks on splitter's arrows;
* selected size will be saved and used for all new or active games (even after app restart or reconnect);
* fixed wrong position of card panel and chats on new game;
* ![357404692-79e1b20c-2f0c-4254-9859-6403138cd006](https://github.com/user-attachments/assets/be4b3259-54ce-4008-a5cf-18240557caed)

## New switch panels menu
* reworked switch panels from main menu;
* added grouping (all games, watching and other panels from one table/tourney will be stored in one group);
* added sorting (latest tables will be added to the end);
* fixed random positions on each opening;
* ![shot_240811_191942](https://github.com/user-attachments/assets/98221f85-79f0-472e-9c8c-31742a46eb61)

## New error dialog
* reworked error dialog with additional information and options;
* added client version and improved stack trace info;
* added option for text copy;
* added option for fast bug create on project's github (new issue will be created with prefilled data);

## New choose alternative cost dialog
* Improved support for multiple alternative costs, now user can choose from multiple options (example: Prying Prayers, #12420)
* Added new choose dialog with card hint and other additional information
* ![shot_240816_161619](https://github.com/user-attachments/assets/0bc26b65-7a89-4fcf-9059-b2cf567610ac)

## GUI dialogs improves and fixes
* app: returned build-in "what's new" page with release notes and other useful information;
* game: added storm counter card hint (available in all games by hints button in player panel, #12360);
* game: improved choose replacement effect dialog - added card hints;
* game: improved choose creature type dialog - important creature types added to the start of the list and marked as my/opponent (#8478):
* ![shot_240816_184226](https://github.com/user-attachments/assets/2724506b-b3bc-4802-aef0-c750b96d0b7a)
* game: improved pick card/trigger dialog - cards list sorted by name now (#11874);
* game: improved spell choose dialog with mana symbols and card hints support (#12155):
* ![shot_240816_185510](https://github.com/user-attachments/assets/5524cfcd-86cc-4a64-b6b4-427be5728db2)
* lobby: fixed that server's lobby do not remember divider position after app restart (tables, matches and chat sizes);
* game: fixed wrong logs formatting on multiple targets;
* game: fixed that pick choice dialog can freeze on search text deleting (#8671);
* game: fixed slow opening and searching on big lists like card names in pick choice dialogs (#8671);
* game: added zone info for played spell logs (#12632);

## Improved server stability and fixes
* Fixed game freeze on rollback usage for some use cases;
* Fixed game freeze on concede usage for some use cases (#11285, #11460);
* Fixed server app freeze on another instance already running, e.g. on app update;
* Fixed game errors in big/late games for some use cases (#11285);
* Fixed broken database in some use cases (example: AI and choose name dialog, #11285);
* Added logs and stats with a max users online;
* Fixed wrong cheating detection in some tourney sideboardings (#11877);

## Other fixes
* game: updated oracle texts, bans list and Canadian Highlander points (#12557);
* game: added MH3 play booster (#12400);
* app: improved app stability in macOS for some configurations (#12261);
* app: fixed app run scripts in client/server folders;
* app: added 22 commander decks to sample folder (#12498)
* cards: introduced not finished cards from [CNS] and [CN2] without draft-matters effects (such effects aren't supported, but cards are required for popular cubes/drafts, example: Agent of Acquisitions, #12473);
* AI: fixed game error on AI targeting activated ability on stack (example: Hope Tender, #12437);

## Abilities fixes
* Becomes the target - improved combo support with multi-mode spells (example: Kira, Great Glass-Spinner, #12452, #11539, #12439, #12227);
* Can't be activated effects - fixed that some restricted effects show abilities as playable (example: Sharkey, Tyrant of the Shire and Karakas, #10642);
* Choose by multiple players - fixed that game ask players in random order instead APNAP in some use cases (#12532);
* Commander colors - fixed wrong colors with 2+ color identity (#12429, #7983, #9852);
* Copy effects - fixed that copy effect not being discarded early enough (example: Shifting Woodland in graveyard, #12433);
* Die triggers - fixed that sacrificed creatures don't trigger their own die trigger (#12195, #12385, #9688, #8481, #10610);
* Evidence abilities - added improved card hint with available evidence to collect;
* Extort - fixed a bug where removing the source of the Extort trigger fizzles the trigger (#12609);
* Look at effect - fixed that looking at a face-down creature with any effect open an empty window instead of actually revealing the card (#12479);
* Revolt - added card hints;
* Sacrifice - improved combo support with control changing effects (example: Evoke's sacrifice after control changed, #12582);
* You gained or lost life - added card hints;

## Cards fixes
* Aclazotz, Deepest Betrayal // Temple of the Dead - added card hint for second side;
* Aether Revolt - added card hint;
* Apex Observatory - improved combo support with double-faced cards;
* Arcane Bombardment - added spell order choose (#12454);
* Devourer of Destiny - fixed that it exiling too early (#12636);
* Echoes of Eternity - fixed double triggers (#12419);
* Enduring Tenacity - fixed not working return ability (#12594);
* Faith's Fetters - fixed combo support with Leaden Myr (#12463);
* Havengul Laboratory // Havengul Mystery - fixed that it doesn't trigger on transform (#12477);
* Hero of Bretagard - fixed that it triggers when a creature is exiled by an opponent's Crib Swap (#12579);
* Hired Claw - added card hint;
* Howltooth Hollow - added card hint;
* Indomitable Might - fixed that it triggering for all creatures (#12530);
* Induced Amnesia - fixed that it doesn't return exiled cards to owner's hand (#12486);
* It That Heralds the End - fixed that cost reduces ability benefits opponent (#12503);
* Jace, Telepath Unbound - improved combo support -3 ability with split and mdf cards (#9607, #9365);
* Life of the Party - added card hint;
* Maarika, Brutal Gladiator - fixed that trigger doesn't cause opponent to sacrifice anything (#8775, #12507);
* Marneus Calgar - fixed that it missing draws in some use cases with multiple players (#12588);
* Mystic Reflection - fixed that it not working with planeswalkers;
* Omo, Queen of Vesuva - fixed that it interacting incorrectly with creature lands (#12558);
* Orcish Lumberjack - improved and simplified mana dialogs (#12575);
* Rakdos Joins Up - fixed that it wrongly counting tokens as legendary (#12574);
* Saheeli the Gifted - added card hint;
* Sardian Avenger - added card hint;
* Sorcerous Squall - fixed miss "up to" part (#12519);
* Spelleater Wolverine - added card hint;
* The War in Heaven - fixed that it doesn't return anything with its III effect (#12412);
* Unstable Amulet - improved combo support with split/mdf/adventure cards;
* Vaultborn Tyrant - fixed that it only triggering once with Flash (#12449);

## New cards
* Assassin's Creed - added 66 new cards;
* Bloomburrow - added 226 new cards;
* Bloomburrow Commander - added 24 new cards;
* Alchemy: Dominaria:
  * Marwyn's Kindred
  * Oracle of the Alpha
  * Wandering Treefolk
* Alchemy: Innistrad:
  * Sanguine Brushstroke
  * Toralf's Disciple
* Arena Tutorial Cards:
  * Blinding Radiance
  * Goblin Bruiser
  * Ogre Painbringer
  * Titanic Pelagosaur
  * Treetop Recluse
* Conspiracy: Take the Crown:
  * Archdemon of Paliano
  * Illusionary Informant
  * Leovold's Operative
* Doctor Who:
  * Confession Dial
  * Last Night Together
  * Nanogene Conversion
  * Return the Past
  * The Rani
  * Time Reaper
  * Vrestin, Menoptra Leader
* Duskmourn: House of Horror:
  * Chainsaw
  * Cursed Recording
  * Doomsday Excruciator
  * Enduring Tenacity
  * Fear of Missing Out
  * Leyline of Hope
  * Screaming Nemesis
  * The Wandering Rescuer
  * Toby, Beastie Befriender
* Fallout:
  * Desdemona, Freedom's Edge
  * Diamond City
  * Idolized
  * Paladin Elizabeth Taggerdy
  * Rampaging Yao Guai
  * Rose, Cutthroat Raider
  * Synth Infiltrator
  * Vault 87: Forced Evolution
  * Wild Wasteland
* Foundations:
  * Anthem of Champions
* Lost Caverns of Ixalan Commander:
  * Apex Observatory
  * Eye of Ojer Taq
* Magic: The Gathering-Conspiracy:
  * Agent of Acquisitions
  * Cogwork Librarian
  * Cogwork Spy
  * Lore Seeker
  * Whispergear Sneak
* Modern Horizons 3:
  * Abstruse Appropriation
  * Arena of Glory
  * Herigast, Erupting Nullkite
  * Primal Prayers
  * Thief of Existence
* Modern Horizons 3 Commander:
  * Aether Refinery
  * Aggressive Biomancy
  * Aurora Shifter
  * Benthic Anomaly
  * Bismuth Mindrender
  * Coram, the Undertaker
  * Eldrazi Confluence
  * Filigree Racer
  * Gluttonous Hellkite
  * Infested Thrinax
  * Inversion Behemoth
  * Mutated Cultist
  * Omo, Queen of Vesuva
  * Planar Nexus
  * Polygoyf
  * Razorfield Ripper
  * Sage of the Maze
  * Sawhorn Nemesis
  * Selective Obliteration
  * Silverquill Lecturer
  * Sphinx of the Revelation
  * Twins of Discord
  * Ulalek, Fused Atrocity
* Murders at Karlov Manor:
  * Deadly Cover-Up
  * Etrata, Deadly Fugitive
  * Expose the Culprit
  * Hide in Plain Sight
  * Lumbering Laundry
  * Vannifar, Evolved Enigma
* Murders at Karlov Manor Commander:
  * Marvo, Deep Operative
* Mystery Booster 2:
  * Rusko, Clockmaker
* Ravnica: Clue Edition:
  * Apothecary White
  * Emissary Green
* Sega Dreamcast Cards:
  * Velukan Dragon
* Unfinity:
  * Nearby Planet
* Visions:
  * Pygmy Hippo
* New Capenna Commander:
  * Henzie "Toolbox" Torre

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](http://xmage.today/#donate).