---
layout: post
author: JayDi85
title: New card hints window
---
Last version added new helper tool - card hints dialog. 
It can be useful for many games to monitor some game 
conditionals like storm counter.

**More details on last update**

GUI - new card hints window features:
* new help window can be opened from a player panel;
* it collect and show all visible game hints from all players and all zones;
* it updates in real time on game update;
* allows to customize visible data;
* allows to open multiple windows (current limit is 5 windows, can be slow to render);
* allows to minimize opened windows;
* workable card popup on mouse move over card name or card id;
* filter modes:
    * all - show hints from all players;
    * player - show hints from single player;
* group mode:
    * by hints - show same hints as one with all used cards;
    * by cards - show full cards list with own hints;
* search mode:
    * allows to filter card hints by player name, card name, card id or card hint;
    * allows to search multiple words (equals to "or")
* current limitation:
    * card popup shows a card instead a real object, e.g. miss card hints in it (related to game logs problem);
    * unsupported of emblems, dungeons and other non card objects from a command zone;
    * unsupported of revealed and library's top cards;

GUI - player's panel improves:
* added hints helper button;
* added player highlight as possible target in choose dialogs;
* improved player name button in small mode;
* fixed wrong height in small mode;

Other fixes:
* game logs: added card popup support for logs with custom object name;

**Examples**

Card hint window with diff group and search modes:
![shot_231118_140743](https://github.com/magefree/mage/assets/8344157/dcedcb03-013a-4902-a512-0b613c9135bd)

Player highlight as possible target:
![shot_231118_134958](https://github.com/magefree/mage/assets/8344157/ebb503a6-ec29-4ede-ae6b-5a7ea5f0de37)

Improved name button in small mode:
![shot_231118_140520](https://github.com/magefree/mage/assets/8344157/c91161ce-cbae-4437-a64d-57a25a91ef98)

Please try new beta version in the [BETA server](http://xmage.today/) 
and report any bugs on [github](https://github.com/magefree/mage/issues).

If you like the project then you can support it by [donate on patreon](http://xmage.today/#donate).