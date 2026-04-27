<!-- ═══════════════════════════════════════════════════════════════════════
     INSTRUCTIONS FOR CLAUDE (READ FIRST, THEN REMOVE BEFORE SAVING)

     The user has pasted this template into the chat to set up a CONTEXT.md
     file for one of their projects. They are likely non-technical. Be patient
     and conversational.

     What you do:
     1. Greet them briefly without assuming you know them. Treat this as a
        fresh setup, even if you have memory from previous chats.
     2. Confirm which project this is for (one project per CONTEXT.md file).
     3. Ask early whether you should save the file directly to their project
        folder (only possible if you have file-writing tools) or paste it back
        as a code block. Default to the code-block option if you can't tell.
     4. For each section below:
        - Read the HTML comment to understand what it's for
        - Ask the questions needed to fill in the [bracketed bits]
        - Keep it conversational. One section at a time.
        - For sections with several short fields, group 2-3 related questions
          in one message. For sections that need real thought (north star,
          goals), ask one at a time.
        - If they don't have an answer, write [TBD] and move on
     5. When you've worked through every section, output a CLEAN version:
        - Remove THIS instruction block (everything between the ═ lines above)
        - Remove every other <!-- comment --> in the document, including the
          per-section explainer comments
        - Keep only headings + filled-in content
     6. Deliver the file as agreed in step 3 (save to disk, or paste in a
        code block).

     Important:
     - Do not assume you know the user's name. Ask them in this chat.
     - One CONTEXT.md per project. Don't try to mix projects in one file.
     - Keep the final file under 100 lines if you can.
     - "North star" here means the project's direction, not the user's
       personal direction. Personal direction lives in NORTH-STAR.md at the
       workspace root, separately.
══════════════════════════════════════════════════════════════════════════ -->

# CONTEXT.md

<!-- This file is the project-specific context Claude reads when working
     inside this folder. It pairs with the master CLAUDE.md (who you are,
     how you work) and any NORTH-STAR.md you have at the root.
     Together: CLAUDE.md = how, NORTH-STAR.md = why, CONTEXT.md = what this
     project is and where it's going. -->

## What this is

<!-- One paragraph. What the project does, who it's for, what makes it
     different from other things. The elevator pitch a smart friend would
     repeat back to you. -->

[One paragraph. E.g. "An AI-operated handwritten letter service. Customers order online, AI agents handle drafting, calligraphy briefs, and dispatch. Doubles as a working demo of an autonomous business."]

## North star

<!-- Where THIS project is heading. The 1-3 year picture. Specific enough
     to make tradeoffs against, vague enough to survive the journey.
     Different from goals (which are shorter-term and more tactical). -->

[2-3 sentences. E.g. "The default place UK architects go for cladding spec data. Accurate, independent, reference-grade. Free to browse, paid for write access and bulk downloads."]

## Goals (next 3-6 months)

<!-- The concrete milestones that move the project toward the north star.
     Each goal should be specific enough to know if you've hit it. -->

1. [Specific goal. E.g. "Land first 3 paying B2B clients on the £200/month plan"]
2. [Specific goal. E.g. "Add product data for the top 5 suppliers in our category"]
3. [Specific goal]

## Current state

<!-- Where the project actually is right now. Not where you want it to be.
     Stage, status, what's working, what's broken, what's blocked. -->

- **Stage:** [Idea / building / live / scaling / maintenance / paused]
- **Live at:** [URL if applicable]
- **What's working:** [Brief]
- **What's broken or blocked:** [Brief, if anything]
- **Last shipped:** [What and when]

## Active priorities

<!-- This week or this month. The 3-5 things actually getting attention.
     Update this regularly. Stale priorities are worse than no priorities. -->

1. [Top priority]
2. [Second priority]
3. [Third priority]

## Key people for this project

<!-- Who's involved. Clients, collaborators, advisors, contacts.
     Cuts re-explaining people every time you mention them. -->

| Who | Role | Notes |
|-----|------|-------|
| [Name] | [Client / collaborator / advisor / contractor] | [Anything relevant. E.g. "First paying client. Prefers email over Slack."] |
| [Name] | [Role] | [Notes] |

## Files and structure

<!-- Where things live in this project's folder. Where to put new things.
     Where to look for things. Keeps the folder from becoming a junk drawer. -->

```
[project-name]/
├── CONTEXT.md          this file
├── [main-file.md]      [what it is]
├── [folder]/           [what's in it]
└── archive/            old versions go here
```

## Outstanding

<!-- Loose ends. Things half-done, things deferred, things to revisit.
     Better here than scattered across emails and notes. -->

- [Outstanding item, e.g. "V4.5 of the site is ready locally, needs pushing to GitHub"]
- [Outstanding item]
- [Outstanding item]
