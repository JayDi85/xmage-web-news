---
layout: post
author: JayDi85
title: Many new sets, tdfc, rooms, and ~1200 new cards
---
New release contains ~1200 new cards from old and new sets, rooms mechanic from Duskmourn, ticket mechanic from Unfinity, Prepared spells, transforming double faced cards, waterbend and much more. It also contains 300+ changes and fixes for old cards and abilities.

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## Other
* deck editor: fixed missing images, full arts, reorganized promo sets and reprints, boosters generation;
* deck editor: improved brackets calculations for x2 combos, removed tutors and improved game changers (#14003);
* deck editor: improved commander colors checking with detail info on wrong color (#14450);
* deck editor: updated bans list;
* AI: improved performance and server stability for big games with many permanents and targets (#9539, #14031, #14044);
* AI: fixed that it doesn't generate add target events in some use cases (#14918);
* GUI, app: improved small background image drawing (#14049);
* GUI, app: fixed wrong game error messages about unit tests;
* GUI, app: fixed error with miss tray icon in some linux systems like gnome (#14130);
* GUI, game: improved stack's hint with targets list (added player name and sorted by it);
* cheats: improved init.txt commands with me/opponent/ai params;

## Ability fixes
* Amass - improved and simplified UX for one target battlefields;
* Blights - fixed that it wrongly trigger for another player (example: Morcant, High Perfect, #14421, #14437);
* Blink/flicker - fixed that some ETB triggers doesn't work for suppressed permanents (example: Cloudblazer with Frogify, #9839, #14898);
* Can't be sacrificed - improved support with cost payment (example: Hithlain Rope, #14194);
* Can't block alone - improved support like Orcish Conscripts;
* Can't have counters - improved support with cost payment (example: Tatterkite, #14194);
* Cascade - fixed that it use card mana value instead spell mana value (example: Fireball with Quandrix, the Proof, #14693, #14687);
* Cast from hand conditional - fixed that it trigger for other players (example: Omniscience with Sen Triplets, #14813);
* Commander - added MDFc cards support as commander and commander damage calculation (#7530, #7637, #7699, #7773);
* Copy cards - fixed that bestow on the stack not resolving into a token;
* Copy cards - improved combo support with copies and move to exile zone (example: Mizzix's Mastery, #14005);
* Damage triggers - fixed duplicated triggers like Armadillo Cloak on Granger Guildmage (#14078);
* Delirium, non combat damage triggers - fixed that it doesn't trigger (example: Fear of Burning Alive, Chandra's Incinerator, #14429);
* Don't cause abilities to trigger - fixed that it doesn't prevent "one or more" events;
* Double faced cards - improved support and many bugs/combos fixed (#14061);
* Earthbend - fixed that it raise triggers for first target only (example: Dai Li Agents, #14426, #14436);
* Exile and return this abilities - improved support with aura cards (example: Estrid's Invocation, #14626, #14755);
* For each card type targets - fixed that human and AI were able to choose any cards amount (example: Atraxa, Grand Unifier, #13964);
* Mana abilities - improved ability activator support from 113.8 rules (example: Mana Cache, #14382, #14381);
* Manifest - fixed game error on manifesting a non-permanents with counters (#13683, #14619);
* Saga cards - improved ETB triggers support that doesn't work (example: Battle at the Helvault Saga, #13710, #11728);
* Soulbond - improved combo support, including paired creatures (#14542);

## Card fixes
* 300+ improvements and fixes for old and new cards;

## New cards
* Total new cards: 1218;
* Assassin's Creed:
  * Shaun & Rebecca, Agents
* Avatar: The Last Airbender - added 194 new cards;
* Avatar: The Last Airbender Eternal - added 87 new cards;
* Duskmourn: House of Horror:
  * Bottomless Pool // Locker Room
  * Central Elevator // Promising Stairs
  * Charred Foyer // Warped Space
  * Creeping Peeper
  * Dazzling Theater // Prop Room
  * Defiled Crypt // Cadaver Lab
  * Derelict Attic // Widow's Walk
  * Dollmaker's Shop // Porcelain Gallery
  * Funeral Room // Awakening Hall
  * Ghostly Keybearer
  * Glassworks // Shattered Yard
  * Grand Entryway // Elegant Rotunda
  * Greenhouse // Rickety Gazebo
  * Inquisitive Glimmer
  * Meat Locker // Drowned Diner
  * Mirror Room // Fractured Realm
  * Moldering Gym // Weight Room
  * Overgrown Zealot
  * Painter's Studio // Defaced Gallery
  * Rampaging Soulrager
  * Restricted Office // Lecture Hall
  * Roaring Furnace // Steaming Sauna
  * Say Its Name
  * Smoky Lounge // Misty Salon
  * Surgical Suite // Hospital Room
  * Ticket Booth // Tunnel of Hate
  * Underwater Tunnel // Slimy Aquarium
  * Unholy Annex // Ritual Chamber
  * Walk-In Closet // Forgotten Cellar
* Duskmourn: House of Horror Commander:
  * Cramped Vents // Access Maze
  * Experimental Lab // Staff Room
  * Polluted Cistern // Dim Oubliette
  * Secret Arcade // Dusty Parlor
  * Spiked Corridor // Torture Pit
* Fallout:
  * Aradesh, the Founder
  * Harold and Bob, First Numens
* Final Fantasy Commander:
  * Chaos Shrine's Black Crystal
  * Chocobo Camp
  * Edea, Possessed Sorceress
  * Fishing Gear
  * Garland, Royal Kidnapper
  * Judgment of Alexander
  * Mega Flare
  * Noctis, Heir Apparent
  * Rinoa, Angel Wing
  * Seifer, Balamb Rival
  * Squall, Gunblade Duelist
  * Vivi's Persistence
* Ice Age:
  * Arcum's Weathervane
  * Bone Shaman
* Lorwyn Eclipsed - added 241 new cards;
* Lorwyn Eclipsed Commander - added 21 new cards;
* Marvel Super Heroes - added 19 new cards;
* Marvel Super Heroes Commander - added 8 new cards;
* Masters Edition II:
  * Lava Burst
  * Orcish Conscripts
  * Orcish Farmer
  * Sacred Boon
  * Scars of the Veteran
* Modern Horizons 3 Commander:
  * Hourglass of the Lost
  * Sunken Palace
* Murders at Karlov Manor Commander:
  * Nelly Borca, Impulsive Accuser
  * Take the Bait
  * True Identity
  * Veiled Ascension
* Reality Fracture:
  * Chandra, Chill of Compliance
  * Stingcaster Mage
* Secret Lair Drop:
  * Jin Sakai, Ghost of Tsushima
  * Kratos, Stoic Father
  * Lucy MacLean, Positively Armed
  * Maximus, Knight Apparent
  * Nathan Drake, Treasure Hunter
  * The Ghoul, Gunslinger
* Secrets of Strixhaven - added 254 new cards;
* Secrets of Strixhaven Commander - added 63 new cards;
* Teenage Mutant Ninja Turtles - added 184 new cards;
* Teenage Mutant Ninja Turtles Eternal - added 66 new cards;
* The Lost Caverns of Ixalan Commander:
  * Paleontologist's Pick-Axe
* Unfinity:
  * Blorbian Buddy
  * Ticket Turbotubes
* Other sets:
  * Abomination, Irradiated Brute
  * Gleemox
  * Loki, God of Lies
  * M.O.D.O.K., Evil Intellect
  * Thanos, Death's Consort
  * The Ice Dancer
  * Ultron, Machine Overlord
  
Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)