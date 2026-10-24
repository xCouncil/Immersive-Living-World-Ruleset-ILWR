# **Update 202601019 - ILWR V2.2**
**Tested with MiMo 2.5/2.6 Free/Pro, Gemini 3.7, Gemini 3.8, Gemini 4, DS 4.1 Flash Thinking**

**Context Usage Reduced to ~14k**

## Files: [V2_20261019](https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR/tree/master/V2_20261019)

### PROSE CONSTRUCTION PIPELINE [PC]
- Reduced context usage

## PLAYER INPUT HANDLING [PIH]
- Tightened the wording to reduce context usage

## SCENE CONTINUITY AND TIMELINE ENGINE [SCTE]
- Tightened the wording to reduce context usage
- Tightened the wording on world lore to try and prevent logic breaks, now named `[Operational Source Material Mechanics, Constraints, & Timetables]`

## CHARACTER INTEGRITY LOCK [CIL]
- Tightened the wording to reduce context usage
- Updated relationship pulls to be verbatim maximum of 4 to reduce output tokens and prevent hallucinations
- Updated memories & knowledge pull to epistemic boundaries, including goals/insecurities for more nuanced reactions

## SCENE ORCHESTRATION [SO]
- Updated the wording for better enforcement of turns and scene pacing
- Tightened the prose constraints to reduce context and output usage

### PROSE EXECUTION [PE]
- Condensed the `[PE-CORE LAWS]` to reduce context and added instructions for `<say></say>` tags to never be narrated as "Character says"
- Implemented minimalist single line header to support in full VN mode
- wrapped `<details></details>` tags in `<say who="DM"></say>` tags to support both Portrait Mode and full VN Mode

### WORLD AND NPC STATE ENGINE [WNSE]
- Made `[VERBATIM PLOT THREADS & NPC ROSTER]` more human readable 
- Changed `[NPC Agenda]` to have `Plot Driven Objective & Motivation` and `Next Objective Advancing Action` to tie NPC actions better to their plot thread / goals
- Improved wording for `[EXECUTING INCS]`, Creating/Updating/Deleting Plot Threads & INCs to make the world feel more dynamic and the auto-updater more reliable
- Improved the wording on `NPC CONTEXT MANAGEMENT (TOGGLE CHECK)` to make it more reliable

### ADDONS
- Deleted the `Visual Novel Dialog` addon please use the official version! it is fully supported by the updates
- Removed the unreliable battle grid in the `Combat Tracker`
- Added Portrait and VN mode support for `DM Dice Rolling`

### Player's preferences for the DM (Magical DM HUD)
- Updated the wording and added the user satisfaction law to try and reduce AI Sycophanty

---
Latest Version of Loose files can be found in
https://discord.com/channels/1105664318332211252/1524010781216342077

Mods:
https://discord.com/channels/1105664318332211252/1542726145743790221

Github for full packages:
https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR