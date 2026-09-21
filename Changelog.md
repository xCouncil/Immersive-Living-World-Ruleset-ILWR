# # **V1 Release! 20260707**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**

---

# **Update 20260710**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Created a separate Prose construction guide which will allow players to shape how they want the prose to be written by the AI

- Re-arranged the baseline rules load order so each rule better feeds into each other

- Re-arranged the pre-flight compliance gate to follow the load order so the AI doesn't have to back reference

- Tightly coupled the narration execution to the  pre-flight and the world and npc state engine. by making the wording airtight.

---

# **Update 20260711**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Re-arranged the pre-flight compliance check to have a cleaner chain of thought to prevent further back reference establishing the continuity first before running the checkpoints

- Added stronger wording in the narration structure that the Pre-flight is the blueprint, the micro while the world and npc state engine is the macro

---

# **Update 20260716**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Renamed and Separated the Scene continuity and timeline engine to its own guide, can be plugged into any header as required

- Tighter language and chain of thought in the pre flight compliance gate, added explicit token efficient formatting without sacrificing its use, and every checkpoint and source guide has proof that it was executed

- Reworked the character integrity lock to still provide nuance but much less cognitive load

---

# **Update 20260718**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


Uploading Alternate Plug and Play sets of the latest versions, for those who want to just drop specific core rules into their campaign and have them outputted in their headers / footers

PS: Some models like MiMo and Gemini prefer this plug and play version where the pre-flight references the source rule, while Qwen and DS seem to prefer the output format within the pre-flight itself so play around with your models!

---

# **Update 20260721**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


With FREEMO's release i endeavored to make this work with it as well as the notoriously lazy and stubborn DSv4 Pro. 

Presenting the FREEMO and DS Proof stack. 

Still Modular and still works with the smarter models like Gemini and MiMo Pro but now also caters to the lazier and not-so-smart models.

---

# **Update 20260726**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Lower total character usage (from 15k to 13k)

- Tighter framework coupling through unique namespaces preventing AI model confusion

- Cleaner checkpoints and chain of thought resulting in 26% less token usage for cognitive load resulting in faster response generations retaining the quality.

---

# **Update 20260730**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Reduced context usage from 14.7k to 12.8k

- Reduced cognitive load by condensing chain of thought and merging it with the output format where applicable

- Reduced drift by having the AI reference the master file (CAMPAIGN CONTROL FRAMEWORK: IMMERSIVE LIVING WORLD RULESET [ILWR]) more frequently

- Added DS guardrails on the master file, specifically:
```
AT THE TOP OF EVERY RESPONSE OUTPUT THIS LINE: [ILWR FRAMEWORK: NBE -> NE -> WNSE]
BEFORE EVERY COMPONENT OUTPUT THIS LINE: ———ILWR FRAMEWORK - NBE/NE/WNSE GENERATING———
```

This can also be placed in the Player's preferences if DS is being extra stubborn

---

# **Update 20260802**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Created alternative versions of some of the core system rules that strip all output formatting and consolidated them in the CORE SYSTEM RULE-NARRATION EXECUTION [NE] with a complete scaffold

- Replacing the standard modules with these alternate versions totals 16.6k characters, the standard version is 12.7k, it is only slightly above if you also toggle on the ILWR - NBE - SAMPLE SCAFFOLD to remind the AI what the format should be

- Based on Preemo's analysis these ALT version should reduce cognitive load and reduce drift, I believe the drift part, the cognitive load I have not seen significant improvements maybe 1-2 seconds faster which can be chalked up to nobody using preemo during the time of testing.

- This is more for those who can afford the +4k context bump and don't want to be bothered toggling the scaffold on and off to correct the AI. On the bright side if you were using the old versions of the framework it was ~16k before as well so using this alt version would have no noticeable change in your total context usage.

---

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

---

# **Update 20260820**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Improved the prose generation guardrails by detaching the PC from the NBE and slotting it into the narration execution, this replaces the ```PRE-FLIGHT COMPLIANCE GATE```
it aims to: better enforce the immersive sensory rich narration, better enforce the narration of the independent world state layer to maintain NPC agency

- Improved the WNSE to assist the AI in generating NPC actions that directly advance the plot threads they are involved in, previously it was treating them as simple labels

- Removed the NPC Next Actions from the SCTE to reduce bloat and AI drift, unresolved world events retained

- Improved the CIL to assist the AI in introducing nuance by having the history/development section be something that reinforces existing traits and adds to their reaction

- Improved the CIL to assist the AI in portraying background NPCs by looking for an [Ambient NPC Personality] section in the NPC card, and only defaults to summarizing it themselves if it doesn't exist. This is highly recommended so your beloved NPCs stay in character even when in the background.

- Improved the NOH to be the sole generation engine of NPC actions with improved handling of player actions that derail their original pre-planned response

- Removed the hardcoded dialog color from the Narration Execution, it now checks your character data for "player dialog color", Personally I put it in my player's preferences for the DM: Player Dialog Color: #47788A

---

# **Update 20260823**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Optimized NE to use less tokens while keeping the core prose construction working and to better handle NPC independent actions

- improved the wording on NOH and also had the AI label them as Foreground / background to force it to produce both actions and dialog (anti diorama / static dead background characters)

- Moved the PC as a subroutine to the Narration Execution where it belongs in the master file

- Optional file to put in the player's preferences for the DM regarding it being a DM that runs the framework

---

# **Update 20260828**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


- Improved the wording on the SCTE Recent events to present only the events leading up to the current scene for continuity and knowledge

- Improved the wording on the SCTE common information to force the AI to say what kind of knowledge the source excerpt provides, this helps reduce the redundancy with the CIL

- Improved and reduced the context usage for the PIH, introduced clear 1 sentence identifiers that will be passed onto the other steps

- Improved the NOH to enforce NPC reactions to prevent "Diorama" scenes where NPCs are mute and static everyone should be reacting to the player

- Improved the NOH to better allow the AI to bring NPCs in and out of scenes depending on their planned actions

- Improved the NOH to better guide the AI to introduce temporary NPCs for triggering world events


- **Reworked the PROSE CONSTRUCTION [PC] in the NARRATION EXECUTION [NE]**

    * Better enforcement of Sensory Rich, Player-centric narration by having the model write the first 2 sentences of its planned paragraph then carry it over into the prose

- Better enforcement of the Independent world state layer to ensure its always rendered alongside the NPC reactions to the Player's turn.


- Improved the Wording on WNSE Step 4 to align with the NOH regarding introducing temporary NPCs for triggering world events or immediate situations and bringing NPCs in and out of the scene depending on their agency

---

# **Update 20260901**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


**SCTE**: 
- SCTE Now only contains the 5 most recent events as a lookback to anchor the continuity
- general NPC knowledge refined as Current Micro State-of-Play World Knowledge Pool reducing AI drift, bleed, and metagaming

**CIL**: 
- Removed the MOTIVATION from the CIL
- Split the Situation Relevant History/Development into 2 distinct steps: Relationship Information and Memories
- Introduced a SITUATION-GENERATED PHYSICAL ACTIONS synthesizing their personality into the immediate physical actions they take for the situation

**NOH**:
- Now only TEXTURES the NPC actions, enforcing the manifestation of their traits, habits, relationship, and history to provide nuance to their CIL Generated Physical Actions
- Introduced a Dialogue Preview to enforce the NPC's established speech pattern reducing AI drift and tropey writing styles
- Introduced a context anchor to pass onto later steps to remove the need to copy them verbatim, reducing bloat
- Improved the wording to assist the LLM in making NPCs pop in-and-out of scenes as needed

**NE / PC**:
- Refined the Paragraph Execution Directives to focus on the texture, quality, and weight of sensory information for increased immersion
- Hard coded the banned prose writing styles
- Refined the metadata anchor and the paragraph preview

**WNSE**:
- Restructured the WNSE as a pipeline: Big Picture -> Granular Actions -> Consequences
- Immediate Objectives are determined from the Next Milestone
- NPC Actions directly derived from the Immediate Objective
- Improved the wording to assist the LLM in making NPCs pop in-and-out of scenes as needed
- World Events now more easily generated as consequences from the world state

---

# **Update 20260906**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


**Master File & NBE**
- Streamlined, PIH moved to Step 1

**PIH**
- Clearer Instructions on Input Grouping and Context Anchoring

**SCTE**: 
- SCTE Now also includes ON-SCREEN NPC tracking and ambient/bystander NPC spawning for BG noise

**CIL**: 
- Now directly references PIH for NPC Sorting
- Converted to pure database lock removing SITUATION-GENERATED PHYSICAL ACTIONS

**NOH**:
- Now generates AND textures the NPC actions using the CIL Context Anchor lookback leading to more faithful adaptations,
added strong wording regarding the manifestation of traits as physical reality instead of meta commentary
- Set clearer guardrails for FG vs BG actions and dialog
- Dialog Preview converted to Full dialog ensuring consistent speech patterns 
- Improved Temporal consistency by stronger wording that the Independent World State layer is a direct continuation of the Reaction Layer
Allowing NPCs to better enforce their agency but adapt to the player input in a realistic manner and remove AI rewinding

**NE / PC**:
- Removed the hex palette, AI is able to randomly select a hex color on its own
- Improved hard coded banned prose writing styles
- Added Temporal Perspective: Realtime to ensure narration is a lived experience
- Changed "Player Literal Sensory Experience" to "Scene Sensory Texture" focusing on the quality, texture, and weight of sensations to avoid instances of mechanical checklists

**WNSE**:
- Split Generated World events from Triggering world events for better AI planning for the next turn
- Introduced NPC toggle so AI toggles NPCs appearing in the next turn ensuring the AI has context for the CIL when they appear
- Added Reasoning blocks to actions and objectives ensuring they move towards the milestones

**Optional Player's Prefs File**
- Stronger DM Persona wording for compliance


---
# **Update 20260914**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**

**Master File**
- Streamlined Reduced Token count

**PIH**
- Clearer Instructions on Input Grouping and Context Anchoring, Dialog signals the end of a narrative beat to force NPC response

**SCTE**: 
- Streamlined, Ambient NPCs / Bystanders Context Anchored so they appear as background fluff not direct background NPCs that
may produce annoying dialog

**CIL**: 
- Removed Ambient NPCs / Bystanders in the CIL to prevent bloat and random background fluff receiving audits

**NOH**:
- Added Action Economy anchors PER beat so NPCs never underreact or go mute
- Clarified NPC actions as "Next Turn" so they dont jump forward in time ahead of the player

**NE / PC**:
- Splitting the NE and the PC into its separate files again so people can easily take it apart and customize to their liking

**PC**:
- Updated the prose styling with a better [Prose Instructional Anchor] it will use the following
Narrative Voice: Player as source=Present Tense-Deep POV, Lived Experience, 
NPC as source=Third Person using Second Person Pronouns, 
Environment as source=Second Person Perceived by the Player's Senses
- Added Ambient NPCs / Bystanders as environmental fluff to add to immersion
- Updated Paragraph Preview with hard guardrails to produce better prose reliably

**NE**: 
- Updated the timekeeping header to use Leaning's style HUD 
- Added the ADDON System! For Headers and Footers

**WNSE**:
- Clarified NPC actions as "Next Turn" so they dont jump forward in time ahead of the player
- Put hard rules that NPC Next Turn Actions should never be Passive or Waiting, they should always be Proactive
- Added Ambient NPCs / Bystanders from SCTE as potential witnesses and triggers for generated world events
- Improved NPC Toggling


**THE ADDON SYSTEM**

The Addon System is designed for players to customize the ILWR without breaking the core loop
It allows you to inject your own headers / footers or even inside the prose itself!
Simply Create a folder named `[ILWR ADDONS]` then in your addon put the `[ILWR ADDON PLACEMENT]` flag
- Header = Execute in the [ILWR ADDONS - HEADERS] section
- Footer = Execute in the [ILWR ADDONS - FOOTERS] section
- Embedded = Execute in the [NBE GENERATED AND PC CONSTRUCTED PROSE] where applicable

**Current Official Addons (Mileage may vary depending on the model you are running!)**
- ILWR ADDON: AUTO UPDATE ENGINE [AUE] credit to @koiske and @nightraven42 
- ILWR ADDON: DM DICE ROLLING [DDR]
- ILWR ADDON: COMBAT TRACKER [CT] credit to @nightraven42 for the idea and @drshinryuu for the Pillars of Play

---


# **Update 20260918**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**

**Reduced Base context usage by ~200**

**NOH**:
- Fixed the placement of the context anchor for OFF-SCREEN NPCS

**PC**:
- Moved the Paragraph preview description to the main loop with an explicit Minimum 3 sentence anchor to prevent dead narrative beat openings
- Added explicit [Narrative Beat] identifiers to signal the AI to generate the [Prose Instructional Anchor for each beat]

**NE**: 
- Removed a Typo and updated only the NPC name to be bold while the dialog is normal font for easier reading

**WNSE**:
- Fixed conflicting instruction typo in the WNSE-STEP-3: WORLD STATE & NPC NEXT TURN ACTIONS, thanks to @Nightraven4t2 for spotting it!


**ILWR ADDON: VISUAL NOVEL DIALOG [VND]**
This is a direct ILWR implementation of my Pseudo Visual Novel Guide: https://discord.com/channels/1105664318332211252/1550354226771918858
It is **Entirely Optional** and does **NOT** overwrite anything in the **NE** when Toggled **OFF**
When Toggled **ON** it implements the new HTML for the circular avatars, it also natively allows for emotion to icon mapping!

---

# **Update 20260919**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


**ILWR ADDON: VISUAL NOVEL DIALOG [VND]**
- Updated the styling of the dialog boxes to be more emphasized and visually distinct
- Upgraded the VND Addon to include chat backgrounds! Just add it to the location BG
list (examples already included in the addon) and it will automatically wrap the prose in that background

---

# **Update 20260921**
**Tested with MiMo 2.5 Pro, Muse Spark 1.2, DSv4 Pro, MiniMax M3, Gemini 3.7 Flash, DSv4.1 Thinking**


**ILWR ADDON: VISUAL NOVEL DIALOG [VND]**
- Updated the styling of the dialog boxes to be more emphasized and visually distinct
- Upgraded the VND Addon to include chat backgrounds! Just add it to the location BG
list (examples already included in the addon) and it will automatically wrap the prose in that background

---