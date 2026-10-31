---
layout: post
author: JayDi85
title: Improved drafts and AI, images download, animations and 268 new cards like Star Trek
---
New release introduces improved drafts with pick suggestions and better AI, better images download and card animations. It also contains 268 new cards from Star Trek and other sets and includes over 200 fixes in existing cards and abilities.

Thank you for supporting the project and the server! Your support makes updates like this possible.

💪 Here are some awesome stats from the previous update with the network rework:

<img width="640" height="500" alt="XMage async update results" src="https://github.com/user-attachments/assets/90d9864a-8ada-469a-9f3c-3cada6c025cd" />

😍 If you like the project, you can [support it on Patreon](https://xmage.today/#donate).

🛠️ If you find any bugs or have ideas for new features or changes, report them on [GitHub](https://github.com/magefree/mage/issues).

## Draft improvements
* other: new card ratings, integrated with real human data from https://www.17lands.com (#16659)
* draft: added pick suggestions based on 17Lands (deck editor shows top 3 cards for the pick based on your current deck/colors and ratings);
* draft: added card auto-picks on missed submit or timeout;
* draft: added deck auto-construct on missed submit or timeout;
* GUI: new card ratings used all around now (card viewer, deck editor, AI bots, auto-picks, pick suggestions, etc.);
* GUI: improved land suggestion dialogs with hybrid colors support, better lands/colors distribution and more;
* AI: draft bots improved, now they select cards like real people do and can change deck colors in the middle of the draft;
* AI: fixed dozens of bugs with deck construction (wrong picks, wrong colors, wrong lands, wrong mana curve and creature amount);
* other: fixed wrong card order in some boosters;

## Animations improvements
* improved battlefield cards drawing and animation, better stability and performance, no more memory leaks (#16624);
* now it's smooth and supports massive actions and updates like AI vs AI games (#16624);
* fixed dozens of bugs with freezes, random errors and wrong clicks (#16624);

## Images download improvements
* improved download stability and fixed dozens of bugs (#16622);
* improved work with zip files, including fixed freezes and unsaved data bugs (#16622);
* faster tokens download;
* better Scryfall support including protection from IP bans and rate limits;
* better progress and error processing, no more download stops on bad cards/sets;

## Other
* app: added default graphic settings for better stability on NVIDIA cards (#4626, #16458);
* app: improved app stability in images download and preferences change;
* game: fixed missing commander damage info on some double-faced permanents (#16647);
* boosters: fixed missing rarity slots in 30A, SWS, MH3 (#16370, #16440);
* boosters: fixed draft freeze on BRO boosters usage;

## Abilities fixes
* Payment cancel - fixed that some spells can lose activation status on impossible payment or cancel (example: Convoke, Delve, Improvise, #16509);
* Sneak abilities improvements:
  - fixed that it doesn't enter tapped and attacking (#14975, #14895);
  - fixed that it doesn't work from instant/sorcery;
* Target becomes creature abilities:
  - improved layers and combo support, fixed dozens of cards (#16464);
  - fixed that target permanent keeps old creature types instead of replacing them (example: Secret Identity, #16455);
  - fixed that it loses non-creature subtypes like Equipment or Clue (example: Scale Up, Living Brain);
  - fixed that it loses color on lost abilities (example: The Curse of Fenric);
  - fixed that "artifact creature" doesn't replace old creature types (example: The Mechanist, Aerial Artisan);
* Batch events improvements (one or more):
  - improved many cards and combo support, no more double or missed triggers (#16506);
  - "Don't cause abilities to trigger" effects - fixed that it can't stop some "one or more" triggers (example: Torpor Orb, #10335, #16506);
  - "One or more" triggers - fixed that it can trigger only once instead of multiple times in multi-step effects (example: Pox, Balance, Magus of the Balance, Restore Balance in combo with Titania, Voice of Gaea, The Gitrog Monster, #16506);
  - Triggers an additional time - added combo support with "one or more" and "put onto the battlefield" triggers (50+ cards like Panharmonicon with Ingenious Artillerist, #13455, #10335);
* Additional costs - fixed that some abilities with additional costs can lose activation status on payment cancel or no possible targets (example: Convoke, Blitz, etc);
* Attacking that player - fixed that it wrongly asks the defender to attack (example: Capricopian);
* Gift abilities - fixed game error on usage with Convoke and other non-mana costs;
* Mana abilities - improved 605.1a support, abilities with card zone moves aren't mana abilities anymore (example: Selvala, Explorer Returned, #15876, #16054);
* Melded permanents - improved combo support, now it can't be turned face down (rule 712.16, #16562);
* Party count and roles - fixed game error on cards with same multi-roles, fixed cards count without roles (#8138);
* Phased-out permanents - improved layers and combo support (example: Explore and Connive triggers without counters, #16561, #16576);
* Redirect effects - improved combo support and legality check (example: Kor Dirge and Kor Chant, #16426);
* Tapped and attacking - fixed that entering tokens was able to choose battle permanents (example: Adeline, Resplendent Cathar and Caller of the Pack, #11230);
* This spell can't be copied - fixed that it was never applied (example: Choreographed Sparks, #16479, #16521);

## Cards fixes
* Age of Ultron - fixed that it was only destroying targets for the first opponent;
* Amzu, Swarm's Hunger - fixed that it can use mana value of opponent's cards when graveyards are exiled at the same time (example: Relic of Progenitus);
* Beast, Erudite Aerialist - fixed flying for copies of Beast (#16478, #16522);
* Cloud, Midgar Mercenary - fixed dies triggers of attached Equipment (#16621);
* Deep Gnome Terramancer - fixed that it triggers multiple times instead of once when several lands enter at the same time (e.g. by Field of Ruin or Circuitous Route, #10088);
* Deepway Navigator - fixed that Merfolk don't get +1/+0 after you attacked with three or more Merfolk (#16481);
* Elesh Norn, Mother of Machines - fixed game error on one or more triggers like dies (#15231, #10335, #11895);
* Emergent Haunting - fixed type/color handling, e.g. keep Enchantment (#16452);
* Firdoch Core - fixed that it loses all creature types (changeling) while it's an artifact creature (#16454);
* Fire Lord Ozai - fixed playing more than one exiled card (#16618);
* Grizzlegom, Hurloon Hero Rulebreaker - fixed removing the maximum deck size (#16519);
* Hurkyl, Master Wizard - fixed that it allows for targeting of incorrect cards (#10116);
* Ingenious Artillerist - fixed wrong damage when artifacts enter under multiple players' control at the same time (example: Kibo, Uktabi Prince);
* Irma, Part-Time Mutant - fixed that it wasn't copying the copiable values of a copy (#16619);
* Juxtapose, Tariff - fixed game error when choosing among tied permanents (#16436, #16437);
* Lifecraft Engine - improved layer/combo support with become creatures (#16484);
* Myriad ability - fixed that auto-answer doesn't work (#12845);
* Maskwood Nexus - fixed that it doesn't grant all creature types to crewed vehicles that become Creatures;
* Mindlink Mech - fixed game error on usage, fixed that it triggers every time instead of the first time each turn (#10479);
* Nefarious Imp - fixed that it can trigger multiple times when permanents leave the battlefield to different zones at the same time (example: unearthed creature or commander);
* Ninja Teen - fixed that it doesn't work with MDF cards;
* Polluted Cistern - fixed that it can count card types of opponent's cards when each player mills at the same time (example: Unseal the Necropolis);
* Pox, Balance, Magus of the Balance, Restore Balance - fixed that "one or more" triggers can trigger only once for multiple steps (e.g. Titania, Voice of Gaea, The Gitrog Monster);
* Ramses, Assassin Lord and Blood Tyrant - fixed not triggering when a player loses (#16598);
* Sarkhan, Dragon Ascendant - fixed type/color handling, e.g. keep Human Druid (#16452);
* Seer of Stolen Sight - fixed that it doesn't trigger on dying or sacrificed tokens (example: creature tokens, Treasure, Clue);
* Spider-Slayer, Hatred Honed - fixed that its ability can't be activated from the graveyard (#16496);
* Sugar Coat - fixed type/color handling, e.g. apply color change (#16452);
* Swat Away - fixed that cost reduction was never applied (#16495);
* Tannuk, Steadfast Second - fixed that warped double-faced cards weren't exiled (#15584, #16620);
* Veteran Survivor - fixed that it doesn't get +3/+3 and hexproof with three or more cards exiled with it (#16482);
* Woodland Champion, Cloakwood Swarmkeeper, Ingenious Artillerist - fixed that Torpor Orb, Elesh Norn and other effects can't stop them from triggering (#10335);
* Xanathar, Guild Kingpin - fixed spending mana as any color after the first card (#16617);

## New cards
* Total new cards: 268;
* Star Trek - added 150 new cards;
* Star Trek Commander - added 82 new cards;
* Assassin's Creed:
  * Apple of Eden, Isu Relic
  * Auditore Ambush
* Darkhold Destiny Commander:
  * Gargantos, the Endbringer
* Marvel Super Heroes Commander:
  * Avenge
  * Fight for the Throne
  * Heart-Shaped Herb
  * Heroic Return
  * King Solomon's Frogs
  * M'Baku, Jabari Chieftain
  * Okoye, Mighty and Adored
  * Origin of Iron Man
  * Panther Habit
  * Silver Surfer, Galactus's Herald
  * Storm, Queen of Wakanda
  * The Spear of Bashenga
  * Thor, Asgard's Avenger
  * W'Kabi, Shield of the Nation
* Marvel: Darkhold Destiny:
  * Magik, Illyana Rasputin
  * Penance Stare
  * Rise from the Nether
  * The Darkhold
* Mystery Booster Commander Edition:
  * Grakk the Pacifist
  * Sifa Grent
* Reality Fracture:
  * Command the Stage
  * Grim Repriser
  * Hapatra, the Desert Fang
  * Hapatra, the Desert Frost
  * Kiora of Salt and Sand
  * Tetsuko Umezawa, Pursuer
  * Vindictive Triumph
  * Way of the Mind Sculptor
  * Whiplash Wordsmith
* Reality Fracture Commander:
  * Tamiyo, Upriser Crowned
  * The Ur-Sphinx
  * Venser, Fervent Forger
* Teenage Mutant Ninja Turtles Eternal:
  * Casey & Raph, Hotheads

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/)
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)