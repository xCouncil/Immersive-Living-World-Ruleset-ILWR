# **Update 202601116 - ILWR V2.3**
**Tested with MiMo 2.5/2.6 Free/Pro, Gemini 3.8, Gemini 4, DS 4.0 Pro, DS 4.1 Flash Thinking**

- **Context Usage Reduced to ~13.5k**
- **Output Tokens Reduced to prevent cutoff while keeping the same features**
- **Improved Epistemic Boundaries**
- **More proactive World and NPC state tracking + Dynamic Events (Incidents)**

## Files: [V2_20261116](https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR/tree/master/V2_20261116)

### CAMPAIGN CONTROL FRAMEWORK [ILWR]
- Merged the `PROSE CONSTRUCTION PIPELINE [PC]` with the Master File to Reduce context usage

## PLAYER INPUT HANDLING [PIH]
- Added instructions for scene and campaign pacing tying it strictly to the player input

## SCENE CONTINUITY AND TIMELINE ENGINE [SCTE]
- Moved `NPC SORTING` to `SCTE` and limiting on-screen Background Characters to 5 to avoid bloating the narration and hitting output limits

## CHARACTER INTEGRITY LOCK [CIL]
- Moved `NPC Sorting` to `SCTE`
- Updated Epistemic Boundaries to be Scene Wide covering all characters `NPC Source Material / Setting / In-Universe Epistemic Boundaries`
- Improved Epistemic Boundaries to cover world logic, recent events, memory recall, and to explicitly restrict NPC Actions `[Recent Events NO CURRENT TURN]`,  `[World Rules, Mechanics, & Logic]`, `[DEEP MEMORY RECALL]`, `[DOES NOT KNOW]`, `[EPISTEMIC RESTRICTIONS]`

## SCENE ORCHESTRATION [SO]
- Improved Background layer wording to specify Inter-NPC Banter, Env Obs, Player Callouts AFTER [PIH]->[FG] to try and improve NPC to NPC interactions
- Added `[NPC Agenda Resolutions]` to better handle NPC's independent actions and prevent the AI from collapsing it into reactions or summaries
- Moved `PROSE LAWS` to `PROSE EXECUTION [PE]` as a dedicated section

### PROSE EXECUTION [PE]
- Moved `PROSE LAWS` to `PROSE EXECUTION [PE]` as a dedicated section inside its own `<details></details>` to ensure compliance and make it easier for players to customize

### WORLD AND NPC STATE ENGINE [WNSE]
- Changed `Verbatim Plot Threads` to a Synthesis `[ILWR-WNSE-DB: PT & INC Synthesis & Developments]` to reduce output tokens and better help the AI plan the `NPC Agenda`
- Changed `[NPC Agenda]` to use `[WNSE-STEP-1 Motivation -> Next Plot Driving Action]` to avoid AI Railroading and better tie NPC actions to their plot thread / goals
- Improved Incidents to reduce output tokens, better cleanup of completed incidents, and avoid AI Railroading: `[PLAYER-COLLIDING INCIDENTS (Source of Truth: ILWR-WNSE-DB: PT & INC)]`, `[EXECUTABLE INCS (Passively waiting Player Schedule & Location trigger)]`, `[EXECUTING INCS-DELETE NEXT TURN]`
- Improved DB Mutations to try and make the WNSE more proactive: `[CREATING PLOT THREADS FROM Player and NPC emerging goals]`, `[UPDATING PLOT THREADS FROM ILWR-WNSE-DB: PT & INC Synthesis & Developments]`, `[CREATING INCS FROM ILWR-WNSE-DB: PT & INC Synthesis & Developments, NPC Agenda, Player Agenda]`, `[DELETING EXECUTED INCS]`
- Improved the wording on `NPC CONTEXT MANAGEMENT (TOGGLE CHECK)` to reduce context and ouput usage plus make it more reliable: `NPC-TOGGLE FOR NEXT SCENE (Activated NPC Cards Comparison)`

### ADDONS
- Improved `DM Dice Rolling` to specify the scope (DM Rolls Only) and the kind of roll its doing 

### Player's preferences for the DM (Magical DM HUD) / CORE DM Laws
- Added DM Behavioral Laws regarding consequences, World and NPC Logic, and Timekeeping

### ILWR-OUTPUT-TEMPLATE
- Renamed to `ILWR-OUTPUT-EXAMPLE` to avoid AI confusion when its disabled

---
Github for full packages:
https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR