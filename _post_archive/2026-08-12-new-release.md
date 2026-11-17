---
layout: post
author: JayDi85
title: Improved AI, images, and ~400 new cards from Marvel, Star Trek and Hobbit
---
New release contains improved AI with modal spells support, scryfall images download fix, and many hot-fixes for some newly added cards. Also it includes 377 new cards from MSH, MSC, TRK, TRC, HOB, HOC and others.

🛠️ If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

😍 If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## Improved AI
- added support of multi-modal abilities (computer can simulate and
activate ability with multiple modes);
- added support of multi-modal abilities with paw prints budget (cards from Bloomburrow);
- added support of multi-modal abilities with "may choose same mode
more than once";
- fixed that computer was able to activate bad options on modal
abilities (due wrong usage of game sims);

## Other
* images: fixed images download from scryfall source (#15744);
* images: added new reprints and promo sets;
* game: updated banned and restricted for Standard, Legacy, and Vintage per August 10, 2026 announcement;
* game: added max modes selection limit to 5 due performance optimization (can be increased in next releases);
* app: improved compatibility with bad or outdated launchers (can't connect to local server, can't download some images, etc);
* app: improved performance, improved startup time for client and server apps;
* deck editor: fixed broken/empty deck on too fast sideboarding e.g. instant loose (#11877);
* deck editor: added deck file overwrite confirm on save;
* deck editor: now it use deck name as file name on save by default (#12813);
* deck editor: improved stability while selection decks and sets (#15871, #15623);
* deck editor: added commander decks for new sets, see launcher/xmage/mage-client/sample-decks (#15646);
* server: fixed miss game mode Custom Pillar of the Paruns (#10633);
* server: improved library names, fixed typos in config, added more config checks on startup;
* server: WARNING for public servers, if you keep configs between updates then make sure it uses actual jar names (take it from fresh install's config.xml);

## Abilities fixes
* Ability counters - fixed that it doesn't stacked to multiple instances (example: exalted counter);
* Choose left or right - added card hints with left-right players info (#15848);
* City's blessing - improved card hint with detail conditional and stats (#15677);
* Copy abilities - fixed that "if it was cast" triggers doesn't work for copied cards (example: Baron Helmut Zemo with Shard of the Nightbringer, #15240);
* Don't cause abilities to trigger - fixed miss restriction for "one or more" triggers (example: Torpor Orb with Moonshadow, #15681);
* Infinity Stones - added card hints for harnessed status of the stones (#15738);
* Mutate tokens - improved compatibility with some triggers, fixed max tokens limit (#14980);
* Warp ability - improved combo support with phased out permanents (#15595, #15612);

## Cards fixes
* Baron Helmut Zemo - fixed that it was able to cast cards from previous boast (#15240);
* Cold-Blooded Crew - fixed wrong trigger;
* Evendo Brushrazer - fixed game error on usage (#15621);
* Fall of Gil-galad - fixed wrongly required target in "fights up to one" effect;
* Garland, Royal Kidnapper - fixed that it doesn't give can't sacrifice ability (#15911, #15915);
* Gisa's Favorite Shovel - fixed game error on some use cases (on leave player or game draw);
* Haktos the Unscarred - fixed that it gives protection from chosen mana value too;
* Human Torch - fixed game error on usage;
* Invisible Woman - added card hint;
* Jennifer Walters - fixed that back side was missing can't cast effect (#15795);
* Kinscaer Sentry - fixed that it should only let you put Creature cards onto the battlefield (#15917);
* Nashi, Moon Sage's Scion - fixed useless popup exile window after usage;
* Ratchet, Field Medic - added card hint with life gained info;
* Restless Bloodseeker - fixed game error on usage;
* Talion, the Kindly Lord - fixed not working trigger for the chosen mana value (#14073, #14158);

## New cards
* Total new cards: 377;
* Marvel Super Heroes - added 34 new cards;
* Marvel Super Heroes Commander - added 65 new cards;
* Star Trek - added 49 new cards;
* Star Trek Commander - added 34 new cards;
* The Hobbit - added 142 new cards;
* The Hobbit Eternal - added 21 new cards;
* Marvel's Spider-Man:
  * SP//dr, Piloted by Peni
* Mystery Booster Commander Edition:
  * Arzakon
  * Autumn Willow, Harmony
  * Balefang the Unslayable
  * Blor the Impervious
  * Boss Uramon, Shadow's Reach
  * Davvol, Evincar of Rath
  * Dyfed, the Guiding Hand
  * Emerald Collector
  * Istvan, Butcher of Eln
  * Joven and Chandler
  * Ruby Collector
  * Tsagan, Raider Warlord
* Reality Fracture:
  * Ajani Resolute
  * Ajani Unrelenting
  * Craterclaw Colossus
  * Garruk, Curse Breaker
  * Garruk, Veiled Butcher
  * Liliana the Faultless
  * Liliana the Repentant
  * Paradox Shaper
  * Prudent Fateseer
  * Stingerquill Voxmancer
  * The Theorist, Jace Beleren
  * Tinybones, Pocket Nuisance
  * Titanbones, Towering Heart
  * Vigorbloom Vanguard
  * Woodwork Prodigy
* Reality Fracture Commander:
  * Darksteel Angel
* 2021 Heroes of the Realm:
  * Arteeoh, Dread Scavenger
* Secret Lair Drop:
  * Stardew Valley
  
Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)