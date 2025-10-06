---
layout: post
author: JayDi85
title: Turn control, boosters, improved AI and 137 new cards
---
New release contains 137 new cards, most from Aetherdrift (including Exhaust mechanic), 
but also includes new cards from ACR, BLC, DSK, DSC, PIP and other. Added turn control 
of another player, improved AI, better mana pool and payment dialogs and boosters/draft 
support for all latests sets like FDN.

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## Turn control, boosters, improved AI and 137 new cards
New release contains 137 new cards, most from Aetherdrift (including Exhaust mechanic), but also includes new cards from ACR, BLC, DSK, DSC, PIP and other. Added turn control of another player, improved AI, better mana pool and payment dialogs and boosters/draft support for all latests sets like FDN.

## Turn control support
* game: added support to control of another human or AI player (cards like Emrakul, the Promised End, #12878);
* game: added support of 720.1. to reset control in the turn beginning instead cleanup step (#12115);
* game: fixed game freezes and wrong skip settings usages in human games (#12878);
* game: fixed game freezes while controlling player leaves/disconnect on active priority/choose of another player;
* GUI: added playable and choose-able marks for controlling player's cards and permanents, including switched hands;
* GUI: added controlling player name in all choice dialogs;
* AI: fixed game freezes in computer games (if AI try to take control over human);
* cheats: added default commands to take and remove control over another player ([server's test mode only](https://github.com/magefree/mage/wiki/Development-Testing-Tools));

## AI improves
* combat: fixed that computer safely blocks the weakest creature instead most powerful;
* combat: fixed that computer blocks an attacker by biggest creature instead optimal;
* game: fixed that computer can cheat with target selection and choose 1 creature instead multiple required (example: sacrifice, #13219);

## Boosters improves
* added play and collection boosters for all actual sets like FDN, DSK, ACR, WHO, CMM, PIP and other (full list in #13160);
* added [real life booster collation](https://www.lethe.xyz/mtg/collation/introduction.html) to Conflux (CON) (#13169);
* added real life booster collation to Alara Reborn (ARB) (#13169);

## GUI improves
* game: improved priority pass on non-empty mana pool (no more confirm dialogs on active "don't lose unspent mana" and other effects, #11717);
* game: improved "do if cost pay" dialog for better auto-answer support - now user can hide an untap cost dialog for already untapped permanent (example: Mana Vault, use right click on buttons, #2656);
* game: fixed rare error while dragging/moving card on first play (close #13201);

## Other
* images: fixed symbols download from gatherer website (#13159, #13157, #9266);
* images: added reprints and boosters for Innistrad Remastered (INR);
* images: added reprints to Secret Lair Drop (SLD), Magic Online Promos (PRM), Shadows of the Past (SIS) and many other sets (full list in #13160);
* images: added tokens for some sets like BLC, DSC;
* images: fixed missing images in SLD and some old sets (#13221);
* deck: fixed outdated names for some promo and old sets;

## Abilities fixes
* Create copy effects - fixed that it can't copy second side of the modal double-faced card (#13269, #13002);
* Defending player conditions - improved [802.2a rules support](https://mtg.wtf/help/rules#section-802-2a), fixed that some effects wrongly fizzled after attacking creature removed from battle (example: Norin the Wary + Blade of Selves, #13179);
* Must be blocked if able - fixed that game can't continue without all available blockers (example: attacking with Menace, #13182);
* You may play an additional land - added card hint to all lands about played count and max limit (#13216);

## Card fixes
* Awakened Skyclave & Grond, The Gatebreaker - fixed that it doesn’t give a land type (#13229);
* Bello, Bard of the Brambles - improved combo support with Ashaya, Soul of the Wild (#13196, #13195);
* Caretaker's Talent - fixed wrong cost of level 3 ability;
* Feather, the Redeemed - fixed that it wrongly works with blinked objects (#13226);
* Gandalf of the Secret Fire - fixed that it wrongly works with blinked objects (#13226);
* Greymond, Avacyn's Stalwart - added card hint;
* Kassandra, Eagle Bearer - optimized dialogs logic for better UX;
* Leyline of Resonance - fixed that it triggering when targeting opponents' creatures (#13223);
* Light Up the Night dealing - fixed duplicated damage;
* Mangara's Tome - fixed that replacement effect doesn't stop after first use (#13188);
* Mirko, Obsessive Theorist - fixed wrong power checking (#13249);
* Pygmy Kavu - added card hint;
* Sharae of Numbing Depths - fixed that it trigger on controller's permanents too (#13176);
* Silent Hallcreeper - fixed wrong effect duration;
* Slinza, the Spiked Stampede - fixed wrong cost reduction effect (#13235);
* Tribute to the World Tree - fixed that it still draw a card if the creature has died before the ability resolves;
* Urza's Avenger - fixed that it put counters on itself (#13215);
* Vampire Gourmand - fixed wrong block restriction;
* Viral Spawning - fixed miss flashback (#13143);
* Zurgo and Ojutai - fixed that it triggering on all damage instead combat only (#13156);

## New cards
* Aetherdrift - added 116 new cards;
* Aetherdrift Commander:
  * On Wings of Gold
  * Prophet of the Scarab
  * Temmet, Naktamun's Will
  * Wizened Mentor
* Assassin's Creed:
  * Kassandra, Eagle Bearer
* Bloomburrow Commander:
  * Fisher's Talent
* Duskmourn: House of Horror:
  * Acrobatic Cheerleader
  * Cryptid Inspector
  * Kaito, Bane of Nightmares
  * Nowhere to Run
  * Unable to Scream
* Duskmourn: House of Horror Commander:
  * Disorienting Choice
  * Kianne, Corrupted Memory
  * Phenomenon Investigators
  * Rendmaw, Creaking Nest
* Fallout:
  * Cait, Cage Brawler
  * Curie, Emergent Intelligence
  * Yes Man, Personal Securitron
* Foundations Jumpstart:
  * Evereth, Viceroy of Plunder
  * Rev, Tithe Extractor
* Tales of Middle-earth Commander:
  * Gandalf of the Secret Fire

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)