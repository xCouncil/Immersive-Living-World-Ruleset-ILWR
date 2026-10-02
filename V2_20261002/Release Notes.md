# **Update 202601002 - ILWR V2.1**
**Tested with Muse 1.2, MiMo 2.5/2.6 Free/Pro, Gemini 3.7 Flash, Gemini 3.8, DS 4.1 Flash Thinking**


## Files: [V2_20261002](https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR/tree/master/V2_20261002)


## Bug Changes:
- Fixed typos identified by @boulder in the PROSE EXECUTION still referencing old info and the WNSE missing long term objectives when creating plot threads

## SCENE CONTINUITY AND TIMELINE ENGINE [SCTE]
- Updated the SCENE CONTINUITY AND TIMELINE ENGINE to explicitly reference all WNSE NPCs and Emergent NPCs (NPCs that are introduced by the player's actions e.g. talking to a shop keeper)

## SCENE ORCHESTRATION [SO]
- Updated the scene layers to state `CHRONOLOGICAL ORDER` instead of `DIRECT CONTINUATION` to reduce AI confusion regarding one layer causing the other when they should just be in chronological order

- Updated `SCENE_BACKGROUND_DETAILS` into `SCENE_BACKGROUND_&_BYSTANDER_DETAILS` to make the world feel more alive with random NPC ambient fluff without giving them dialog

## WORLD AND NPC STATE ENGINE [WNSE]
- Renaming `[TRIGGERING INC]` to `[EXECUTING INC]` to reduce AI confusion that the INCs will execute on the next turn
- Split `ON-SCREEN NPCS` into 2 categories: `[NEXT SCENE: IMPLIED ON-SCREEN (PRELOAD)]` & `[NEXT SCENE: WNSE ON-SCREEN]` so the AI knows to activate NPC cards

---
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