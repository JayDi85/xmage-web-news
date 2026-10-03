---
layout: post
author: JayDi85
title: Welcome to Async World with reworked and fast network, 421 new cards, prepared and rulebreakes
---
One of the most important updates in recent years 💪 With the reworked network and client-server logic, XMage now works in a truly async mode. No more dependence on slow or fast connections, no more laggy opponents ruining the game. Players from every corner of the earth are welcome 🤜🤛

New release contains network rework for faster and stable games and drafts, 421 new cards from FRA and other new and old sets including 46 cards with prepared mechanics and 3 cards with rulebreakers. It also contains over 100 fixes in existing cards and abilities.

<img width="640" height="320" alt="Image" src="https://github.com/user-attachments/assets/14add491-f33f-459f-a417-a67fe7516e77" />

🛠️ If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

😍 If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## Async world and network reworked

What it does for players:
* over 40 problems were found and fixed with disconnects, errors, race conditions, concurrent data modifications, missed or outdated data, freezes and other errors that players randomly catch  every day;
* many memory and connection leaks were fixed too, so public servers are much more stable now;
* **more stable drafts, tourneys and matches**;
* **faster games and faster responses to player actions**;
* fast server connect/reconnect and fast chat messages;
* safe watching of other players' games;
* fast and stable AI vs AI game watching;
* for laggy players: no more missed game dialogs or updates — all important data comes with high priority;
* for laggy players: server-side data optimization (you get only actual data, outdated data is dropped before sending);
* for fast players: no more dependence on laggy players — if you play fast, you get fast responses to your actions;
* [more details here](https://github.com/magefree/mage/pull/16434);


## Rulebreakers
Implemented special rulebreakers that allow to pass some deck validation rules:
* no maximum deck size by Whtz the Bibliophile;
* additional cards by Seluma, Light of Aysen;
* additional colors by Tolabow, Loch Rascal;

## Other
* GUI, game: fixed wrong card images in hand and other zones after stack in MTGO render mode (#16369);
* GUI, game: added counters puts/removes logs for any actions (#9440, #9528);
* GUI, game: fixed log spam when player can't lose and has <=0 life (#16300);
* GUI, card viewer: improved by giving users an actual toggle between Cards vs Tokens (#16332);
* deck: added multiple reprints and alchemy sets;
* deck: updated Canadian Highlander points (#16038, #16078);
* deck: updated Duel Commander banlist;
* deck: updated Pauper banned list (#16097);
* images: fixed missing Undercity dungeon (#16088);
* images: fixed missing set symbols;
* images: fixed missing cards in many old sets;

## Abilities fixes
* Copy abilities - fixed duplicated effects and triggers in some cards with copy (example: Urza's Saga with Echoing Deeps, #12475, #16256);
* Duel Commander - now only one commander can be cast from the command zone per game (#16091);
* Equip abilities - improved compatibility with restrictions on first equip (example: O-Naginata, #15970);
* Exile top of library, may play - improved exile dialogs;
* Replicate abilities - improved combo support with triggers and copies (example: Isochron Scepter copies, #13998, #13758, #16106);
* Whenever you gain life - added card hints on stack with gained life amount (#16364);

## Cards fixes
* Absorbing Man - fixed copy effect (#15986);
* Ace, Fearless Rebel - fixed that fight target isn't optional;
* Armored Kincaller - fixed that it counts Dinosaurs you don't control;
* Balancing Act - fixed that players don't sacrifice/discard anything when a player controls no permanents or has no cards in hand (#16361);
* Behold the Sinister Six! - fixed that it can return non-creature permanent cards;
* Bloodchief Ascension - added card hint;
* Boiling Rock Rioter - fixed that it allows to cast exiled Ally spell without paying its mana cost;
* Bone Devourer - fixed that it counts all counters instead +1/+1 counters only;
* Breaching Dragonstorm - fixed that it puts exiled cards on the bottom of library;
* Burden of Proof - fixed that it doesn't give +2/+2 to Detective you control when enchanting it;
* Caught in the Crossfire - fixed that first mode doesn't deal damage and second mode deals damage to all creatures;
* Clive, Ifrit's Dominant - fixed that Ifrit can fight itself;
* Combat Tutorial - fixed that it can put +1/+1 counter on opponent's creature;
* Commander Liara Portyr - fixed that it reduces cost of opponent's spells and abilities;
* Cosima, God of the Voyage - fixed wrong usage by AI;
* Covetous Elegy - fixed wrong implementation (#16057);
* Crescent Island Temple - fixed that it doesn't count itself on enter and triggers on own enter;
* Dawnhand Dissident - fixed wrong targeting (#16020, #16089);
* Deepway Navigator - fixed that it doesn't boost itself;
* Defend the Rider - fixed that it can target permanent you don't control;
* Denry Klin - fixed that it puts too many counters on himself when entering the battlefield (#9779);
* Distant Melody - fixed game error on miss choice (#14392, #16072);
* Dose of Dawnglow - fixed that blight only applied in opponent main phase instead any (#16047);
* Dragon's Fire - fixed game error on no valid choices;
* Elephant-Mandrill - fixed that it counts artifacts owned by opponents instead controlled;
* Emeritus of Ideation - improved exile cost window;
* Fang, Roku's Companion - fixed that it can target non-legendary creature, fixed that it returns tapped and under owner's control;
* Far Fortune, End Boss - fixed not working max speed ability;
* Firion, Wild Rose Warrior - fixed that token copies are sacrificed at the next end step instead next upkeep;
* Flamechain Mauler - fixed that menace should last until end of turn (#16197);
* Focus Fire - fixed wrong damage amount, must be 2 plus creatures and Spacecraft count;
* Foggy Swamp Visions - fixed wrong targets amount, must be X targets;
* Gaea's Will - fixed that it not exiling spells you play (#16336, #16346);
* Glister Bairn - fixed that it can target itself;
* Hare Apparent - fixed that it counts non-creature permanents;
* Hauntwoods Shrieker - fixed wrong usage by AI;
* Ignis Scientia - fixed that it making treasure instead of food;
* Inventory Management - fixed that it doesn't attach Auras and Equipment;
* Kindred Dominance - fixed game error on miss choice (#14392, #16072);
* Krang, the All-Powerful - fixed that it lookup for draw instead drew event (#16027, #15962);
* Kratos, Stoic Father - fixed that it doesn't trigger on opponent's Gods dies;
* Kraven's Last Hunt - fixed that chapter I mills 4 cards instead 5;
* Leonardo, Sewer Samurai - fixed that it allows to cast from graveyard during opponent's turn;
* Lucy MacLean, Positively Armed - fixed wrong condition (#16042);
* Madame Null, Power Broker - fixed that it is creating extra +1/+1 counters for no life cost (#15175);
* Metamorphic Blast - fixed that target creature loses its abilities;
* Midnight Crusader Shuttle - fixed wrong second choice dialog;
* Mirrormind Crown - fixed that it works during your turn only;
* Mogis, God of Slaughter - fixed wrong sacrifice cost;
* Momo, Friendly Flier - fixed that it reduces cost of non-creature spells, fixed that it triggers on itself;
* Mondo Gecko - fixed that hexproof from chosen color doesn't end at the end of turn;
* Morningtide's Light - fixed that it returns creatures untapped instead tapped;
* Mysterio, Master of Illusion - fixed that it doesn't exile Illusion tokens on leave;
* O'aka, Traveling Merchant - improved highlight when ability cost payable (a controlled nonland permanent has a counter);
* Oracle of the Alpha - fixed miss Mox Sapphire in conjured Power Nine;
* Pain's Reward - fixed game freeze with AI games;
* Prehistoric Turtlesaurus - fixed that it counts non-creature permanents with +1/+1 counters;
* Price of Freedom - fixed that it can target permanents owned by opponents instead controlled;
* Rampaging Classmate - fixed that it counts itself as other attacking creature;
* Resonance Technician - fixed that it can copy opponent's spells;
* Ride's End - fixed that cost reduction works only with tapped creatures instead any tapped permanent;
* Rinoa, Angel Wing - fixed that it not tapping the creature;
* Roadside Blowout - fixed that cost reduction works only with creatures instead any permanent;
* Robot token - fixed miss Warrior subtype;
* Sail into the West - fixed that it should exile itself if "Return" wins vote (#16092);
* Salvation Colossus - fixed that it gives indestructible to itself;
* Scorpion Sentinel - fixed that it requires eight lands instead seven;
* Serah Farron - fixed that it can transform with only one other legendary creature;
* Sidequest: Play Blitzball - fixed that it doesn't attach to a creature after transform;
* Sold Out - fixed that it checks current damage instead damage dealt this turn;
* Sothera, the Supervoid - fixed;


## New cards
* Total new cards: 421;
* Reality Fracture - added 234 new cards;
* Secrets of Strixhaven - added 36 new cards (prepared);
* Secrets of Strixhaven Commander - added 10 new cards (prepared);
* Reality Fracture Commander:
  * Avacyn, Angel of Horror
  * Ginger, Queen of Sweets
  * Memnarch, the Warden
  * Nissa, Leyline Tamer
  * Niv-Mizzet, Ghost Counsel
  * Ob Nixilis, the Ascended
  * Omnath, Locus of the Void
  * Turbulent Crater
  * Turbulent Shore
  * Turbulent Wetlands
* Alchemy: Murders at Karlov Manor:
  * Emmara, Voice of the Conclave
  * Emporium Thopterist
* Alchemy: Wilds of Eldraine:
  * First Little Pig
  * Victory of the Pyrohammer
* Doctor Who:
  * Osgood, Operation Double
  * The Eighth Doctor
  * The Five Doctors
* Jumpstart: Historic Horizons:
  * Pool of Vigorous Growth
* Lorwyn Eclipsed Commander:
  * Ashling, the Limitless
* March of the Machine Commander:
  * Ichor Elixir
* Marvel Super Heroes:
  * Black Widow, Super Spy
  * Daredevil, Man Without Fear
  * Heroic Feast
  * Iron Man Armor
  * Kang the Conqueror
  * Knight of Wundagore
  * Leader, Super-Genius
  * Loki, God of Mischief
  * Mister Hyde, Monster Within
  * Murdock's Crusade
  * Night Nurse, Healer of Heroes
  * Powerful Broker
  * Secret Invasion
  * Spider-Man, To the Rescue
  * Storm, Windrider
  * Super-Adaptoid
  * Too Evil to Stay Dead
  * Worlds Within Worlds
* Marvel Super Heroes Commander:
  * Alex Wilder, Runaway
  * Asgardian Inspiration
  * Avengers Quinjet
  * Batroc the Leaper
  * Beast Mode
  * Black Bolt, Inhuman King
  * Bob, Reluctant HYDRA Agent
  * Captain America, Skybound
  * Captain Marvel, Shooting Star
  * Council of Reeds
  * Damocles Base, Sword of Kang
  * Doctor Jane Foster
  * Fixer, Techno Terror
  * Heroes for Hire
  * Immortus, Master of Eternity
  * N'Yami-Class Mother Ship
  * Nico Minoru, Runaway
  * Shuri, the Black Panther
  * The Frightful Four
  * Timeline Inquiry
  * Vision, Spectral Synthezoid
  * Vulture, Feathered Fiend
  * Wakanda Forever!
  * Wanda's Vision
  * Wasp, Shrinking Savior
  * West Coast Expansion
* Murders at Karlov Manor Commander:
  * Otherworldly Escort
* Mystery Booster Commander Edition:
  * Ashaya's Enduring Bond
  * Case of the Lost Witness
  * Chief Magistrate of Mercadia
  * Ekthi, Contaminator Priest
  * Elda, Conjurer of Spectacle
  * Euru, Acorn Scrounger
  * Feroz, Ulgrotha's Warden
  * Flitwing, Lyev Detective
  * Grandmother Goby
  * Greensleeves
  * Grizzlegom, Hurloon Hero
  * Homer, the Hermit
  * Jandor, Fortuned Traveler
  * Lyna, Veil of Vengeance
  * Maular, the Next Evolution
  * Meatsqueak, Hoard Lord
  * Nephilim Epochal
  * Nivea, Beloved Battlemage
  * Olag and Miau, New Friends
  * Overcooked
  * Selenia, the Cursed Heart
  * Seluma, Light of Aysen
  * The Everforger
  * Tolabow, Loch Rascal
  * Uugguu, the Omniplasm
  * Valko Indorian
  * Whtz, the Bibliophile
  * Worzel, the Protector
  * Zagorka, Mother of Sanctum
* Ravnica: Clue Edition:
  * Amzu, Swarm's Hunger
* Secret Lair Drop:
  * The Fifteenth Doctor
* Star Trek:
  * Cantankerous Captain
  * Command Decision
  * Common Goal
  * DOT-7 Repair Squad
  * Dathon and Picard at El-Adrel
  * Eject the Warp Core
  * Federation Field Medic
  * Federation Probe
  * General Chang, Cold Warrior
  * Hive Mind Coprocessor
  * I'm a Doctor, Not a ...
  * La'An Noonien-Singh, Security
  * Perils of the Past
  * Shields Up!
  * Support Mission
* Star Trek Commander:
  * Captain Kirk, Boldly Going
  * Christine Chapel, Combat Medic
* Teenage Mutant Ninja Turtles Eternal:
  * Dimension X Pizzasaur
  * Foot Chopper
  * Mikey & Mona, Mutant Sitters
* The Hobbit:
  * Balin, Loremaster
  * Beorn the Fierce
  * Bolg of the North
  * Desert Were-Worm
  * Elven Passage
  * Gandalf, Goblins' Bane
  * Getaway Barrel
  * Glamdring, Foe-hammer
  * Goblin Plate Mail
  * Inside Information
  * Key to the Side-Door
  * Kili the Resourceful
  * Lake-town Mariners
  * Lake-town Toymaker
  * Last Light of Durin's Day
  * Master's Councillors
  * Mirkwood Nurturer
  * Moment of Glory
  * Orcrist, Goblin-cleaver
  * Part in Friendship
  * The Eagles Are Coming!
  * The Master of Lake-town
  * The Notary Hobbits
  * Thranduil's Decree
* Visions:
  * Time and Tide

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)