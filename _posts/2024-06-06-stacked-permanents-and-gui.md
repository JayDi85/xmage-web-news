---
layout: post
author: JayDi85
title: Stacked permanents, improved downloader, GUI fixes and 700 new cards
---
New release contains ~300 newly implemented cards and ~400 reprints from MH3, M3C, PIP, WHO, MKM and other sets. It also includes new mechanics like colorless hybrid mana, radiation, cloak and other.
Also, it introduces new GUI features like stacked permanents and many GUI related fixes.

Stacked creatures and tokens
* Now all creatures and tokens stacked by x5 cards like lands;
* Only same permanents will be stacked (with same name, PT, abilities and other);
* ![shot_240606_210530](https://github.com/magefree/mage/assets/8344157/de0d5045-bf78-41e7-96c5-ecc78d74e9f3)

Improved images download
* added filter to download basic lands only;
* added new source for memory optimized images (scryfall's small images);
  * small images require x10 less disk space, network and memory usage (1.5 GB instead 15 GB);
  * it's look good in small screens and MTGO render mode (see main menu - images - render mode);
  * if you use image render mode or 4K monitor then use big images source as before;
  * use "re-download" checkbox to download new images for old set;
  * ![shot_240606_213751](https://github.com/magefree/mage/assets/8344157/816847b8-b020-435e-870f-be8f9f0ad548)
* added tokens download for many new sets;
* fixed images download for some special cards (#11926);

GUI fixes
* battlefield: improved auto-answers support (right click menu) for some choose dialogs like Rhystic Study (#12088);
* battlefield: fixed wrong rendering of designation icons over avatar (#12169);
* battlefield: fixed that attack/block arrows was visible after disconnect (#12258);
* battlefield: fixed wrong render of attack and other arrows over dialogs (#12261);
* deck editor: improved support of mtgjson decks (added import of commander decks, see https://mtgjson.com/downloads/all-decks/ );
* cards: improved rendering of some double-faced cards like Jace, Vryn's Prodigy (#12134);
* cards: fixed miss token image in some use cases (if it was created from a card and a set contains multiple images);
* cards: fixed wrong background rendering of card's popup window (#12261);
* other: fixed that size settings changes do not work in-game sometimes (broken fonts in feedback panel);
* other: fixed wrong font sizes in table's and feedback panel popup hints;

Improved server stability
* improved game stability on player's concede (#11460);
* added max tourneys limit on server (max games / 5);
* fixed that rollback requests do nothing in some use cases (related to #11285);
* fixed server crashes on usage of multiple permanents with {Any} mana abilities (example: Energy Refractor, #11285);

Other fixes
* AI: fixed game freezes and errors on computer's {Any} mana usage (#9467, #6419);
* game: updated banned cards (#12136);
* game: improved Mystery Booster generation (#12138);
* launcher: updated client/server run scripts from "mage" folder with actual recommended settings;

Ability fixes
* Modal double-faced cards - fixed game error on usage with some replacement effects (example: Diluvian Primordial, #12176, #12184);
* Modal double-faced cards - improved support with copy effects (fixed that copied token has abilities from both sides, #10146, #8476);
* Triggers for damage, life, milled and other - fixed too much triggers raise in some use cases with multiple source events at the same time;
* Phantom cards - improved counter remove on multiple damage (example: Phantom Wurm, #12179);
* Gain abilities - improved combo support with Evoke, Dash and Prowl (example: Hunting Velociraptor, fixed #11714, #12237)

Card fixes
* Annie Joins Up - fixed missing creature check in second trigger (#12199);
* Anthem Dying - fixed that first strike phase sesulting in double strike (#10232);
* Azra Oddsmaker - fixed that chosen creature is not indicated to opponent (#12352);
* Blood Baron of Vizkopa - fixed that it only checks one opponent (#12204);
* Calamity, Galloping Inferno - fixed that it not creating tokens on attack (#12175);
* Case the Joint - fixed that it doesn't look at other players library (#12151);
* Chromatic Star - fixed wrong combo with Serra Paragon (#12330);
* Danse Macabre - fixed wrong usage (#12247);
* Disciple of Caelus Nin - fixed that it doesn't ask other players to keep permanents #12151);
* Dragon Cultist - fixed wrong damage count (#12149);
* Fight or Flight, Do or Die - fixed that it separates all creatures instead of just the active player's (#12245);
* Force Drain - fixed card type (#12306);
* Hollow Marauder - fixed that it making it's owner discard cards instead of the target opponents (#12254);
* Kess, Dissident Mage - improved support with adventure cards (#11924);
* Krark's Thumb - fixed that it can generates too many flip triggers (#12152);
* Leafkin Avenger - fixed that it count opponent creatures, added card hint (#12146);
* Legate Lanius, Caesar's Ace - fixed wrong counting creatures (#12183);
* Lidless Gaze - fixed that it not letting the user cast the exiled cards until the end of his next turn (#12305);
* Molten Disaster - fixed that kicker did not have split second (#12290);
* Niv-Mizzet, Guildpact - fixed that it doesn't gain life on both damage (#12329);
* Obeka, Splitter of Seconds - fixed wrong extra phase;
* The Master, Trasncendent - improved combo with other effects;
* Topography Tracker - fixed game error on some use cases;
* Transmutation Font - fixed game error on usage;
* Trespasser's Curse - fixed game error on some use cases;
* Urborg Scavengers - fixed that it not getting keywords when exiling cards (#10409, #12180);
* Wake Thrasher - fixed game error on some use cases;
* Xanathar, Guild Kingpin - fixed that it does not allow lands to be played from opponent's deck (#12133);
* Zirda, the Dawnwaker - fixed wrong companion legality (#11346);

New cards and reprints
* [MH3] Modern Horizons 3: added 242 new cards;
* [M3C] Modern Horizons 3 Commander: added 27 new cards;
* [PIP] Fallout: added 34 new cards;
* [YDMU] Alchemy: Dominaria
  * Slimefoot, Thallid Transplant
  * Vinesoul Spider
* [MAT] March of the Machine: The Aftermath
  * Deification
* [ACR] Assassin's Creed
  * Cleopatra, Exiled Pharaoh
* [OTC] Outlaws of Thunder Junction Commander
  * Felix Five-Boots
* [WHO] Doctor Who
  * Flesh Duplicate
  * Trenzalore Clocktower
  * Weeping Angel
* [MKM] Murders at Karlov Manor
  * Coveted Falcon
  * Cryptic Coat
* [REX] Jurassic World Collection
  * Grim Giganotosaurus
  * Ian Malcolm, Chaotician
  * Indominus Rex, Alpha
  * Indoraptor, the Perfect Hybrid
* [BOT] Transformers
  * Slicer, High-Speed Antagonist
  * Slicer, Hired Muscle
* And hundreds of reprints in different sets

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).