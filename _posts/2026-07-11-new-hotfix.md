---
layout: post
author: JayDi85
title: Hot-fixes to many cards, abilities and choose dialogs
---
New release contains dozens of card and ability fixes, including copies, casts and dfc. It also improved GUI selection and auto-selection in some use cases, better game logs and many more.

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## Other
* GUI, game: added detail logs about SBA actions (player lost reason, aura/battle/world move to graveyard reason, etc);
* GUI, game: fixed not working partly selected cards list in some dialogs (example: Eerie Ultimatum, #14413);
* GUI, game: fixed that auto-choose doesn't work in some dialogs with one possible selection (1 of 1, 2 of 2, example: Orvar, the All-Form, #14804);
* GUI, deck editor: updated bans and restrictions on June 29 2026;
* GUI, deck editor: improved app stability on file selection in some Windows (#15495);
* GUI, cards viewer: fixed error on empty sets list (#15575);
* images: added reprints from M3C;
* images: improved scryfall download support by latest api (#15552);
* server, API: fixed and simplified user settings change like avatar;
* test mode: improved quick test games, now it allow spectators (use wait for me and connect by another name);

## Ability fixes
* Companion ability - fixed that it was marked as playable in some use cases;
* Cast from copied cards - fixed that it can't be selected (example: Mizzix's Mastery, Baron Helmut Zemo, #15240, #14005, #14366);
* Cloak-disguised abilities - fixed miss ward text (#15190, #15470);
* Cloak-disguised abilities - fixed card type leak to opponent by face up cost (#13431);
* Copy abilities: fixed that flickering copied tokens can affect original permanents (example: rooms or saga, #14409, #14548);
* Modal double faced commanders - fixed that it was able to shuffle it without replacement effect (example: Glimpse of Tomorrow, #14991, #14992);
* Modal double faced cards: fixed wrong mana value for copied permanents (#15415, #15471);
* Non-modal double faced cards: fixed wrong mana value for back sides, for copied permanents (#15471);

## Card fixes
* Ant-Man, Elusive Avenger - fixed game error on usage (#15457);
* Aurelia, the Warleader - fixed wrong card name (#15581);
* Binding Geist // Spectral Binding - fixed not working aura face (#15472);
* Black Panther, Vanguard - fixed that it affect opponent's permanents;
* Blaster Hulk - fixed game error on usage;
* Deathbringer Regent - fixed that it count only controlled creatures;
* Shadowfax, Lord of Horse - fixed miss Haste ability (#15567);
* Stalwart Successor - fixed game error on non-creature tokens;
* Sword of the Meek - fixed that their combo was preventable by Elesh Norn, Mother of Machines and other (#15220, #15231);
* Syr Vondam, Sunstar Exemplar - fixed that it can't trigger on self exile or blink (#15583);
* Thalakos Deceiver - fixed wrong effect's duration, must be until end game (#15324);
* Thanos, the Mad Titan - fixed miss choosing by players;
* The Wondrous Wasp - fixed wrong lose abilities effect duration;
* Vibranium token - fixed miss vibranium subtype;
* With Great Power... - fixed not workable effect on die;

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
