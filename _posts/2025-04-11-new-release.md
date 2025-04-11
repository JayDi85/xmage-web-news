---
layout: post
author: JayDi85
title: AI and images download, Tarkir set and 350+ new cards
---
New release contains 357 new cards, most from Tarkir and Aetherdrift (including Omen, Mobilize and Harmonize mechanics), but also includes new cards from other sets like FIN, ACR, WHO and other. It also contains new combat rules without damage assignment order, fixes like scryfall images download, AI freezes, Rain of Riches's cascade and many other improves.

If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).

## AI and images download, Tarkir set and 350+ new cards
New release contains 357 new cards, most from Tarkir and Aetherdrift (including Omen, Mobilize and Harmonize mechanics), but also includes new cards from other sets like FIN, ACR, WHO and other. It also contains new combat rules without damage assignment order, fixes like scryfall images download, AI freezes, Rain of Riches's cascade and many other improves.

## AI
* fixed game freeze on cards with combat triggers (#13342);

## Other
* game: added new combat rules from Foundations release - no more combat damage assignment order (#13279);
* images: fixed images download from scryfall source;
* images: added many tokens from old and new sets, fixed miss images (#13492);
* deck: updated bans list;
* deck: updated deck's edh power level and integrated game changers to it (game changer usage set deck's max points to 20, #13483);
* GUI, game: added auto-skip of select blocker step if not blockers available (#13496);
* GUI, game: added auto-resize to new popup windows like reveal/graveyard (#4351, #12281);
* GUI, game: fixed game error in choose ability dialog on using CTRL and mouse wheel (#13148, #13186);
* GUI, lobby: fixed error on mouse move over some table headers (#13331);
* network: fixed that some players can be disconnected and immediately lose on mobile networks (#13155, 13390);

## Ability fixes
* Choose a player at random - fixed that it wrongly choose same player (example: Scrambleverse, #12679, #13526);
* Delve abilities - removed unnecessary windows with exiled cards (except few cards that can use it);
* Do if cost paid - otherwise effects not applied if cost cannot be paid (#13433);
* It's become a creature - improved combo support with other creature depended effects due mtg layers;
* Ninjutsu abilities - fixed that multiple invocation causes multiple damage and triggers (#13425);
* Suspend abilities - fixed that some cards can be unplayable in some use cases (example: Epochrasite, #13527);
* Suspend abilities - improved combo support with Gandalf of the Secret Fire (#13527);
* Suspend abilities - improved combo support with MDFC and adventure/omen cards (#13527);
* Ward abilities - fixed that it apply only once for multiple triggers instead multiple times (example: Roaming Throne, #13498);
* X cost abilities - fixed missing game logs and card icons in some use cases (#13516);
* X cost abilities - fixed that some cards ask to announce already defined X values (example: Bargaining Table, #13516);
* X cost abilities - fixed that some cards do not support combo with other cost modification effects (#13516);
* X cost abilities - fixed that some cards with ignore min/max limits for X (allow to choose any X, example: Scorched Earth, Open The Way, #13516);

## Card fixes
* Angelic Aberration - fixed that it used current PT instead base (#13478);
* Delney, Streetwise Lookout - fixed wrong trigger (#13241);
* Fanatic of the Harrowing - fixed that it discard by wrong players;
* Fecund Greenshell - fixed that it trigger on opponent creatures too (#13414);
* Fungal Plots - fixed useless exile window;
* Gastal Thrillroller - fixed not working return from graveyard (#13400);
* Gnostro, Voice of the Crags - added card hint;
* Grist, the Hunger Tide - added card hint (#13354);
* Hakim Loreweaver - fixed not working destroy ability;
* Inniaz, the Gale Force - fixed that it wrongly choose left/right player (#13526);
* Macabre Reconstruction - fixed wrong cost reduction;
* Minion of the Wastes - fixed wrong boost effect (same for Wood Elemental and Nameless Race);
* Mongrel Pack - fixed dies trigger;
* Mu Yanling, Wind Rider - fixed not working second ability (#13361);
* Nether Traitor - fixed that it doesn't trigger correctly (#13451);
* Noise Marine - added card hint;
* Not Dead After All - fixed that it moved cards by wrong player (#13365);
* Open The Way - fixed that it allow to choose any X without limits (#13516, #12810);
* Profound Journey - fixed that it can't target battle card type (#13377);
* Rain of Riches - fixed that it does not cascade (#9669, #13396);
* Season of Loss - added card hint (#13354);
* Songs of the Damned - added card hint (#13354);
* Sumala Sentry - fixed not working trigger (#13432);
* Sword of Dungeons and Dragons - simplified code and replaced golden color token by all colored token (#13470);
* The Aetherspark - fixed that it able to be targeted when attached to a creature (#13430);
* The Aetherspark - fixed that it can't activate abilities when not controlling any creatures (#13462);
* Unbound Flourishing - improved combo support for activated abilities with predefined X mana costs like Bargaining Table (#13516);
* Unmoored Ego - fixed that exile cards choice is not optional (#13349);
* Veiled Apparition - fixed miss flying ability;
* Volatile Stormdrake - fixed that it can skip sacrifice part in some use cases (#13307);
* Volcanic Torrent - added card hint;
* Webstrike Elite - fixed not working triggered effect from cycling (#13401, #13397);

## New cards
* Tarkir: Dragonstorm - added 245 new cards;
* Tarkir: Dragonstorm Commander - added 28 new cards:
* Aetherdrift - added 38 new cards;
* Aetherdrift Commander:
  * Hashaton, Scarab's Fist
  * Lost Monarch of Ifnir
  * Nissa, Worldsoul Speaker
  * Pia Nalaar, Chief Mechanic
  * Priest of the Crossing
  * Rampaging Aetherhood
  * Renewed Solidarity
  * Saheeli, Radiant Creator
  * Stridehangar Automaton
  * Territorial Aetherkite
* Assassin's Creed:
  * Alexios, Deimos of Kosmos
  * Brotherhood Headquarters
  * Haytham Kenway
  * Layla Hassan
  * Overpowering Attack
  * The Aesir Escape Valhalla
  * Viewpoint Synchronization
  * What Must Be Done
* Bloomburrow Commander:
  * Evercoat Ursine
* Doctor Who:
  * Bill Potts
  * Ensnared by the Mara
  * Fugitive of the Judoon
  * Peri Brown
  * The First Doctor
  * The Girl in the Fireplace
  * The Night of the Doctor
  * The Second Doctor
  * The Sound of Drums
  * This Is How It Ends
  * Wilfred Mott
* Duskmourn: House of Horror Commander:
  * Suspended Sentence
  * Ursine Monstrosity
* Fallout:
  * Strong, the Brutish Thespian
* Final Fantasy:
  * Jumbo Cactuar
  * Sazh's Chocobo
  * Sephiroth, Planet's Heir
  * Sin, Spira's Punishment
  * Stiltzkin, Moogle Merchant
  * Summon: Shiva
  * Tonberry
* Final Fantasy Commander:
  * Celes, Rune Knight
  * Cloud, Ex-SOLDIER
  * Terra, Herald of Hope
  * Y'shtola, Night's Blessed
* Masters Edition II:
  * Goblin Ski Patrol
* Ravnica: Clue Edition:
  * Suppressor Skyguard
* Total cards: 357

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)