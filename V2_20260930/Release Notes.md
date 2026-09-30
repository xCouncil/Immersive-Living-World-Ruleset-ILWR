# **Update 20260930 - ILWR V2**
**Tested with MiMo 2.5/2.6 Free/Pro, Gemini 3.7 Flash, Gemini 3.8, DS 4.1 Flash Thinking**


# **ILWR V2**
Special Thanks to @boulder & @dumpy for playtesting V2, its through their efforts that V2 was able to be released in a timely manner

- **Context Usage REDUCED to ~15k from ~25k**
- **80% Reduction in Token Output / Scratchpad Bloat**
- **Uses Auto Updates to Manage the Dynamic Events and Plot Threads in the Character Data**
- **Retains the Same functionality, Immersive NPCs and a living breathing world that advances on its own**

---

## Files: [V2_20260930](https://github.com/xCouncil/Immersive-Living-World-Ruleset-ILWR/tree/master/V2_20260930)


## Structural Changes:
Core Files renamed and re-written
- CAMPAIGN CONTROL FRAMEWORK [ILWR]
- PROSE CONSTRUCTION PIPELINE [PC]
- PLAYER INPUT HANDLING [PIH]
- SCENE CONTINUITY AND TIMELINE ENGINE [SCTE]
- CHARACTER INTEGRITY LOCK [CIL]
- SCENE ORCHESTRATION [SO]
- PROSE EXECUTION [PE]
- WORLD AND NPC STATE ENGINE [WNSE]

**Dedicated Character Data sections NEED to be created for the WNSE to function:**
Create a Folder in your Character data called `ILWR-WNSE-DB: PT & INC`

## NPC Card Changes (Optional but Highly Recommended):
i highly recommend (although it eats context) to prepend NAME- to each section of your NPC cards like `Name-Personality`, `Name-Location`, `Name-Appearance`.

```
NPC Name1
Name1-Location: ...
Name1-Personality: ...
Name1-Appearance: ... 
....
NPC Name2
Name1-Location: ...
Name1-Personality: ...
Name1-Appearance: ...
```
Because when searching the context window the AI finds multiple "Personality" lines even though they are below the "Name" 

So it greatly helps if they see

NPC Name2
Name2-Location: ...

**Easier searching, like looking for a needle in a haystack in the dark but the needle glows**

---
## Visual Novel Dialog Changes
> ### ⚠️AI Realm caps  the output tokens  at 10k, the current state of the Visual Novel Mode requires a lot of tokens for the HTML, consider removing the backgrounds if your scenes are long or have multiple NPCs

> ### 🎉 The VND is fully standalone even without ILWR that cleanly separates the Instructions and the config allowing you to change the CSS easily, context usage is also reduced. I highly recommend creating an NPC Card for your character so you can create an icon for it and zoom in to your characters lovely face!

- AI GM Instructions isolated in  `VISUAL NOVEL DIALOG [VND]`
- Links and Configuration should go in into another GM Guide `[VND] Config`
- To remove the background simply delete the instruction for the `BACKGROUND WRAPPER`


Credits to @violetsama for the idea, updating the instruction to:
> URL RULES: ALL URLS MUST BE CONSTRUCTED BY APPENDING THE ASSET ID TO THE BASE URL https://storage.googleapis.com/airealm-prod-images/npc-images/npc_YOUR_CHAT_ID_HERE

Your Chat ID is the numbers and letters you see at the end of your chat e.g. https://airealm.com/user/viewChat/**123abcd** 

or In the case of Mobile devices it is whatever comes before the **_123145.jpg** for image links
e.g. https://storage.googleapis.com/airealm-prod-images/npc-images/npc_CHATIDHERE_2407222.jpg

Once you have that rule and chat id setup you can change all your NPC cards to just have the **_123545.jpg** saving context e.g.
```
Color: #DC143C
Icon - Default - _2357528.jpg
Icon - Focused/Determined - _2357536.jpg
```

Credits to @pitifuldelay for the idea
**You can now change how harsh the background overlay is depending on your BG**

In your location BG you can add DARK/LIGHT to it to indicate whether the BG is too bright
- DARK = Image is dark, less harsh background overlay, you should be able to see the BG more
- LIGHT = Image is light and drowns out whites, harsher background overlay so both the narration and the BG is still visible

```
[LOCATION BG]
FALLBACK BG (When none are applicable): _2333427.jpg
Location - BG URL - DARK/LIGHT
Combat - _2357558.jpg - DARK
```

---
## **Migrating from V1 to V2**
*If you use the Visual Novel Addon replace it as well following the Visual Novel Dialog Changes instructions*
1. Replace all your V1 files your only ILWR files should be:
    - ILWR-0-CAMPAIGN CONTROL FRAMEWORK [ILWR]
    - ILWR-1-PROSE CONSTRUCTION PIPELINE [PC]
    - ILWR-1-PC-1-PLAYER INPUT HANDLING [PIH]
    - ILWR-1-PC-2-SCENE CONTINUITY AND TIMELINE ENGINE [SCTE]
    - ILWR-1-PC-3-CHARACTER INTEGRITY LOCK [CIL]
    - ILWR-1-PC-4-SCENE ORCHESTRATION [SO]
    - ILWR-2-PROSE EXECUTION [PE]
    - ILWR-3-WORLD AND NPC STATE ENGINE [WNSE]
    - ILWR-OUTPUT-TEMPLATE **(TOGGLED ON INITIALLY)**

2. Send a Message to the AI DM:
    ```
    (( OOC: DM Pause the Campaign Completely, I have reworked the ILWR read the Campaign Control Framework and all its steps, then analyze the Output Template and confirm your readiness to run it ))
    ```

3. Execute your next turn with the `ILWR-OUTPUT-TEMPLATE` **ON**

4. Verify that it is running, there should be **ZERO** prose in the [PC] section, the only place where
sentences should be written are:
- `SCTE`
- `CIL`
- `WNSE`

5. Once you confirm that it is running send another message to the DM to create your Plot Threads and Incidents:
    ```
    (( OOC: DM Pause the Campaign, Look at my current plot threads and world events, execute the new WNSE creating the plot threads and Incidents in the ILWR-WNSE-DB: PT & INC folder ))
    ```

6. Manually adjust them as needed but all plot threads and incidents (formerly world events) should be in the `ILWR-WNSE-DB: PT & INC` folder

7. Toggle `ILWR-OUTPUT-TEMPLATE` **OFF**

8. Continue playing as usual!

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