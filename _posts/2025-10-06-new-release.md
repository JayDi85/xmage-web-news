---
layout: post
author: JayDi85
title: Reworked AI, bracket/edh levels, and ~1200 new cards
---
New release contains ~1200 new cards from old and new sets. It also includes new retro frame card style rendering, deck's backet/edh calculation, supported moxfield and archidekt text import. AI targeting logic was fully reworked and improved for better performance and stability. Added many promo sets, tokens and images. Also it contains 3000+ changes and fixes for cards and abilities.

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## New retro frame render
Added new retro frame render for all classic cards and reprints (#13563). If you like that style then you can force it for all modern cards too by Preferences - GUI Images menu.

<img width="856" height="388" alt="shot_251005_214820" src="https://github.com/user-attachments/assets/a10880d2-27d6-490d-8c83-ebe02696e56d" />

## Deck editor and bracket/EDH levels
* bracket: added bracket level calculations in deck's validation panel;
* bracket: added detail cards info for each bracket level;
* bracket: added all levels support, including x2 infinite combos due https://commanderspellbook.com ;
* edh: added power level info in deck validation panel (#5361, #11732, #13341);
* edh: added detail calculation info (hint with cards and their power levels);
* edh: fixed that deck's edh power level ignore individual card's levels and used only commanders;
* edh: removed hidden and outdated deck restrictions by commander colors;
* edh: now players can really limit their table by edh power level;

![Image](https://github.com/user-attachments/assets/e0157837-e84e-4e8f-9314-6a2e4dcb4227)

## Deck editor, search, and deck generation improves
* search: added non-strict search (enter multiple words in any order or case, #6548);
* search: added strict search (enter exact phrase inside quotes, #6548);
* generate: added commander decks support (#5680);
* generate: added more options for deck size;
* generate: fixed and improved cards searching due selected colors (now it search by color identity instead mana cost);
* deck: improved invalid deck information (added more details in wrong commander color);
* deck: now a duplicated cards adds to the same place as original cards (#3314);
* deck: improved grid padding for better cards selection by mouse;
* deck: improved deck import from clipboard (added support of moxfield and archidekt decks format, #13838);
* deck: fixed that clipboard import can choose wrong promo card (close #7666);

## Draft improves
* added drafts with multiplayer game support (see examples in #13701);
  * new tourney's single game mode allow to play tourneys/drafts with all players in one game without multiple rounds;
  * it's allow to setup classic drafts with 1 vs 1 games and multiple rounds
  * added AI opponents support including draft bots from a public servers;
  * improved single/multiplayer drafts - allow unlimited number of draft bots;
* example with single game mode:
  * setup draft with x4 humans -> draft + one game with x4 humans;
  * setup draft with x2 humans and x2 draft bots -> draft + one game with x2 humans;
  * setup draft with x1 human, x1 mad bot and x2 draft bots -> draft + one game with human vs AI;
* example with multiple games mode:
  * setup draft with x4 humans -> draft + multiple 1vs1 games until tourney finish;
* other: fixed miss tourney Booster Draft Swiss (Rich Man);

![shot_250531_101002](https://github.com/user-attachments/assets/9bdee4e2-6d97-4a18-929f-7c5c78e550dc)

## Cube improves
* deck: migrated to single cube files (**warning for server's owners**, if you use custom config the it require some fixes, see default config);
* deck: better support of Cube From Deck (fixed client/server errors, additional info about loaded cards, etc);
* deck: updated to latest cube versions (mtgo vintage, paper);

## AI improves
* fully reworked targeting and selection logic (#13638, #13606, #11285, #11134, #11666, #13617, #13613);
* now AI will look at effect's outcome and target's battlefield score to make a most valuable choice;
* added detail logs on too long thinks (show battlefield/stack stats, abilities activation chain on AI freezes, #10154, #13766);
* improved get amount selection (now AI will not choose big and useless values);
* improved spell selection on free cast (now AI will try to cast spells with valid targets only);
* improved performance and server stability in games with "choose name" effects (#11285);
* improved support of multiple targets abilities;
* improved performance on too many possible targets (fix game freezes and server crashes - #9539, #9438, #9518, #11285, #5023);
* fixed game freeze in some use cases with invalid target combinations (#13606, #11285);
* fixed game errors with source related filters (#13713);
* fixed game freeze in hand's cards selection (#13290);
* fixed game freeze in target amount selection with X=0 (#13290);

## Performance and stability
* fixed game freeze on leaving player before finish target selection (example: Nethergoyf, #13567, #11285);
* fixed game freeze on auto-choice usages with disconnected or under control players (#11285);
* disabled triggers integrity checks for better performance;

## Other
* download: new xmage install will save images as raw files instead zip archives by default for better compatibility (#13978);
* images: added many promo sets and miss promo cards (#13834, #13903);
* images: added and fixed many miss or outdated images in multiple sets (#13760);
* images: added missing tokens for SLD, UNF, TDC, DSK, UND, UGL, WHO and many other sets (#13775, #13779);
* images: fixed sets/rarity icons download from gatherer source (#13797);
* images: updated gatherer source for latest images download, improved some tokens download (#13826);
* images: fixed miss emblems download of Star Wars' Yoda and Aurra Sing;
* images: improved cards rendering with full art like poster cards (#13911);
* server: fixed that it doesn't allow to use 3 characters names despite config settings;
* server: fixed that's server can't start on some wrong config settings;
* deck: added Freeform Unlimited deck type to play games with any cards amount (#13815);
* deck: updated bans list for multiple game modes;
* deck: updated Canadian Highlander point list;
* GUI, game: fixed that attacking creature draws a wrong colored arrow after blocked creature removed (must be gray, #11894);
* GUI, game: fixed that player doesn't mark avatar as selected/green in "up to" targeting;
* GUI, game: fixed small font in some popup messages on big screens (related to #969);
* GUI, game: added min targets info for target selection dialog;
* GUI, game: added source info in "choose number/amount" dialogs, added auto-choose for single possible value (#13638);
* GUI, lobby: fixed some errors on table/game close from server side (#13844);


## Ability fixes
* Bestow - improved support of aura copy and attach as bestow, e.g. Arna Kennerüd use case (#13559);
* Bestow - reworked implementation, many combo and bugs fixes (#13973);
* Can block any number of creatures - fixed that it can be broken with some of "can block an additional creature" effects;
* Can't sacrifice effects - fixed that some cards with sacrifice can ignore it (#13916);
* Changeling - improved combo support with some cards (see example: Valley Flamecaller and Alania, Divergent Storm, #13640);
* Craft ability - improved combo support with transform cards (#13729);
* Foretell ability - improved implementation and fixed some bugs (#13879);
* Kate Stewart, All Will Be One - fixed wrong combo with suspended permanents (#13870);
* Land type changing effects - improved combo support and layer dependency processing;
* Named card name - fixed wrong card name in some rules, e.g. with gain ability;
* Player under control - fixed that it doesn't hide opponent's hand after control lost (#13353);
* Remove time counter - fixed that it can't be selected for permanents with protection (example: Rift Elemental, #13857);
* Search and put to battlefield - improved combo support with MDF cards (#13466, #13683);
* Split cards - improved combo support with cards like Feather, the Redeemed (#12353, #13665);
* Targeting and non-targeting cards - fixed that effects wrongly use target and non target choices (wrong protection, targetted triggers, etc - #13680);
* Ward ability - improved combo support with re-casting aura (#13523, #13740);

## Card fixes
* Aetherflux Conduit - fixed that it using mana value rather than mana spent;
* Aettier and Priwen - fixed not working (#13822);
* Alpine Moon - fixed that it incorrectly removing abilities in layer 4;
* An-Havva Constable - fixed wrong count calc;
* Angel of Jubilation and Yasharn, Implacable Earth - fixed that it incorrectly allowing/preventing sacrifice costs (#13753, #9650, #13422);
* Ballad of the Black Flag - fixed wrong turn condition of last ability (#13785);
* Bello, Bard of the Brambles - fixed wrong layers combination;
* Bull-Rush Bruiser - fixed wrong effect duration;
* Clement The Worrywort - fixed wrong target stacking;
* Clement, the Worrywort - fixed wrong implementation;
* Conformer Shuriken - fixed wrong power compare on trigger (#13804);
* Contractual Safeguard - fixed wrong lookup filter;
* Diplomatic Relations - fixed missing target;
* Dragon's Fire - fixed wrong targeting (#13756);
* Dwarven Catapult - fixed game error on usage;
* Fall of the First Civilization - fixed that it not allowing nonlands to be chosen and that it doesn't drawing enough cards;
* Font of Agonies - improved combo with fetch lands support (#13717);
* Frodo, Determined Hero - fixed wrong lookup filter;
* Gavi, Nest Warden - fixed game error on usage;
* Gilgamesh, Master-at-Arms - fixed that it allowing any permanent to be attached (#13823);
* Golbez - fixed that it returns card to hand, not battlefield;
* Gorex, the Tombshell - fixed that it doesn't return cards on death (#13657);
* Gossip's Talent - fixed game error on usage (#13652);
* Illvoi Light Jammer - fixed wrong mana cost;
* Incarnation Technique - fixed that it doesn't processing trigger properly between the mill and return (#13601);
* Jaya, Fiery Negotiator - fixed emblem's trigger and wrong zone;
* Ketramose, the New Dawn - fixed that it doesn't seeing itself on exile;
* Kolodin, Triumph Caster - fixed missing targets;
* Krile Baldesion - fixed not working trigger;
* Louisoix's Sacrifice - fixed wrong additional cost (#13812);
* Maarika - fixed that it showing all enemy untapped, noncreature permanents as being required to block her, improved card hints;
* Mathas, Fiend Seeker - fixed that ability coming back when another counter is added;
* Migloz, Maze Crusher - fixed wrong duration;
* Mirror Golem - fixed game error with token copy (#13850);
* Mirror of Life Trapping - fixed combo support with face down creatures (#13749);
* Mistrise Village - fixed wrong effect duration and discard logic;
* Nahiri, Forged in Fury - fixed the trigger firing for all attacking creatures, not just equipped ones (#13893);
* Nibelheim Aflame - fixed that it wrongly damage a targeted creature (#13813);
* Oni-Cult Anvil - fixed that it doesn't trigger on itself;
* Overwhelming Surge - fixed wrong lookup filter (#13614);
* Parapet Thrasher - fixed wrong triggered ability;
* Phelia, Exuberant Shepherd - fixed that it return all cards (#13722);
* Pit of Offerings - fixed wrong targeting;
* Portal Manipulator - fixed that it should work during any declare attackers step, not just the controller's;
* Professor Hojo - fixed miss ability type check (#13814);
* Professor Hojo - fixed that it can’t be used on low mana (#13811);
* Psychic Frog - fixed wrong exiling cards;
* PuPu UFO - fixed that it setting its toughness to 0;
* Pulsar Squadron Ace - fixed that it not revealing the card it finds;
* Push // Pull - fixed wrong multiple triggers (#13450);
* Quilled Charger - fixed wrong saddle duration;
* Ragost, Deft Gastronaut - improved by card hint;
* Ravenous Slime - fixed that it not exiling when it dies simultaneously;
* Repentance - fixed wrong damage source;
* Resurrection Orb - fixed that trigger working on creature that changed zones (#12974);
* Rex - fixed that it doesn't restrict stolen abilities to only once per turn;
* Rhet-Tomb Mystic - fixed wrong color cost (#13582);
* Rise of the Dread Marn - fixed that it counting noncreature permanents (#13738);
* Ryan Sinclair - fixed that it not allowing spells with equal mana value to be cast;
* Sensational Spider-Man - fixed that it not targeting at all;
* Shared Fate - fixed that it ignore range of influence (#13839);
* Shinryu, Transcendent Rival - added card hint about which player was chosen;
* Shuriken - fixed that it giving control to wrong player;
* Sigurd, Jarl of Ravensthorpe - fixed that last ability didn't trigger on entering sagas;
* Spectral Denial - fixed wrong target;
* Stadium Headliner - fixed wrong damage;
* Stalwart Successor - fixed that it doesn't check entering permanents;
* Strago and Relm - fixed wrong casting player (#13803);
* Struggle for Project Purity - fixed miss rules text (#13568);
* The Wind Crystal - fixed that it not granting lifelink;
* Tombstone Stairwell - fixed that it doesn't destroy tokens on leaves the battlefield;
* Topography Tracker - fixed that it applying to opponents' creatures;
* Transpose - fixed wrong zone;
* Tromell, Seymour's Butler - fixed wrong etb effect (#13894);
* Vampiric Embrace - fixed wrong +1/+1 creature (#13615);
* Will of the Mardu - fixed not working first ability (#13558);
* Zedruu the Greathearted - added card hint;
* Zenos yae Galvus - fixed that it was not letting you choose a creature when it entered;
* Zodiark, Umbral God - fixed that it only count creatures;
* and much more undocumented fixes with cards and abilities;

## New cards
* Total new cards: 1156;
* Avatar: The Last Airbender - added 81 new cards;
* Avatar: The Last Airbender Eternal - added 51 new cards;
* Edge of Eternities - added 252 new cards;
* Edge of Eternities Commander - added 24 new cards;
* Final Fantasy - added 317 new cards;
* Final Fantasy Commander - added 108 new cards;
* Marvel's Spider-Man - added 186 new cards;
* Marvel's Spider-Man Eternal - added 20 new cards;
* Assassin's Creed:
  * Altair Ibn-La'Ahad
  * Fall of the First Civilization
  * Havi, the All-Father
  * Jacob Frye
  * Monastery Raid
  * Ratonhnhaketon
  * Shay Cormac
* Bloomburrow Commander:
  * Echoing Assault
  * Sword of the Squeak
* Commander Legends: Battle for Baldur's Gate:
  * Commander Liara Portyr
* Doctor Who:
  * Ashad, the Lone Cyberman
  * Barbara Wright
  * Blink
  * Danny Pink
  * Day of the Moon
  * Everybody Lives!
  * Genesis of the Daleks
  * Hunted by The Family
  * Idris, Soul of the TARDIS
  * Midnight Crusader Shuttle
  * Nyssa of Traken
  * Ryan Sinclair
  * Strax, Sontaran Nurse
  * Sycorax Commander
  * The Caves of Androzani
  * The Curse of Fenric
  * The Day of the Doctor
  * The Eleventh Doctor
  * The Face of Boe
  * The Fourth Doctor
  * The Master, Formed Anew
  * The Master, Gallifrey's End
  * The Master, Mesmerist
  * The Parting of the Ways
  * The Seventh Doctor
  * The Toymaker's Trap
  * The War Games
  * The Wedding of River Song
  * Trial of a Time Lord
  * Vislor Turlough
* Duskmourn: House of Horror:
  * Ghostly Dancers
  * Keys to the House
  * Marina Vendrell
  * Monstrous Emergence
  * Reluctant Role Model
  * Trial of Agony
  * Undead Sprinter
  * Valgavoth, Terror Eater
* Duskmourn: House of Horror Commander:
  * Ancient Cellarspawn
  * Barbflare Gremlin
  * Demonic Covenant
  * Into the Pit
  * Sadistic Shell Game
  * Soaring Lightbringer
  * Star Athlete
* Fallout:
  * Inventory Management
  * Mysterious Stranger
  * Nuka-Nuke Launcher
  * Preston Garvey, Minuteman
  * Three Dog, Galaxy News DJ
  * Vault 11: Voter's Dilemma
  * Vault 13: Dweller's Journey
* Foundations Jumpstart:
  * Aphelia, Viper Whisperer
  * Psemilla, Meletian Poet
* Lorwyn Eclipsed:
  * Ashling's Command
  * Bitterbloom Bearer
  * Deceit
  * Eirdu, Carrier of Dawn
  * Emptiness
  * Figure of Fable
  * Formidable Speaker
  * Isilu, Carrier of Twilight
  * Morningtide's Light
  * Mutable Explorer
  * Sygg, Wanderbrine Shield
  * Sygg, Wanderwine Wisdom
* Mirage:
  * Discordant Spirit
  * Shadowbane
  * Sirocco
* Modern Horizons 3 Commander:
  * Exterminator Magmarch
  * Overclocked Electromancer
  * Rampant Frogantua
  * Tempt with Mayhem
* Murders at Karlov Manor Commander:
  * Foreboding Steamboat
  * Mob Verdict
  * Serene Sleuth
  * Unexplained Absence
* Outlaws of Thunder Junction Commander:
  * Forger's Foundry
* Ravnica: Clue Edition:
  * Boros Strike-Captain
  * Covetous Elegy
  * Dimir Strandcatcher
  * Frenzied Gorespawn
  * Furious Spinesplitter
  * Herald of Ilharg
  * Memory Vampire
  * Ordruun Mentor
  * Portal Manipulator
  * Resonance Technician
* Secret Lair Drop:
  * Abby, Merciless Soldier
  * Aloy, Savior of Meridian
  * Amy Rose
  * Atreus, Impulsive Son
  * Dr. Eggman
  * Ellie, Brick Master
  * Ellie, Vengeful Hunter
  * Jaws, Relentless Predator
  * Joel, Resolute Survivor
  * Knuckles the Echidna
  * Kratos, God of War
  * Shadow the Hedgehog
  * Sonic the Hedgehog
  * Super State
* Transformers:
  * Cyclonus, Cybertronian Fighter
  * Cyclonus, the Saboteur
* Warhammer 40,000 Commander:
  * Lucius the Eternal
  * The Red Terror

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)