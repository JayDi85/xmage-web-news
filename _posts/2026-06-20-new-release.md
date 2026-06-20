---
layout: post
author: JayDi85
title: Marvel's sets, mutate and ~430 new cards
---
New release contains ~430 new cards from old and new sets, 30+ cards with mutate mechanic from Ikoria and other. It also has some fixes for cards, abilities, gui's card selection and deck editor.

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## Other
* game: fixed game freeze on auto-choose and 1 available card to select (example: Inquisition of Kozilek, #14018, #14420, #14630);
* deck editor: improved check and error messages on importing of bad deck file or cards;
* deck editor: fixed layout errors on loading some decks (#11157);
* deck editor: fixed deck corruption (cards duplication) on oldest cards replacement use with O button, improved replace stats (#8104);

## Ability fixes
* Alternate casting - fixed that it was able to activate some alternate cost (example: Cyclonic Rift with Bolas's Citadel, #14934);
* Fateseal ability - fixed that it can't to put any cards to the bottom (example: Mesmeric Sliver, #14167);
* Squad costs - fixed that it require payments in some use cases (example: Space Marine Devastator with Etali, Primal Storm, #14940, #14966);
* Type adding effects - fixed that it doesn't apply to some MDFC and other multi faces creatures (example: Biotransference, Conspiracy, Leyline of Transformation, and Maskwood Nexus, #14817, #14925);
* X-cost spell with alternative cost - fixed that some effects can't see X value (example: Geometer's Arthropod, #14989);


## Card fixes
* Ennis, Debate Moderator - fixed game error on usage;
* Fix Flow State - fixed wrong effect's conditional (#14959);
* Hall of the Bandit Lord - fixed game error on usage (#12162);
* Maralen, Fae Ascendant - added outdated window cleanup, added card hints;
* Mishra, Excavation Prodigy - fixed wrong multi-triggers on discard effects;
* Old-Growth Educator - fixed that infusion ability only adds one +1/+1 counter (#14984);
* Raph & Mikey, Troublemakers - fixed game error on usage (#15191);
* Raphael, Most Attitude - fixed game error on usage;
* Seifer Almasy - fixed game error on usage (#14943);
* Seifer, Balamb Rival - fixed game error on usage (#14942);
* Spider-Man Noir - fixed game error on usage (#14935);
* Taster of Wares - fixed not working card targeting (#14932);
* The Ooze - fixed not working trigger (#15166);
* Urza, Powerstone Prodigy - fixed wrong multi-triggers on discard effects;

## New cards
* Total new cards: 424;
* Alchemy: Secrets of Strixhaven:
  * Corpseweaver Prodigy
  * Glorifying Verse
  * Grave Studies
  * Interdisciplinary Studies
* Commander Legends: Battle for Baldur's Gate:
  * Grell Philosopher
* Fallout:
  * Cass, Hand of Vengeance
  * Strong Back
* Ice Age:
  * Mercenaries
* Ikoria: Lair of Behemoths - added 31 new cards with mutate:
* Marvel Super Heroes - added 158 new cards;
* Marvel Super Heroes Commander - added 214 new cards;
* Mirage - added 1 new cards:
  * Cycle of Life
* Teenage Mutant Ninja Turtles:
  * Brilliance Unleashed
  * Novel Nunchaku
  * Turtles Forever
* Tempest:
  * No Quarter
* The Hobbit:
  * An Unexpected Party
  * Bilbo, Luckwearer
  * Bilbo, Thief in the Night
  * My Precious
  * Smaug the Magnificent
  * The Arkenstone
  * Tom, Bert, and William
  
Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)