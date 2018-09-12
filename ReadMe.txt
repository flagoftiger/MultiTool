MultiTool:ReadMe          v7.1.0.001        2016/12/28          DigitalSorceress

SUMMARY
MultiTool: A set of tools to help make Multi Boxers lives a bit easier.


HISTORY / INSPIRATION
As someone who dual / triple boxes all the time, I have found a lot of little bits and pieces in the addon world that help take some of the drudgery out of multiple invites, turnins, quest gossips, yada yada. Often times, I find I am installing a whole addon just for one small feature, leading to a lot of overhead. I decided that Enough is enough.

This addon was inspired by Smurfy's MultiBox v2 which has a great collection of really useful stuff. If MultiBoxer was Ace3 or used a more lightweight approach, I'd probably just contribute and/or make a fork. Instead, I've decided to try my hand at a ground-up, exactly-what-I-want, lightweight Ace3-based addon.

I'd also like to acknowledge "Zanthor's Quest Broadcaster" for giving me a road map for quest gossip cloning.


ABOUT 'MASTERLESS' TOOLS
A lot of the available addons for multi boxers seem to use the concept of a "master".. Makes sense I suppose, after, all, you tend to play one toon (master) and have all the others (slaves) follow you and do stuff when your master does.

This is all well and good, but I often find that when not in combat, (quest pickup/turnin, flight masters, etc...) I may want to be taking lead on a different toon. (cuz I happen to be on that mouse/kbd for some reason).

So, I designed a system for flightmasters and quest givers where all you do is open the npc dialog on all your toons, then pick the option on ANY ONE and the others follow you.

NOTE: I deliberately do NOT clone quest reward choices on the grounds that I run three different classes and want to pick that myself. I may put in an option for "total clone" where that is allowed, but for now, you gotta pick your rewards manually.


FEATURE ROAD MAP
I've got a LOT of little things I'd like to do with this addon over time. Some of these may be impractical or not really end up being what I wanted. They are listed here somewhat in the order I want to build them in.

* Warn on losing AutoFollow - Implemented v0.3.05
  This was due to a suggestion from jst-one from www.dual-boxing.com forums
  
  The Party Options config is starting to get kind of big... may need to re-think that a bit

* Auto Accept Resurrect - Implemented v0.3.04
  Adding config options and event handling

* Custom Sounds - Implemented v0.2.05
  Customizable warning sounds for various events

* BLIZ Addon Config compatible - Implemented v0.1.02
  Will properly integrate into the new Blizard addon configuration pages

* Profile support - Implemented v0.2.04
  Will use profile-type system to allow for easy customization per toon/account

* WhiteList - Implemented v0.2.04
  define one or more toons in a list for use in invites, taxi following, auto trade, etc that require a high degree of trust (More than just general friends list) Possibly define permissions (canAutoTrade, canChooseTaxi, canAutoInvite, etc...)

* Auto Deny duel requests - Implemented v0.1.02
  Maybe MAYBE allow whitelist to request dual - though dueling dualboxers seems a bit Freudian to me

* Inviter - Not Started
  Attempt to invite all those on your white list with one click

* Taxi Dispatcher - Implemented v0.1.03
  Allows other toons in your group with the addon to automatically take the same taxi node as you

* Quest Log Full alert - Implemented v0.2.00
  Some kind of sound/warning to other members of group with addon if a toon's quest log is close to full

* Bags full warning - Implemented v0.2.00
  Some kind of sound/warning to other members of group with the addon that bag space is low/empty

* LootSetter - Not Started
  Automatically set party loot to FFA when leader and party consists only of those on your ffa list. When adding members NOt on your list, switch to Group Loot

* Auto Accept Group Invite - Implemented v0.2.04
  Able to auto accept group invites from those on your white list

* Auto Repair - Implemented v0.2.00
  When a toon with the addon opens a dialog with a repair vendor, it will attempt to repair all

* Auto Repair Announce - Implemented v0.2.07
  When Auto Repair has caused you to spend money, it will announce amount spent to other MultiTool users in your party. Configurable for self-only or broadcast and with sound.

* "Follow Me" - Not Started
  Any toon in group with the addon can send a "follow me" command and the others will attempt to /follow them... this will probably ONLY work out of combat due to Blizz security

* AutoTrade - SHELVED (AcceptTrade() can not be fired from addon due to WOW restrictions)
  IF a party member in your group with the addon AND in your white list clicks "accept trade", your toon will auto accept

* Triage - Not Started
  Auto switch party lead to next in line in your whitelist when current leader dies

* Quest Gossip Share - Implemented v0.1.06
  Allows other toons in your group with the addon to copy your choices on quest dialogs

* Auto Quest Completion - Not Started
  Quests with simple turn-in-and-done dialogs will autocomplete when NPC dialog is opened

* Quest Progress Announcement - Not Started
  Announces to others in your party who have the addon when you make progress on a quest(like the old cosmos-based Party Quests) used to do

* Auto Share quests - Not Started
  when one toon picks up a quest, they will attempt to share with others in the group who have the addon

* Auto accept shared quests - Not Started
  when a shared quest is offered by another in your group with the addon, you will attempt to accept

* Auto accept escort/event confirm type quests - Implemented v0.2.04
  When someone in your group starts an escort quest, your toon can auto accept instead of having to click yes or miss out

* Auto Sell Gray/Junk - Implemented v0.2.00
  When a toon with the addon opens a vendor dialog, it will attempt to auto-sell gray quality items... need a blacklist to stop selling of arbitrary desired items

* Auto restock reagents - Not Started
  When a toon with the addon opens vendor dialog, will scan for desired reagents/items as well as current supply in toon's inventory and buy enough to return to preset supply

* Group Hearth - Not Started
  Command to cause all in your group with MultiTool (in whitelist when I finally build that) to hearth

NOTES
There are probably many things I can't think of at the moment, but this is a good wish-list.

If I can figure out a way to do it, I may set this up as individual modules so that one can quickly enable/disable parts they want or don't want to save performance and to try and isolate the parts from each other as much as possible



---------------------------------------------------
|  TAXI DISPATCH...                               |
|      current setting: Shadowprey Village        |
| (you will automatically choose this destination)|
|   when you talk to a flightmaster)              |
|   ___                                           |
|  | X |   Uncheck this box to cancel your taxi   |
|   ---                                           |
---------------------------------------------------
