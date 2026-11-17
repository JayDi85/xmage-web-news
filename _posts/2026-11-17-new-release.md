---
layout: post
author: JayDi85
title: New cards from top 100 commander decks, tons of fixes and 67 new cards
---
New release adds all long waiting cards from top 100 commander decks like Jace, Multiverse Architect and other ~70 new cards. It's also contains the biggest pack of fixes for abilities and cards (affected over 500+ cards and abilities).

<img width="536" height="181" alt="new-cards" src="https://github.com/user-attachments/assets/aa879be9-7848-47ca-af12-a087c5ed5012" />

😍 If you like the project, you can [support it on Patreon](https://xmage.today/#donate).

🛠️ If you find any bugs or have ideas for new features or changes, report them on [GitHub](https://github.com/magefree/mage/issues).

## Other
* deck: added some new promo sets and SLD cards;
* game: fixed that cards and effects still counted or affected opponents who left the game (example: Blazing Sunsteel, Araumi of the Dead Tide, Encore, #13289, #16724, #16743);
* game: fixed that some cards can choose players who left the game (example: Black Vise, Fact or Fiction, Hithlain Rope, #16752);
* GUI, game: fixed client error on emblem or dungeon usage in dialogs with m15 card render mode (example: trigger order with Liliana's emblem, #15972);
* GUI, game: fixed random errors on card popup usage (#11612);

## Ability fixes
* Auras put onto the battlefield by effects - fixed that double faced aura weren't attached or allowed to choose (example: Storm Herald, Aura swap, #13819, #14977);
* Auras put onto the battlefield by effects - improved combo support with flickers and wrong attachment dialog (example: Retether then Replenish);
* Balance - fixed that players who left the game count as having nothing (#16731);
* Becomes a copy - fixed that the returned permanent became a copy after a blink in response to its copy ability (example: Absorbing Man, Protean Thaumaturge, Crystalline Resonance, Artisan of Forms);
* Convoke multitapping and other alternative mana payment rework and improvements (#16508);
* Copy a spell or ability for each it could target - fixed that it can be copied with non-legal targets (example: Soul's Fire on Ink-Treader Nephilim, 707.10d support);
* Copy abilities - fixed that some cards can wrongly target spells on stack (example: Lithoform Engine, Adric, Mathematical Genius, Vantress Visions and others, #12005, #12706);
* Copy effects - improved combo support with copy of copies (example: Permeating Mass, #14116, #10801, #16746);
* Copy effects - improved compatibility with double faced cards (fixed game errors like Fractured Sanity, #16429);
* Entering attacking - fixed that some effects wrongly prevent it (example: Mirri, Weatherlight Captain and Judoon Enforcers, #14115, #10234);
* Enters with counters effects - fixed that double-faced cards enter without counters (Graceful Restoration, Planar Incision, Feign Death, Ghost Vacuum and other);
* Morph - fixed game error on face down cast of Aura cards (example: Gift of Doom, #15580);
* Prepare and Vengeance cards - fixed that a prepare / vengeance spell can be cast by cast without paying its mana cost effects (example: cascade abilities);
* Prepare cards - fixed that an old prepared spell copy stays in exile and can be cast after the creature returns to the battlefield (example: blink);
* Put into graveyard this turn - fixed that it doesn't work with double-faced cards (example: Faith's Reward, Activated Sleeper, Banon and other 20+ cards);
* Put to battlefield effects - better compatibility with double faced cards (example: Aetherplasm, Push // Pull, and other);
* Scry - fixed that it can wrongly raise triggers on scry 0 (example: Graven Lore);
* Spell costs less to cast - fixed that some spells wrongly show playable status (Focus the Mind, Gigastorm Titan and other);
* Until the end of your next turn - fixed that it can't be used during the end step of your next turn (example: Commune with Lava);
* Whenever activates an ability triggers - fixed that triggers doesn't see activates of mana abilities (example: Avalanche of Sector 7, #14026);

## Card fixes
* Activated Sleeper - fixed that it doesn't get Phyrexian type as a copy;
* Aminatou's Augury - fixed that it asks for the card type while processing the cast event (#16750);
* Aminatou's Augury - fixed that it can't cast transforming cards or modal back faces, shares used card types when cast again in the same turn and uses up card types on cancelled casts (#15838, #14878, #16723);
* Angelic Enforcer - fixed that a negative life total is not doubled;
* Angrath, Minotaur Pirate - fixed that -11 ability doesn't destroy creatures and deals no damage;
* Arachnus Spinner - fixed that it asks for a creature to attach Arachnus Web to instead of using the target creature;
* The Argent Etchings - fixed making Incubators trigger Phyrexian enter abilities (#16667);
* Arni Metalbrow - added choose card hint with attacker info (#16732);
* Artifact Possession - fixed that it doesn't trigger from abilities without {T};
* Azor, the Lawbringer - fixed that it restricts the current turn instead of the opponent's next turn when it enters during an opponent's turn (#4570);
* Battlemage's Bracers - fixed that an ability of the equipped creature was copied when that creature was sacrificed as a cost;
* Battle Angels of Tyr - fixed that it not creating a Treasure (#9829, #16666);
* Bolg's Company - fixed that its mana ability used the stack (#16687);
* Boom Scholar - fixed cost reduction (#16736);
* Bounty of the Deep - fixed that it seeks two cards as two separate actions (Val, Marooned Surveyor triggered twice);
* Breathkeeper Seraph - fixed that it returns creatures on any player's next upkeep instead of yours and can return a creature that left the graveyard;
* Bruna, Light of Alabaster - fixed game error with double faced Auras;
* Bull-Rush Bruiser - fixed that it ignores Warriors in some use cases;
* Cass, Hand of Vengeance - fixed that it doesn't return double faced Auras;
* Darkblade Agent - added card hint;
* Demonic Gifts - fixed that it can return a creature that died again as a new object (#16465);
* Destined Confrontation - fixed that nothing was sacrificed under limited range of influence (#16689);
* Dimir Strandcatcher - fixed that it counts all opponents instead of attacked ones;
* Driftgloom Coyote - fixed that it never got the counter (#16693);
* Emeritus of Woe - fixed wrong rules text;
* Exterminator Magmarch - fixed that it can copy the spell to a permanent the spell can't target (example: a creature with hexproof);
* Flickerform - fixed that it doesn’t return double faced creatures and Auras;
* Gerrymandering - fixed that it doesn't work with double faced and mutated cards (#16795, #16721);
* Ghastlord of Fugue - fixed wrong player in the game log message about the exiled card;
* Gogo, Master of Mimicry - fixed that copy ability can target spells (#12706);
* Haphazard Bombardment - fixed that it never destroys permanents with aim counters;
* Henzie "Toolbox" Torre - fixed that blitz doesn't work with double-faced cards (#16733);
* Henzie "Toolbox" Torre - fixed that it doesn't give blitz to creature spells with {X} (example: Walking Ballista with X=2);
* Icehide Golem - fixed that its reminder text counted as an ability (#16707);
* Illusionist's Bracers - fixed that an ability of the equipped creature was copied when that creature was sacrificed as a cost;
* Joined Researchers - fixed that it doesn't become prepared at opponent's end step;
* Jukai Liberator - fixed that it can seek nonpermanent cards like instants;
* Kezzerdrix - fixed that it deals damage to you even if your opponents control creatures;
* Lashwhip Predator - fixed that its cost reduction never works;
* Lorehold Archivist - fixed wrong rules text;
* Loot, the Pathfinder - fixed that its exhaust mana ability used the stack and can be copied by cards like Pit Automaton (#16477, #16736, #16793);
* Ludevic, Necrogenius - fixed that Olag doesn't become a copy of exiled card and doesn't get +1/+1 counters;
* Magus Lucea Kane - fixed that a mana ability with {X} in its activation cost didn't use up its delayed trigger;
* Muldrotha, the Gravetide - fixed that it asks for the card type while processing events (#16779);
* Myth Unbound - fixed that it didn't draw when the commander was put into the command zone from graveyard, exile or the stack (#16708);
* Nimble Obstructionist - fixed that it can counter spells (#12706);
* Norman Osborn - fixed that Goblin Formula's mayhem missed cards discarded before it applied (#16762);
* Oracle en-Vec - fixed that in multiplayer the chosen creatures were destroyed at the end of the next player's turn instead of the target opponent's turn (#13980);
* Oracle en-Vec - fixed that a chosen creature was destroyed after it left and returned to the battlefield;
* Pain for All - fixed that no damage was dealt if the enchanted creature died from the damage (#16695);
* Peter Parker's Camera - fixed that copy ability can target spells (#12706);
* Planeswalker's Mischief - fixed that it not returning uncasted to hand (#16753);
* Primitive Etchings - fixed that the first card you draw is not revealed and doesn't trigger on other players' turns;
* Promise of Loyalty, White Sun's Twilight, Tsabo's Decree, Fog Patch, Extinction, Sunspine Lynx, Riptide Chronologist - fixed that it doesn't work in games with limited range of influence;
* Radiant Grace - fixed that it doesn’t return to the battlefield transformed attached to an opponent (#9687);
* Reborn Hero - fixed that it returns under its owner's control instead of yours and can return a card that left the graveyard;
* Revival // Revenge - fixed that a negative life total is not doubled;
* Rocket-Powered Goblin Glider - fixed that it not attaching when cast from graveyard (#14017, #16674);
* Rowen - fixed that the first card you draw is not revealed and doesn't trigger on other players' turns;
* Sage of Ancient Lore - fixed that back face dying as a 0/0 on transform (#16587);
* Scheming Silvertongue - fixed wrong rules text;
* Sphinx's Decree, Azor, the Lawbringer - fixed that opponents can't cast instant and sorcery spells in later turns too, not only during their next turn;
* Steward of the Harvest - fixed wrong abilities of your creatures after a land card left exile or after a turns rollback;
* Storrev, Devkarin Lich, Kagha, Shadow Archdruid, Maralen, Fae Ascendant, Voltaic Visionary - fixed that it doesn't work with double-faced cards;
* Takklemaggot - fixed that it can't return as a non-Aura enchantment;
* Tawnos’s Coffin - fixed that it doesn’t return double faced creatures and Auras, fixed that it returns a creature untapped;
* Tezzeret, Betrayer of Flesh - fixed that mana abilities and sacrificed artifacts don't use up the cost reduction;
* Thieves' Auction - fixed that it doesn't work with double faced and mutated cards (#16795, #16721);
* The Spot, Living Portal - fixed wrong filter;
* Twinblade Geist - fixed game error on cast with disturb (#16071, #16073);
* Unbound Flourishing - fixed that it didn't trigger on mana abilities with {X} in their activation cost (there is nothing to copy);
* Urborg Stalker - fixed that it never deals damage to opponents on their upkeep;
* Whtz - fixed that is not playable unless you have three open mana instead deck size 200 checking (#16726);
* Wyll's Reversal - fixed that it forgetting to pass target filter, fixed roll (#16757, #14072);

## New cards
* Total new cards: 67;
* Alchemy: Edge of Eternities:
  * Val, Marooned Surveyor
* Commander Legends: Battle for Baldur's Gate:
  * Windshaper Planetar
* Marvel Super Heroes:
  * Political Triumph
  * Robot Domination
  * Taskmaster, Mercenary Mimic
* Marvel Super Heroes Commander:
  * Archnemesis
  * Daredevil, Fearless Fighter
  * Doom's Time Platform
  * Extract Power
  * Flying Drone
  * Galactus, Devourer of Worlds
  * Glorious Purpose
  * H.E.R.B.I.E., Lovable Robot
  * Intrepid Ace
  * Iron Monger, Sadistic Tycoon
  * Kang Dynasty
  * Lady Loki, Agent of Chaos
  * Living Laser
  * Loki, the Deceiver
  * Mister Immortal
  * Rhino, Terrible Trampler
  * Sauron, Dino Devotee
  * Scarlet Witch, Chaotic Avenger
  * Typhoid Mary, Fractured
  * Ultron, Unlimited
* Marvel: Darkhold Destiny:
  * Hela's Arcanum
  * Hela, Mistress of Darkness
  * Temple of Khonshu
* Murders at Karlov Manor Commander:
  * Eye of Duskmantle
  * Feather, Radiant Arbiter
  * Immortal Obligation
* Nauctis: The Sunken Realm:
  * Abyssal Lotus
  * Calmwater Mentor
  * Ring of Unity
  * Salinae, the Ocean Mother
  * Shimmering Citadel
  * Tecton, Malignant Ruin
* Reality Fracture:
  * Jace's Machinations
  * Sanctum Lurker
  * Uldaros Theorix
* Reality Fracture Commander:
  * Dack Fayden, Helping Hand
  * Jace, Multiverse Architect
  * Jhoira, Weatherlight Corsair
  * Teferi's Reproach
* Star Trek:
  * D-7 Battle Cruiser
  * Deep Space 9
  * Georgiou, Terran Emperor
  * L'Rell, Fierce Visionary
  * Lieutenant Commander Data
  * Live Long and Prosper
  * Romulan Bird-of-Prey
  * Salt Vampire
  * Sarek, Federation Ambassador
  * Storied Veteran
  * The Destruction of Praxis
  * U.S.S. Voyager, Lone Wanderer
* Star Trek Commander:
  * Borg Incursion
  * Commander Spock
  * Giant Space Amoeba
  * U.S.S. Defiant, Mirror Migrant
  * Voq, Torchbearer
* The Hobbit:
  * Azog, Moria's Ruin
  * Elrond, Moon-Reader
  * Woodland Weavemaster
* Transformers:
  * Blaster, Combat DJ
  * Prowl, Stoic Strategist
  * Soundwave, Sonic Spy

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)