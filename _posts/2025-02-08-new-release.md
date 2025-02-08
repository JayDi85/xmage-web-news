---
layout: post
author: JayDi85
title: New blocking AI, Aetherdrift and 108 new cards
---
New release contains 108 new cards, most from Aetherdrift (including Start your 
engines mechanics), but also includes new cards from other sets like PIP or DSK. 
It also contains reworked AI's blocking with more smarter AI and improved stability 
and performance.

Warning. current version can't run local server in some machines, new fix incoming...

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## AI and reworked blocking
* now AI will use simplified 1 vs 1 combat damage simulations to choose better blocker (#13290);
* now AI will use [chump blocker](https://mtg.fandom.com/wiki/Chump_blocker) to sacrifice creature and skip game loose (in simple use cases, #4485);
* now AI will correctly use a blockers with Deathtouth, Indestructible, First/Double strike and other battle related abilities (#13290);
* fixed game freezes for no-possible block configurations like Menace (#13290);
* fixed computer cheating to ignore block requirements like Menace (now AI will choose all required blockers instead 1);

## AI and other improves
* improved performance and fixed server crashes on use cases with too much target options like "deals 5 damage divided as you choose" (#11285):
* improved performance in tournament games (now computer will play AI vs AI games at the same time);

## Other
* game: added defenders info in declared attackers log;
* game: added source info in choose mode dialogs;
* deck: added booster to DFT;
* deck: added tokens from INR;
* deck: added reprints from all Wizards Play Network, Judge Gift Cards, and Game Day Promos;
* deck: updated reprints from Special Guests;
* deck: fixed that UNF cards was illegal in command games (example: Name Sticker Goblin, #13295);

## Ability fixes
* Choose card name dialogs - added support to choose names from adventure spells (example: Anointed Peacekeeper, #13286);
* Decayed ability - improved rules text with more details (#13296);
* Dredge abilities - fixed game error in some use cases;
* Greatest power among creatures - added card hints in all related cards;
* Number of card types in graveyards - added card hint for cards like Tarmogoyf;
* Reveal abilities - added support of face down creatures (#13277);

## Card fixes
* Ballad of the Black Flag - fixed wrong text (#13300);
* Crypt of Agadeem - added card hint (#13283, #12603);
* Heaped Harvest - fixed that it trigger only once on enters and sacrifice (#13309);
* Shadow Kin - fixed game error on usage with MDF cards (#13308);
* Shifting Woodland - fixed game error on usage with MDF cards (#13308);

## New cards
* Aetherdrift - added 99 new cards;
* Aetherdrift Commander:
  * Accursed Duneyard
  * Adaptive Omnitool
  * Aetherflux Conduit
  * Peema Trailblazer
  * Rhet-Tomb Mystic
* Bloomburrow Commander:
  * Thickest in the Thicket
* Duskmourn: House of Horror:
  * Hauntwoods Shrieker
* Fallout:
  * Struggle for Project Purity
* Unfinity:
  * Priority Boarding

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)