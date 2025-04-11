---
layout: post
author: JayDi85
title: Hot-fix release and December banned cards
---
New hot-fix release contains December 16 banned and restricted cards list. It includes ~6 new cards from Baldur's Gate, Duskmourn, Foundations and other sets, some ability and card fixes too.

## Other fixes
* game: updated bans list for [December 16 changes](https://magic.wizards.com/en/news/announcements/banned-and-restricted-december-16-2024);
* client: added java version and charset info to error report;
* client: improved default run scripts for better compatibility with non-ascii paths, increased default memory limit to 2 GB (#13121);

## Ability fixes
* Dies, destroy, leaves and sacrifice triggers - fixed that it doesn't work on itself for some cards (#13089);
* When you cast this spell - fixed that it required double cost for cards with alternative costs like Evoke (example: Nulldrifter, #12843);

## Card fixes
* Come Back Wrong - fixed game error on usage with tokens (#13056);
* Elvish Branchbender - fixed that it works after blink (#13064);
* First Responder - fixed that it doesn't add counters;
* Gornog, the Red Reaper - fixed that it doesn't trigger on attack (#13100);
* Havengul Laboratory // Havengul Mystery - fixed that it doesn't transform back on creature leaves;
* Itlimoc, Cradle of the Sun - added card hint with additional info;
* Orim's Chant - fixed game error on kick usage (#13130);
* Pol Jamaar, Illusionist - fixed not working draw effect (#13106);
* Shivan Dragon - fixed wrong card name in J21 set (#13138);

## New cards
* Alchemy Horizons: Baldur's Gate:
  * Mirror of Life Trapping
* Commander Legends: Battle for Baldur's Gate:
  * Hezrou
* Duskmourn: House of Horror Commander:
  * The Master of Keys
* Foundations:
  * Banner of Kinship
  * Quilled Greatwurm
* Mystery Booster 2:
  * Hish of the Snake Cult

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).