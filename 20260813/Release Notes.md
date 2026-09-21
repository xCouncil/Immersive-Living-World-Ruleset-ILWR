# **Update 20260813**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Integrated the scaffold to the main directives while maintaining a relatively low context usage (17,360 total)

- Added better guardrails for Player Input to be split intelligently (Different Subject/Objective = new beat) to prevent AI top loading
the player's turn and not have NPCs react beat by beat

- Reworked SCTE and CIL for Anti DM Metagaming, SCTE now only contains the world state and relevant history, CIL determines in character knowledge

- Prose Construction Reworked to emphasize the sensory emotional experience presenting it as if the player is in the world itself, tries to prevent subtext

- Added back pre-flight compliance gate as a checkpoint between NBE and NE to try and steer the AI into compliance before writing prose


**REWORKED WNSE WITH ACTUAL CONSEQUENCES AND DYNAMIC EVENTS**

- Reworked the WNSE, SCTE, and NOH to provide the player with plot threads advanced by the NPCs on their own and dynamic events
as consequences of their actions

- SCTE will now track the NPC next actions (NPC turns) and world events that are pending

- NOH now includes the REACTION LAYER and the INDEPENDENT WORLD STATE LAYER, the reaction layer has every NPC available react to the player's input
the Independent world state layer triggers NPC actions that advance their plot threads e.g. going off somewhere or meeting you somewhere later or setting something up
and also triggers world events as consequences of your actions e.g. NPCs witness you do X, it results in Y that happens on Z

- WNSE now set to generate and track Plot Threads and World Events based on the campaign summary and a source of truth file
```ILWR - WNSE: OPEN PLOT THREADS & WORLD EVENTS``` which the DM will keep track of and trigger at the appropriate times (You can manually add/edit plot threads and world events you dislike

Latest Version of Loose files can be found in
https://discord.com/channels/1105664318332211252/1524010781216342077

Mods:
https://discord.com/channels/1105664318332211252/1542726145743790221

FAQs:
https://discord.com/channels/1105664318332211252/1548859287227596830

Visual Novel Guide:
https://discord.com/channels/1105664318332211252/1550354226771918858

Github for full packages:
https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR