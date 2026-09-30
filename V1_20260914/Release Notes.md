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


Loose files can be found in
https://discord.com/channels/1105664318332211252/1524010781216342077

Mods:
https://discord.com/channels/1105664318332211252/1542726145743790221

FAQS:
https://discord.com/channels/1105664318332211252/1548859287227596830