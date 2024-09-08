---
layout: post
author: JayDi85
title: Non-blocking GUI, ~170 new cards and other
---
New release contains ~170 newly implemented cards from DSK, YNEO, ACR, BLB, BLC and other new and old sets. It also include stability fixes for macOS systems, new non-blocking GUI, new dark theme, scryfall images fix and other improves.

**Warning** for server admins - if you are using custom `config.xml` then it must be manually updated with Remixed -> Reshuffled replacement. See full release notes for detailed migration instruction.

## New non-blocking GUI
- added non-blocking UI to almost all app and game dialogs;
- it allows to switch between UI dialogs and use any UI elements at any moment;
- it allows to use chat, card popup, battlefield, concede and other features while choosing (#12670);
- it allows to download images while playing (experimental feature, #4160);
- example use case: before choose a card name you want to research battlefield and other zones;

## New GUI theme
* added new dark theme named Carbon Fiber (see Preferences -> GUI theme, #12733);
* ![shot_240908_194948](https://github.com/user-attachments/assets/451c0ff2-1453-494e-ba49-85ffb0f44128)

## Other fixes
* app: fixed freezes on macOS systems in some use cases (related to #12431, #11292, #9300, #4920);
* game: update bans list from August 26th 2024 (#12739);
* game: renamed Chaos Remixed Draft to Chaos Reshuffled Draft (#12755);
* download: fixed broken images download from scryfall (#12817);
* download: improved cancel stability and fixes that it can't stop preparing/downloading process in some use cases;
* download: added Mystery Booster 2;
* connection: added wrong connection message for wrong java versions;
* connection: auto-connect visible in main menu on startup instead app freeze;
* connection: added <ESC> button to close connection dialog;
* GUI, game: fixed wrong number of targets in stack ability for some use cases (example: cumulative upkeep, #12824);

## Ability fixes
* Attach to permanent - fixed that aura with non-legal target was able to move to battlefield and back to graveyard (303.4g, #12098);
* Attach to permanent - improved combo support with prevention and other effects (example: Unfinished Business and Shroud ability, #12098);
* Create token effects - improved combo support with copy effects and multiple tokens (#12704);

## Card fixes
* Alchemist's Talent - fixed wrong usage of class 3 effects;
* Coram, The Undertaker- fixed that it doesn't allow to play lands and instances (#12691);
* Corrosive Ooze - fixed that it does not destroy Equipment (#11766);
* Dazzling Denial - fixed miss target to counter;
* Dewdrop Cure - fixed that it return to hand instead battlefield;
* Dracoplasm - fixed wrong sacrifice;
* Empty the Laboratory - fixed wrong processing of death triggers (#12770);
* Everquill Phoenix - fixed missing target in the token;
* Keen-Eyed Curator - fixed game error on usage in deck (also fixed Gustha's Scepter, Eater of Virtue, Death-Mask Duplicant);
* Maskwood Nexus - improved combo support with modal double-faced cards (#12554, #10607);
* Nearby Planet - fixed that it doesn't appear to be able to tap for mana (#12743);
* Phyrexian Negator - reworked implementation;
* Scythe of the Wretched - fixed not working trigger (#12657);
* Sergeant at Arms - fixed that it triggers all the time instead on kicker only (#12705);
* Sontaran General - fixed that it goaded first opponent instead all (#12666);
* Stargaze - fixed wrong effect on small library;
* Teferi's Ageless Insight - improved combo support with "for each card drawn this way" effects (#12616);
* Tempt with Bunnies - fixed wrong tokens count, improved combo support in multiplayer (#12708, #12702);
* Tempt with Vengeance - fixed wrong tokens count, improved combo support in multiplayer  (#12708);
* The Fourteenth Doctor - fixed game error on usage (#12689);
* Thornvault Forager - fixed wrong mana amount;
* Unbound Flourishing - improved combo support with copy and other effects, X doubling now a triggered ability (#12597);
* Verdant Succession - improved combo support with multiple triggers (#12695);
* Warren Warleader  - fixed miss boost effect;
* Wicked Slumber - fixed game error on usage, improved choice dialog (#12665);

## Server config migration
Due Remixed -> Reshuffled renaming new config must contain follow lines (search old config by `Remixed`):
```
<tournamentType name="Booster Draft Elimination (Reshuffled)" jar="mage-tournament-boosterdraft-1.4.54.jar" className="mage.tournament.ReshuffledBoosterDraftEliminationTournament" typeName="mage.tournament.ReshuffledBoosterDraftEliminationTournamentType"/>
...
<tournamentType name="Booster Draft Swiss (Reshuffled)" jar="mage-tournament-boosterdraft-1.4.54.jar" className="mage.tournament.ReshuffledBoosterDraftSwissTournament" typeName="mage.tournament.ReshuffledBoosterDraftSwissTournamentType"/>
```

## New cards
* Duskmourn: House of Horror - added 104 new cards;
* Duskmourn: House of Horror Commander:
    * They Came from the Pipes
* Alchemy: Kamigawa
    * Boseiju Pathlighter
    * Dragonfly Pilot
    * Experimental Pilot
    * Jukai Liberator
    * Kami of Bamboo Groves
    * Swarm Saboteur
* Assassin's Creed
    * Adewale, Breaker of Chains
    * Assassin Initiate
    * Bleeding Effect
    * Caduceus, Staff of Hermes
    * Edward Kenway
    * Eivor, Wolf-Kissed
    * Mjolnir, Storm Hammer
    * The Capitoline Triad
    * Yggdrasil, Rebirth Engine
* Bloomburrow
    * Camellia, the Seedmiser
    * Fireglass Mentor
    * Gev, Scaled Scorch
    * Helga, Skittish Seer
    * Kastral, the Windcrested
    * Long River Lurker
    * Mockingbird
    * Osteomancer Adept
    * Pawpatch Recruit
    * Rottenmouth Viper
    * Season of Loss
    * Season of the Burrow
    * Starfall Invocation
    * Sugar Coat
    * Three Tree City
    * Valley Floodcaller
    * Valley Questcaller
* Bloomburrow Commander
    * Alchemist's Talent
    * Arthur, Marigold Knight
    * Bello, Bard of the Brambles
    * Gourmand's Talent
    * Hazel of the Rootbloom
    * Mr. Foxglove
    * Ms. Bumbleflower
    * Swarmyard Massacre
    * Tempt with Bunnies
    * The Odd Acorn Gang
* Doctor Who
    * River Song
* Fallout
    * Animal Friend
    * Codsworth, Handy Helper
* Foundations
    * Felidar Savior
    * Helpful Hunter
    * Prideful Parent
    * Vengeful Bloodwitch
* Jumpstart: Historic Horizons
    * Kiora, the Tide's Fury
    * Subversive Acolyte
* Mirage
    * Reflect Damage
    * Yare
* Modern Horizons 3 Commander
    * Blaster Hulk
    * Wonderscape Sage
* Murders at Karlov Manor Commander
    * Panoptic Projektor
* Tales of Middle-earth Commander
    * Courageous Resolve
* Unfinity
    * Atomwheel Acrobats
    * Six-Sided Die
* Unglued
    * Team Spirit
* Visions
    * Forbidden Ritual
* Warhammer 40,000
    * Seeker of Slaanesh
    * The Ruinous Powers

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](http://xmage.today/#donate).