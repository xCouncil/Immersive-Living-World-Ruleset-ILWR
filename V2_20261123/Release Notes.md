# **Update 202601123 - ILWR V2.4 - Moving to System Instructions!**
**AI Realm is introducting System Instructions Improving Ruleset adherence and removing possible conflicts!**

**Tested with MiMo 2.5/2.6 Free/Pro, Gemini 3.8, Gemini 4, DS 4.0 Pro, DS 4.1 Flash Thinking**

## Summary of Changes:

- **Context Usage Reduced to ~13.2k**
- **Output Tokens Reduced to prevent cutoff while keeping the same features**
- **Improved Epistemic Boundaries and NPC Personality Adherence**
- **Improved NPC Agenda**
- **Introduced Core Gameplay Rules, an optional replacement to the default system instructions**
- **Reintroduced the ILWR-BOOTSTRAP**
- **Added Auto Update Preferences so the AI can better make use of the `WNSE`**

## Files: [V2_20261123](https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR/tree/master/V2_20261123)

### CAMPAIGN CONTROL FRAMEWORK [ILWR] - RENAMED TO `ILWR-0-GAMEPLAY-LOOP`
- Converted into the `CAMPAIGN SIMULATION FRAMEWORK [ILWR] Folder` to house the core files

### Added the `CORE GAMEPLAY RULES`
- Alternatives to the default system instructions covering Combat, dice rolls, skill checks, DM Behavior and Timekeeping, Mature content, OOC Communication, Player Agency and pacing, and Text Styling

## CHARACTER INTEGRITY LOCK [CIL]
- Improved Epistemic Rules for better adherence: `Universal Epistemology` section
- Re-arranged the `CIL` to set the epistemic boundaries first before the personality audit to improve character fidelity

### PROSE EXECUTION [PE]
- Improved `PROSE EXECUTION CHECKLIST` containing easily editable constraints for Prose Narration:
`[CORE LAW: FORBIDDEN PROSE CONTENT]`, `[CORE LAW: MANDATORY BEAT REQUIREMENTS]`, `[CORE LAW: MANDATORY SCENE CLOSURE]`
- Added `Active turn binding` to ensure the AI doesn't treat it as boilerplate and ignore

### WORLD AND NPC STATE ENGINE [WNSE]
- Added 2 sentence constraint to `[ILWR-WNSE-DB: PT & INC Synthesis & Developments]` to reduce output tokens and better help the AI plan the `NPC Agenda`
- Changed `[NPC Agenda]` to to a clean top down generation with `WNSE-STEP-1 Motivation`, `Current Micro Status`, `Next Turn Micro Step` including better anti-railroading/scripting instructions

### ILWR-OUTPUT-EXAMPLE -> RENAMED AND IMPROVED INTO ILWR-BOOTSTRAP
- Renamed to `ILWR-BOOTSTRAP` for easier AI Steering

---
Github for full packages:
https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR