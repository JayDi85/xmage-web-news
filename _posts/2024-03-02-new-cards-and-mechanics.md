---
layout: post
author: JayDi85
title: Face down reworked and hundreds of new cards
---
New release contains ~450 new cards from PIP, MKM, MKC, CLU and other sets. It also includes new mechanics like Disguise.

Face down cards reworked:
* gui: added special images for face down cards like Morph, Manifest, etc (download it as normal tokens);
* gui: added day/night button to view a real card for controller/owner;
* gui: improved game logs - now it contains a workable object reference (it can be opened with card popup hint like normal card logs);
* game: fixed that faced-down card can render symbols, abilities and other hidden data from a real card;
* game: improved combo support with many cards like MDFC, split, adventure, etc (#11873);
* ![shot_240302_204958](https://github.com/magefree/mage/assets/8344157/2deb37eb-0027-4b7a-bf2d-244766770e66)

Improved rendering of some non-standard cards:
* gui: improved Saga cards (#11762);
* gui: improved Adventure cards (#11764)
* gui: improved Class cards (#11767)
* ![image](https://github.com/magefree/mage/assets/1636645/0a565d2e-8483-4e3d-ba25-3edfddeb740a)

Other fixes:
* images: added tokens for LCC, RVR, MKM, MKC;
* images: no more needs in client restart to apply newly downloaded images or render settings;
* images: improved backface image quality (use main menu -> symbols to download it);
* images: fixed missing tokens from DDD set;
* images: fixed missing images download from SLD and other sets (#11883);
* gui, card viewer: added special set to view all special tokens like face down (XMAGE);
* gui, cards: added missing image info in card popup hint (now it works in any render mode);
* server: improved server stability and fixed bloated logs about game timer;
* AI: fixed wrong timer in computer games;

Abilities fixes:
* Copy abilities - improved stability and cards support;
* Modal double-faced cards - improved support, no more other side effects on battlefield;
* Player under control - improved stability and related cards support (possible NPE errors, additional runtime checks);
* Storm abilities - added card hints with storm counter (#11795);
* Train and Mentor abilities - fixed that it triggers without really put a +1/+1 counter (example: Savior of Ollenbock, #11718);

Card fixes:
* Amend Case of the Shifting Visage - added card hint;
* Blinkmoth Urn - fixed that it's triggering while tapped;
* Eldritch Pact - fixed wrong target choose (#11736);
* Mob Rule - fixed buggy control effect (#11811);
* Myojin of Grim Betrayal - fixed that ability doesn't work with non-battlefield zones (#11721);
* Neyali, Suns' Vanguard - improved exile zone;
* Polygraph Orb - added card hint;
* Shimmer Dragon - added card hint;
* The Enigma Jewel - fixed wrong searching for activated abilities (#11832);
* Training Grounds - improved choices;
* Warden of the Eye - fixed that it has broken in AI games;
* Wayta, Trainer Prodigy - fixed wrong cost reduction (#11782);
* Zombie Mob - fixed wrong trigger;

New cards and reprints for:
* PIP: added ~200 cards from new set;
* MKM: added ~70 cards from new set;
* MKC: added ~50 cards from new set;
* CLU: added ~30 new cards and ~250 reprints;
* ACR: Eivor, Battle-Ready, Haystack, Ezio, Blade of Vengeance;
* ANB: Baloth Packhunter, Compound Fracture, Hallowed Priest, Mardu Outrider, Tin Street Cadet;
* BIG: reprints;
* BLB: Mabel, Heir to Cragflame, Bria, Riptide Rogue, Lumra, Bellow of the Woods, Byrke, Long Ear of the Law;
* ICE: Arcum's Sleigh;
* MH3: Psychic Frog, Scurry of Gremlins, It That Heralds the End, Flare of Cultivation, Snow-Covered Wastes;
* MIR: Torrent of Lava, Acidic Dagger;
* OTJ: Hell to Pay;
* REX: Dino DNA;
* SLD: Lara Croft, Tomb Raider;
* WHO: TARDIS;

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/) 
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](http://xmage.today/#donate).