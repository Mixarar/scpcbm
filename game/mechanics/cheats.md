---
title: Console commands
description: 
published: true
date: 2023-11-05T05:07:37.443Z
tags: 
editor: markdown
dateCreated: 2023-11-05T05:06:50.742Z
---

- [:arrow_backward: Back *Go back to the Mechanics page.*](/en/game/mechanics)
{.links-list}
# Console commands
The in-game console can be opened with the F3 key. Laptops with a Fn key may have to use the Fn + F3 keystroke. Alt + F3 is also a solution. Commands may be entered into the console in the format <command> <parameters> followed by the return or enter key, where multiple parameters are separated by a space.
## Parameter Types
- integer: A whole number, no decimals or fractions.
- float: An integer supporting fractions as decimals.
- string: A string of letters or numbers. Quotation marks must be omitted when entering strings in the console for them to be recognized.
- boolean: True or false, written as 1 or 0. Currently parsed as strings.
Note that the parameter of a command is not checked, so it may cause errors when used.
## Command Table
  | Commands| Parameters | Description |
|:-------------- |:-------:| ----:|
| help | String | 	If 'string' equals "1", displays a list of commands that can be used. If 'string' equals "2", displays the second part of the command list. If 'string' equals another command, displays help for that command if it's available. |
| 096state | None |Prints SCP-096's position, idle Boolean, and state if it has spawned. |
| reset096 | None | Resets SCP-096 back its idle, sitting down state. |
| 106speed | Float | Sets SCP-106's movement speed. Default is 0.01. |
| enable106 | None	 | Enables SCP-106 if it's either been disabled or contained.|
| disable106 | None |Disables SCP-106. Has the same function as containing it. |
| 173state | None | Prints SCP-173's position, idle Boolean, and state.|
| 173speed | Float |Sets SCP-173's movement speed. Default is 0.35. |
| enable173| None| Enables SCP-173 if it's already been disabled.
| disable173| None| Disables SCP-173. Has the same function as the MTF placing it into containment
|halloween | None| Replaces SCP-173's default texture with a jack-o-lantern-like texture.
| asd| None| General purpose debug command. Sets wireframe, godmode and noclip to on. Sets camerafog to 15 20.
|asd2 | None| Sets godmode and infinite stamina to on. Disables SCP-173 and contains SCP-106.
|gamma |Integer | Sets the gamma correction. Should be set to a value between 0.0 and 2.0.
|camerafog | CameraFogNear Float| Sets the draw distance of the fog. The fog begins at 'CameraFogNear' units away from the camera and becomes completely opaque at 'CameraFogFar' units away from the camera. Example: camerafog 5 15
  | camerapick|None | Prints the texture name and coordinates of the model the camera is pointing at.
  |debughud |String | If 'string' is equal to "on", "1", or "true", turns the debughud on. If 'string' is equal to "off", "0", or "false", turns the debughud off. The debughud displays status information about the player, SCP-173, SCP-106, SCP-096 if spawned, the current room event, and all currently spawned MTF units.
  |godmode |String | 	If 'string' is equal to "on", "1", or "true", turns godmode on. If 'string' is equal to "off", "0", or "false", turns godmode off. If 'string' equals anything else, toggles godmode. Godmode prevents the player from dying, prevents SCP-106 from taking them to the Pocket Dimension, and protects the player from any gunshot wound fired by guards, Nine-Tailed Fox, or helicopters. Bleed-related damage caused by SCPs, such as SCP-939 or SCP-966, is still possible however, and SCP-049 briefly blurs the player's vision even if his touch can do nothing to them in this state.
  |noclip fly| String| If 'string' is equal to "on", "1", or "true", turns noclip on. If 'string' is equal to "off", "0", or "false", turns noclip off. If 'string' equals anything else, toggles noclip. Noclip allows the player to fly through the game without any form of collision.
  | noclipspeed|Float | Sets the movement speed multiplier of the player during noclip to 'Speed'
  |infinitestamina/infstam |string | If 'string' is equal to "on", "1", or "true", turns infinitestamina on. If 'string' is equal to "off", "0", or "false", turns infinitestamina off. If 'string' equals anything else, toggles infinitestamina.
|notarget |String |If 'string' is equal to "on", "1", or "true", turns notarget on. If 'string' is equal to "off", "0", or "false", turns notarget off. If 'string' equals anything else, toggles no target. Disables every NPC's ability to target the player, essentially making them invisible.
  |stopsound stfu |None |Stops all currently playing sounds.
  |showfps | None|Toggles the FPS counter.
  |heal | None|Removes all injuries and blood loss from the player. Does not have an effect on a SCP-008 based infection.
  |kill suicide | None|Kills the player, bypassing Godmode.
  | revive undead resurrect|None |Revives the player. Does not have any effect on injuries, bloodloss or SCP-008 infection. Disables godmode and noclip.
  |infect |Float |Sets the SCP-008 based infection on the player to 'Infect' (Has valid range of 0 - 91, anything outside of this has a high chance of causing a MAV[1]).
  |injure | 	Float|Sets the player's injury level. (Has valid range of 1 - 5.) Higher injury levels induce blood loss and slower movement. Any value higher than 5 will kill the player.
  | Sanic| None|Toggles the "increased speed followed by death" mode used for certain items, displaying "GOTTA GO FAST" when enabled, and "WHOA SLOW DOWN" when disabled.
  |spawn |String Integer |Spawns a new instance of 'string' 0.2 units above the player. Sets the NPC's state to 'integer'.
|spawnitem	 |String |	Spawns a new item at the player's coordinates. Values for items are identical to the name they display in the inventory or their "tempname". Some items will require you to type in their template name as some of them can have the same name when viewed in the inventory. For example, if 'string' is equal to "Eyedrops", it will spawn the "Fine" eyedrops. However, to spawn the "Very Fine" variant of eyedrops, the "tempname" is needed, in this case it would be "supereyedrops".
  |ending |String |Immediately brings up the specified ending screen with the appropriate dialogue. If no ending is specified, a default ending screen will appear.
  |toggle_warhead_lever | None|Toggles the lever in the warhead room, affecting the game's ending.
  |unlockexits | String|	Unlocks the site's exits. If 'string' is set to "a" Gate A will unlock, if it is set to "b" Gate B will unlock and inputing anything else will unlock both gates.
  |teleport |String |Teleports the player to the room they input.
  |tp |String |Teleports the player to the MTF NPC defined as the "leader".
  | playmusic|String |Plays .ogg/.wav music files from the directory SCP - Containment Breach Multiplayer/SFX/Music/custom/. The file's extension must be specified.Using this command without specifying a file will cause any currently playing custom music to stop.
  |scp-420-j |None |Spawns 20 SCP-420-J instances in a circle around the player. These instances have a 50% chance of being a Joint, rather than SCP-420-J.
  | wireframe| String|If 'string' is equal to "on", "1", or "true", turns wireframe on. If 'string' is equal to "off", "0", or "false", turns wireframe off. If 'string' equals anything else, toggles wireframe. Wireframe allows only the edges of models to be rendered.
  | pumpkin spawnpumpkin|None |What pumpkin?
| jorge| None|Outputs the message "JORGE HAS BEEN EXPECTING YOU".
  |spawnradio |None |Spawns a Radio at player's position. This radio has electricity, although there is no battery in radio.
  | spawnnvg|None|Spawns a Night Vision Goggles at player's position.
  | spawnnav| None|Spawns a S-Nav Ultimate at player's position.
  |teleport173	 |None |Teleports SCP-173 to player's position if SCP-173 is not re-contained.
  | teleport106| None|Teleports SCP-106 to player's position if SCP-106 is not re-contained.
  |spawnparticles |Integer |Spawns a particle at player's position according to ID.
  | giveachievement| Integer|Gives a achievement to player according to ID.
  |427state | Float|Set holding time of scp427, no parameter will set with max value.
  |setblinkeffect | BlinkEffect: Float|BlinkEffect will effect the speed of blink, BlinkEffectTimer will decide the duration of BlinkEffect.
  
## Npc Types
 | NPC Parameter| NPC Value|
|:-------------- |:-------:|
|008zombie|SCP-008 Infected
  |scp049 |SCP-049
  | 049-2|SCP-049-2 Instance
  | scp066|SCP-066
  |scp-096 |SCP-096
  |scp-106 |SCP-106
  |scp-173 |SCP-173
  | scp-372|SCP-372
  |scp513-1 |SCP-513-1
  |scp966 |SCP-966
  | scp-1499-1|SCP-1499-1
  |class-d |Class-D
  |guard |Guard
  |mtf |MTF unit
  | helicopter|Apache
  |tentacle |SCP-035 Tentacle
  |008 |SCP-008 infected
  ## Item Types
` you need to type "Spawnitem "itemname" to spawn the item `
| Item Template Name| Item Value |
|:-------------- |:-------:|
  |gasmask |Gas Mask
  | supergasmask	|Super Gas Mask
  |gasmask3 |Heavy Gas Mask
  |key1 |Level 1 Keycard
  |key2 |Level 2 Keycard
  | key3|Level 3 Keycard
  |key4 |Level 4 Keycard
  |key5 |Level 5 Keycard
  | key6|Omni Keycard
  |firstaid |First Aid Kit
  | finefirstaid|Small First Aid Kit
  |firstaid2 |Blue First Aid Kit
  |vest |Ballistic Vest
  | finevest|	Heavy Ballistic Vest
  | veryfinevest|Bulky Ballistic Vest
  |s-nav 300 navigator |S-Nav 300
  |s-nav 310 navigator|S-Nav 310
  | s-nav navigator ultimate|S-Nav Ultimate
  | hazmatsuit|Hazmat Suit
  |hazmatsuit2 |Mysterious Hazmat Suit
  |hazmatsuit3 |Heavy Hazmat Suit
  |radio |Radio
  |fineradio |Radio which does not require batteries.
  |veryfineradio |Very Fine Radio
  | 18vradio|Radio which uses 18V batteries.
  |bat |9V Battery
  |18vbat |18V Battery
|killat|Strange Battery
  |revision eyedrops |ReVision Eyedrops
  |fineeyedrops |RedVision Eyedrops
  |redvision eyedrops |Fine Eyedrops
  |supereyedrops |Very Fine Eyedrops
  |hand |Severed Hand
  | hand2|Black Severed Hand
  | clipboard|Clipboard
  |nvgoggles |Night Vision Goggles
  |wallet |Wallet
  |finenvgoggles|"Fine" variant of the Night Vision Goggles
  | supernv|"Very Fine" variant of the Night Vision Goggles
  |scp148 |SCP-148
  |scp148ingot |Ingot of SCP-148
  |scp500 |SCP-500-01
  |scp513 |SCP-513
  | scp714|SCP-714
  | scp860|SCP-860
  | scp1025|SCP-1025
  |scp1499 |SCP-1499
  |420 |SCP-420-J
  | joint|Joint
|smelly joint |Smelly Joint
  | cigarette|Cigarette
  | veryfinefirstaid|Strange Bottle
  | mastercard|MasterCard
  |playing card |Playing Card
  |origami |Origami
  | Emily Ross's Badge|Emily Ross's Badge
  | emptycup|Empty Cup
  | coin|Coin
  |ticket |Movie Ticket
  |key |Lost Key
  | Old Badge|Old Badge
  | Quarter|Quarter
  
  
  
  