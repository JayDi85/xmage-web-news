---
layout: post
author: JayDi85
title: 1000 new cards from OTJ, PIP, WHO and other
---
New release contains ~1000 new cards from OTJ, BIG, PIP, MKM, MKC, WHO and other sets.
It also includes new mechanics like Commmit Crime, Plot, Saddle and other.

Other fixes:
* images: added download support of meld cards (#11778);
* gui: deck editor - improved popup menu and lands dialog, added commander hint to sideboard;
* game: added 5-minute match timer option (#11925);
* game: removed public deck hash info;
* deck: fixed that Crusade was banned in Premodern;
* deck: fixed that Snow-Covered Wastes were not allowed as other snow-lands (#11938);
* deck: fixed wrong deck limit for Once More With Feeling;
* deck: improved xmage dck-files - now it correctly load a card's amount (related to files from third party services);
* server: improved server stability after some memory overflow errors (card not found errors, related to #11285);
* server: improved server stability and fixed game freeze on buggy triggers from cards like Nyxbloom Ancient (#11285, #8426);
* server: removed useless info message about disconnect stats, improved games/tourney stats;
* server: fixed bloated logs on user disconnections;
* server: fixed that new users can't connect to long living server (if it works too long without restarts, #11285);
* server: fixed wrong cheating warning on deck construction (#11877);
* other: improved admin tools (more tables info, auto-connection, fixed bugs, #5388):

Abilities fixes:
* Add counters abilities - fixed that it was able to wrongly add additional counter in rare use cases;
* Cards named xxx in your graveyard - added card hints (example: Compound Fracture, #11887);
* Face-down spells you cast - fixed that cost reduction applied to disguised cards (#11962);
* If you control commander - improved support with phased out commanders (example: Deflecting Swat, #12058);
* Mana triggered abilities - fixed duplicated or too much mana bugs in some use cases (#8426, #12087);
* Megamorph abilities - fixed that face down creatures show megamorph instead morph status (#11957);
* Permanents count - fixed that some cards ignore non-creature permanents (#7008);
* Priority on cleanup (discard triggers) - improved 514.3a rules support, multiple priorities works fine now (#12115, #12090);
* Return to battlefield transformed - fixed that it was able to return non-transformable cards (#12066);
* Suspend abilities - it's optional now due updated rules (#11892);
* Whenever one or more xxx deal damage - fixed that some cards was able to generate multiple triggers (#11943);
* Whenever xxx is dealt damage - fixed that some cards was able to generate multiple triggers (#11841, #12033);
* You may play, you may cast - improved support with other cards (example: Gonti, Lord of Luxury + Zoetic Cavern);

Card fixes:
* AAT-1 - fixed wrong trigger check (#12068);
* Aether Snap - fixed that it do nothing (#11988);
* Aspect of Manticore and Airtight Alibi - fixed that it's not granting their "to end of turn" effects (#11907);
* Basandra, Battle Seraph - fixed too long cast prevention effect (#11997);
* Cosmium Catalyst - fixed that it allow to choose spell instead random (#11933);
* Court of Locthwain - fixed that it's not allowing free cast of double-faced cards (#12073);
* Deep Gnome Terramancer - fixed that it's triggering out of extra lands played;
* Disorder in the Court - fixed that cards not return from exile (#9877);
* Faerie Mastermind - fixed wrong card hint (#11783);
* Jilt - fixed game error on usage (#12022);
* Judith, Carnage Connoisseur - fixed too long effects (#11917);
* Kairi, the Swirling Sky - fixed wrong targeting;
* Lara Croft, Tomb Raider - fixed that as though ability not properly scoped to controller (#11945);
* Laughtning Jasper Flint - fixed that trigger being not optional;
* Maddening Hex - fixed that it can attaching to dead players;
* Maestros Ascendancy - fixed not working cast from graveyard (#10403);
* Nahiri's Resolve - fixed delayed trigger;
* Norn's Decree and other cards - fixed wrong searching for defender players (#11921);
* Obeka, Splitter of Seconds - fixed that it adds upkeeps during combat (#12085);
* Ojer Axonil, Deepest Might - fixed that it doesn't check that the source is controlled (#12066);
* Ondu Rising - fixed wrong targeting (#11953);
* Opposition Agent - fixed that player can't play exiled cards after agent's death (#7405);
* Phyrexian Ingester - reworked;
* Qarsi Deceiver - fixed wrong playable calculation (#11956);
* Ral, Caller of Storms Planeswalker - fixed that it damages own creatures (#12112);
* Rampage of the Clans - fixed wrong triggers (#11959);
* Savvy Trader - improved exile zone info;
* Scurry of Gremlins - fixed wrong token;
* Serrated Arrows - fixed triggered ability;
* Shipwreck Sentry - fixed not working attack ability (#12022);
* Sigarda's Vanguard - fixed that it was wrongly affected by protection effects;
* Sludge Titan - fixed that it track milled cards in non-public zones too;
* Stampede Surfer - fixed wrong token;
* Structural Assault - added card hint;
* Vigil for the Lost - fixed not working die trigger (#11969);
* Wrathful Raptors - fixed wrong targeting by AI (#11960);

New cards and reprints for:
* OTJ: added ~370 cards from new set;
* OTC: added ~300 cards from new set;
* BIG: added ~90 cards from new set;
* PIP: added ~150 cards from new set;
* MKM: added ~90 cards from new set;
* MKC: 
  * Experiment Twelve, Showstopping Surprise, Counterpoint, Charnel Serenade, 
  * Kaust, Eyes of the Glade, Innocuous Researcher, Prisoner's Dilemma;
* WHO:
  * Me, The Immortal, Amy Pond, Rory Williams, Bigger on the Inside,
  * Reverse the Polarity, Sontaran General, Everything Comes to Dust;
* MH3:Ajani Nacatl Pariah;
* CLU: Unruly Krasis, Headliner Scarlett, Corporeal Projection;
* REX: Cresting Mosasaurus, Compy Swarm, Blue, Loyal Raptor, Henry Wu, InGen Geneticist;
* SLD: Rose Noble, The Fourteenth Doctor, The Meep;
* XANA: removed non-existing cards (#11915);
* PH17: Inzerva, Master of Insights;
* MAT: Ob Nixilis, Captive Kingpi;
* SCD: reprints;
* SLP: reprints;
* SPG: reprints;
* OTP: reprints;

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/) 
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](http://xmage.today/#donate).