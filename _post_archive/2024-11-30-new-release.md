---
layout: post
author: JayDi85
title: Foundations and 221 new cards
---
New release contains 221 new cards, most from Foundations, but also includes new cards from DFT, DSK, DSC, MKC and other. 
New real life booster generations for old sets and improved target auto-choice by GUI. And of course it has many fixes for 
abilities and cards.

## Improved booster generation
Added [real life booster collation and runs](https://www.lethe.xyz/mtg/collation/) in old and new sets instead generic rarity distribution:
* APC, DMR, EXO, INV, JUD, LCI;
* LRW, MOM, NPH, ODY, ONE, ONS;
* SHM, TMP, TOR, ULG, USG, VIS;

## GUI improves and fixes
* game: improved auto-choose logic for single targets, added more compatible use cases, e.g. auto-choose target opponent in duel game (#13036, #12466, #12784);
* game: added default card hint to see day/night and next turn transform conditions (use player panel to see that hints #8414);
* game: added card popup support in choose target amount dialogs (example: damage distribution, #9827);
* game: fixed black background instead card hint popup on some java versions (#12857);
* table: improved save/load config for new table dialog (miss player types, AI skill level and deck files params, #12981);
* table: improved save/load config for new tourney dialog (miss num seats, decks, skill, player types and other params, #12981);
* other: added new error dialog for more use cases;
* other: improved text color in dark theme for better readability (#12873);
* preferences: removed outdated settings with images download threads (it's 5 by default now);

## Other fixes
* game: updated rules for first/second main phases (#12788);
* game: updated bans list like Tamiyo, Inquisitive Student from commander (#12948);
* game: added reprints to Wilds of Eldraine Commander;
* images: fixed very slow download finish in some use cases;
* server: improved stability, improved disconnection logs, fixed some race conditional bugs and freezes;

## Ability fixes
* Whenever, Whenever one or more - improved combo support with multiple events at the same time, now it will generate one or multiple triggers due card rules (example: Exquisite Blood, #13057, #10805);
* Leaves-the-battlefield triggers - improved combo support with sacrifice cost, mass removal and other actions with source remove (no trigger bugs, #13088);
* If xxx triggers, that ability triggers an additional time - fixed that it doesn't work on blink/remove (example: Harmonic Prodigy, Annie Joins Up, Clara Oswald, Echoes of Eternity);
* Hideaway - improved combo support with multiple/copied hideaway effects (#13009);
* Recover abilities - fixed that it doesn't ask to pay a cost on multiple triggers;

## Card fixes
* Diresight - fixed wrong draw amount;
* Enduring Courage - fixed miss boost effect (#12937);
* Enduring xxx - fixed that it return card under wrong player (example: Enduring Courage);
* Erestor of the Council - fixed that it wasn't drawing a card;
* Florian, Voldaren Scion - added card hint;
* Keen-Eyed Curator - fixed not working boost effect (#13022);
* Landscaper Colos - fixed that it able to use own graveyard;
* Legion's Initiative - fixed that it is not working and left your creatures in exile for ever (#12900);
* Mage Hunter's Onslaught - fixed that it doesn't work in some use cases;
* Marchesa, Resolute Monarch - fixed that it trigger on wrong damage (#12994);
* Master of the Wild Hunt - reworked to use single damage dialog instead multiple calls, added card hints (#9827);
* Popular Entertainer - fixed that it doesn't trigger on damage (#13060);
* Tatsunari, Toad Rider - fixed that ability doesn't allow reach creatures to block (#13059);
* The Mindskinner - fixed that it doesn't mill, fixed wrong damage prevent (#12928);
* The Raven's Warning - fixed wrong targeting on trigger;
* Verrak, Warped Sengir - improved combo support with phyrexian style effects like K'rrik, Son of Yawgmoth (#10119);
* Wick's Patrol - fixed wrong targeting on trigger;
* Zimone, Mystery Unraveler - improved targeting;

## New cards
* Foundations - added 126 new cards;
* Foundations Jumpstart - added 52 new cards:
* Aetherdrift:
  * Brightglass Gearhulk
  * Daretti, Rocketeer Engineer
  * Earthrumbler
* Assassin's Creed:
  * Become Anonymous
  * Ezio Auditore da Firenze
* Bloomburrow:
  * Dragonhawk, Fate's Tempest
  * Festival of Embers
  * Jackdaw Savior
  * The Infamous Cruelclaw
* Duskmourn: House of Horror:
  * Fear of Abduction
  * Ghost Vacuum
  * Grab the Prize
  * Irreverent Gremlin
  * Leyline of Transformation
  * Meathook Massacre II
  * Niko, Light of Hope
  * Omnivorous Flytrap
  * The Rollercrusher Ride
  * Unstoppable Slasher
* Duskmourn: House of Horror Commander:
  * Curator Beastie
  * Formless Genesis
  * Giggling Skitterspike
  * Glitch Interpreter
  * Redress Fate
  * Seance Board
  * Shriekwood Devourer
  * The Lord of Pain
  * Valgavoth, Harrower of Souls
  * Zimone, Mystery Unraveler
* Fallout:
  * Grim Reaper's Sprint
  * Overencumbered
* Murders at Karlov Manor Commander:
  * Boltbender
  * Havoc Eater
  * Hot Pursuit
  * Ransom Note
* Mystery Booster 2:
  * Stone Drake
* Wilds of Eldraine Commander:
  * Tegwyll's Scouring
* Secret Lair Drop:
  * Black Panther, Wakandan King
  * Captain America, First Avenger
  * Iron Man, Titan of Innovation
  * Storm, Force of Nature
  * Wolverine, Best There Is
* Unknown Event:
  * More of That Strange Oil

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).