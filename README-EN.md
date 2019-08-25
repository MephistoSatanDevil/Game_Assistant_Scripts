[简体中文](README.md) | [English](README-EN.md)

# Game Assistant Scripts

**Author: c4_angel**  
**Support languages: English, Simplified Chinese**  
**Version: 1.6**  [ChangeLog](CHANGELOG-EN.md)

## Compatibility and Installation
- This mod only support Baldur's Gate Enhanced Edition(BG:EE), Siege of Dragonspear(SoD), Baldur's Gate II Enhanced Edition(BG2:EE) and Baldur's Gate Trilogh Enhanced Edition(EET).
- The mod will modify almost all of the spells in game (with no actual change to the effects of them) for checks in the scripts. So for insurance of the mod works well, it **MUST** be installed **AFTER** any mods which introduce new spell(s) or replace those already existed in game (such as Spell Revision). 
- The mod append at least two slots to SPLSTATE.ids (the number may be larger based on your mod enviroment). So the mod may fail to install if there are not enough slots.
- At the beginning of install, the mod will ask the user to set three hotkeys. Also you can set them before install by editing the ini file in the mod folder, or use component 2 to set/change the hotkeys whenever you want.

## WHAT IS IT
This mod aims to complete those boring, mechanical, time-wasting (IMO) operations automatically, by scripts.  
There are three part of the mod (only one main component): Battle AI Script, Auto Pause, and a semi-auto buffing system called "1-Key-Buffing".  
To use the script, you can:
- Activate the AI mod (default hotkey is "A" to switch AI mod on/off, or click the lock button in the lower right conner of your screen).
- Select one of your party member.
- Press the "call console" hotkey you have set. 
- Follow the guide, set the parameters as you prefer.

**NOTE: Except the Auto Pause system, the other two can only work when the AI mod is activated.**

### Battle AI Script
Just like the other AI scripts, this one controls the character's actions if no command given.
- Attacks. The script gives you three options: Attack the enemies in his/her weapon range (DEFAULT); Attack the enemies in sight aggressively; No attack action.
- Attack when invisible or not: NO (DEFAULT); YES
- Attack if Detect Traps or Turning Dead modal is activated or not: NO (DEFAULT); YES
- Bards start BATTLESONG modal automatically, then make attack actions: YES (DEFAULT); NO
- Thieves/Stalkers try to Hide in Shadows automatically: YES (DEFAULT); NO

### Auto Pause
Monitor the stat when characters cast those two kind of physical defence spells, and pause game when effects runs out.  
These are global setting, and disabled by default.
- StoneSkins and IronSkins. (The character must be either mage, druid, or cleric/ranger, or had acquired use-any-item ability.)
- Protection from Magical Weapons and the Mantle series. (The character must be mage, or had acquired use-any-item ability.)
	
### 1-Key-Buffing
There are two conditions must be satisfied to start 1-Key-Buffing: 
- AI mod is ON.
- Not in a combat, no enemy around any party member.
If you meet the conditions, you can press the self/team to start the buffing progress. Further instructions will be displayed in the console.

The following type of spells supported: 
- Arcane spells: e.g. StoneSkins(self only), Luck(both self and team), Improved Haste(party only)
- Divine spells: e.g. Armor of Faith(self only), Death Ward(both self and team), Champion Strength(party only)
- Innate spells (disabled by default): e.g. Hardiness(self only)
- Delayed Spells (to prevent spells cast by party members be protected): e.g. Globe of Invulnerability(self only)
- Arcane spells provide resistance enchantment (both self and team): e.g. Protection from Acid
- Divine spells provide resistance enchantment (both self and team): e.g. Resist Fire and Cold
	
**NOTE: In current version, the 1-Key-Buffing can read spells in vanilla BG:EE/BG2:EE, and those introduced/modified by “Improved Anvil v6.4”, "Eternal Force v4.4(Chinese only)" and "QC Kitpack v1.0(Chinese only)". So there may be differences when you install different mods. All supported spells are displayed in the console.**
