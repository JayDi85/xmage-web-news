---
layout: post
author: JayDi85
title: Network improved, reconnection mode and new cards
---
Most important changes: new reconnection feature. Now users can safely restart 
app and reconnect to the server without game lost and after IP changes (after proxy/vpn/wifi/router restart).

If you catch any problems with miss data, random disconnects, 
empty decks, not started game/tourney, empty battlefield, etc 
then report it to [that special github issue](https://github.com/magefree/mage/issues/11526).

Also, new release contains dozens new cards and reprints for:
* SLD, LCC, CLU, MKM;
* MIR: Implement Tainted Specter, Sand Golem, Mangara's Blessing, Mangara's Equity;
* ICE: Implement Hipparion;

![shot_231204_160817](https://github.com/magefree/mage/assets/8344157/fed279b1-f00f-49a3-a6c2-c04f4fe901ee)

Network upgrade and new reconnection mode:
* users can disconnect or close app without game progress loose now;
* disconnect dialog will show active tables stats and additional options;
* all active tables will be restored on reconnect (tables, tourneys, games, drafts, sideboarding, constructing);
* user must use same server and username on next connection;
* there are few minutes for reconnect until server kick off a disconnected player from all player's tables (concede/loose);
* now you can safety reconnect after IP change (after proxy/vpn/wifi/router restart);

Other improvements and fixes:
* gui: cards - added restriction card icon with details info about all sources;
* ![shot_231202_235152](https://github.com/magefree/mage/assets/8344157/759a8d6a-9f10-437a-85ba-f191e21e14f6)
* gui: main menu - improved switch panel button, added stats about current tables/panels;
* gui: improved data sync and updates (fixes many use cases with empty battlefield, not started games/drafts/tourneys, not updatable drafts, etc);
* gui: improved main and battlefield menus (better naming, allow to view AI opponent's deck);
* other cards and qol fixes;

Full change history available on GitHub as [commits history](https://github.com/magefree/mage/commits/) 
or as [wiki page](https://github.com/magefree/mage/wiki/Release-changes)
If you find any bugs or has ideas on new features or changes then report it on [github](https://github.com/magefree/mage/issues).

If you like the project then you can [support it by patreon](https://xmage.today/#donate).