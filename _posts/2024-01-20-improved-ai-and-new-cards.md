---
layout: post
author: JayDi85
title: Improved AI and new cards
---

AI improves:
* added support to attack battle permanents (#10246);
* fixed that AI was able to attack multiple targets by single creature (#7434);
* fixed wrong usage of Shielded By Faith's reattachment effect (#11672);

Other:
* GUI: improved stability of popup hint window (fixed game freeze in some use cases, #11595);
* GUI: improved font color of popup card hint (#11663);
* sound: now music settings will be applied after save (#11675);
* game: updated Canadian Highlander points list (#11602);
* game: improved booster generation for RVR set;
* game: improved stability of commander games (#11081);
* images: added double faced images download from REX;

Abilities fixes:
* Adds mana of any type produced - fixed support of multiple mana choices (example: Kinnan, Bonder Prodigy, #11643);
* Can't be sacrificed - improved cards and combo support (example: Assault Suit, #11587);
* Convoke, spend only mana produced by - improved combo support with some cards (example: Manamorphose can be used to cast Imperiosaur now, see #11620);
* Hydra cards - fixed that copies enter to battlefield without counters (example: Magus Lucea Kane copy Neverwinter Hydra or Apocalypse Hydra, #11581);
* Prevent damage - fixed that it was able to prevent damage for blinked/flickered permanents (example: Desert Sandstorm, #11606);

Card fixes:
* Agent of Treachery - added card hint;
* Alistair, the Brigadier - fixed wrong checks of historic permanents (#11665);
* Armored Kincaller - fixed that it trigger on itself (#11653);
* Consulate Surveillance and Healing Grace - fixed wrong preventing effects (#11623);
* Desolation - fixed wrong lands count;
* Domri Chaos Bringer - fixed that first ability not granting riot to the creature spell (#11604);
* Dueling Grounds - fixed that it's applying to non creatures (#11662);
* Faerie Snoop - fixed wrong card destination;
* Goblin Researcher - fixed wrong conditional (#11653);
* Goldberry, River-Daughter - fixed wrong counters count;
* Incursion Specialist - fixed wrong block ability (#11589);
* Karn Liberated - improved game restart support in commander games (#11628, #11081);
* Mana Maze - fixed game error on usage (#11572, #11575);
* Manamorphose - fixed that it can't be used to cast Imperiosaur (#11620);
* Michiko Konda, Truth Seeker - fixed miss trigger;
* Mind Stone - fixed rarity in WOC set;
* Morality Shift - fixed wrong exchange ability;
* Plague Reaver - fixed wrong target (#7714);
* Pooling Venom - fixed wrong attachment effect (#11680);
* Possessed Portal - fixed wrong sacrifice ability (#11603);
* Rowan's Grim Search - fixed wrong no cards put (#11660);
* Runadi, Behemoth Caller - fixed combo support with X cost (#11626);
* Sanwell Avenger Ace - fixed that it's allowing casting for free (#11674);
* Sword of Light and Shadow - removed duplicated choose dialog (#11636);

Also, new release contains new cards and reprints for:
* CLB: Jon Irenicus, Shattered One;
* CLU: reprints, Library;
* ICE: Touch of Vitae;
* LCC:
  * Pantlaza, Sun-Favored, From the Rubble, Admiral Brass, Unsinkable, Bronzebeak Foragers, Sunfrill Imitator;
  * Progenitor's Icon, Wayta, Trainer Prodigy, Arm-Mounted Anchor, Contest of Claws, Carmen, Cruel Skymarcher;
  * The Grim Captain's Locker, Clavileno, First of the Blessed, Ripples of Potential, Promise of Aclazotz;
* LCI: reprints, tokens;
* LTC: Hithlain Rope;
* MIR: Mindbender Spores;
* MKC: Morska, Undersea Sleuth;
* MKM: added many cards;
* PH19: The Cinematic Phoenix;
* PIP: Mr. House, President and CEO;
* REX:
  * Hunting Velociraptor, Permission Denied, Don't Move, Welcome To... // Jurassic Park;
  * Life Finds a Way, Spitting Dilophosaurus, Ellie And Alan, Paleontologists, Savage Order;
  * Ravenous Tyrannosaurus, Swooping Pteranodon;
* UNF: Celebr-8000;
* WHO: Adipose Offspring, The Third Doctor, Duggan, Private Detective, Leela, Sevateem Warrior;

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/) 
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](http://xmage.today/#donate).