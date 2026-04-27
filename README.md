# CONTEXT.md

The project-specific context file. Tells your AI assistant what this project is, where it's going, and what's actually happening right now. One per project.

This is one of a family of five templates that customise AI for the way you actually work.

| Template | What it covers | When to do it |
|----------|----------------|---------------|
| **[CLAUDE.md](https://github.com/catrinmdonnelly/CLAUDE.md)** | Who you are, how you work, what's on your desk | First. Even if you do nothing else, this gets you 70% of the value |
| **[COPY.md](https://github.com/catrinmdonnelly/COPY.md)** | How things should sound. Voice + banned phrases | Second. Voice is the most-violated AI default |
| **[DESIGN.md](https://github.com/catrinmdonnelly/DESIGN.md)** | How things should look. Design tokens + banned aesthetics | Third. Only if you make visual things (websites, slides, social posts) |
| **[CONTEXT.md](https://github.com/catrinmdonnelly/CONTEXT.md)** (this repo) | What each project is and where it's going | Per project, when you start working in a specific folder |
| **[NORTH-STAR.md](https://github.com/catrinmdonnelly/NORTH-STAR.md)** | Career-level direction. The why behind the projects | Last, and only if you have multiple businesses or want to think strategically |

You don't have to do all five. The minimum useful set is **CLAUDE.md + COPY.md**. Add the others as you need them.

They reference each other. Your CLAUDE.md tells AI to read the others when the relevant work comes up, so you do not have to think about which file is needed when.

## Why this exists

Without a CONTEXT.md, every time you open a project folder Claude has to guess what the project is, where it sits, and what's currently going on. That's where the generic, miscalibrated answers come from.

CONTEXT.md fixes it for ONE project. Drop it in the project folder. Claude reads it on every session inside that folder. Suddenly Claude knows that "the site" means your actual production URL, that "the redesign" is what's blocked, and that "the main client" is the specific company you're working with.

The pattern works at scale. If you have ten projects, you have ten CONTEXT.md files, each tightly scoped to its project. Claude only loads the relevant one (the one in the folder you're working in). No bleed, no clutter, no 5,000-line master file.

## Built on the work of others

The per-project context file pattern isn't new. If anything in here is good, the credit goes to:

- **[Anthropic](https://code.claude.com/docs/en/best-practices)** for making Claude Code project-aware: it automatically loads CLAUDE.md from the project folder, which is what makes the per-folder pattern viable. This template is the "what to put in it" template.
- **[Garry Tan / gstack](https://github.com/garrytan/gstack)** for the per-project CLAUDE.md pattern at scale, including subdirectory context files that load on demand.

What's mine is the structure (north star + goals + state + priorities + people + files + outstanding), the HTML-comment guided pattern, and the explicit separation from CLAUDE.md (operational) and NORTH-STAR.md (visionary).

## How it fits with the other files

| File | Scope | Loaded when |
|------|-------|-------------|
| **CLAUDE.md** | You as a person, how you work | Every session, automatically |
| **NORTH-STAR.md** | Your career-level direction | When strategic questions come up (CLAUDE.md tells Claude to load it) |
| **CONTEXT.md** (per project) | What this project is and where it's going | When working in that project folder |
| **DESIGN.md / COPY.md** | Visual / voice rules | When the relevant work comes up (CLAUDE.md tells Claude to load them) |

This scoping is how you avoid duplicates. Each piece of information lives in one place, loaded at the right time.

## Who it's for

- **Solo founders** running one or more projects who want consistent context across all of them
- **Consultants** who handle multiple client projects and need each one's state at hand
- **Anyone using Claude Code or Cursor** with multiple folders on their machine
- **Small teams** sharing a project's state via git

## What's in this repo

| File | What |
|------|------|
| `CONTEXT.md` | The template. Drop it in any project folder, walk through with Claude, save the clean version. |

The template uses HTML comments throughout. When the user pastes it into Claude, the meta-instruction at the top tells Claude to walk them through it section by section, then strip the comments and save a clean file. Non-technical users get a guided experience. Technical users can edit it directly.

## How to use

There are two ways:

### Conversational (the easy way)
1. Copy the contents of `CONTEXT.md` from this repo
2. Paste it into a Claude chat
3. Tell Claude which project folder it's for
4. Answer the questions Claude asks, one at a time
5. Claude outputs a clean CONTEXT.md (no comments) ready to save

### Manual
1. Copy `CONTEXT.md` to your project folder
2. Open it in any text editor
3. Read the HTML comments to understand each section
4. Fill in the bracketed bits, delete the comments
5. Save

## Sections in the template

| Section | What it captures |
|---------|------------------|
| **What this is** | One-paragraph description. The elevator pitch. |
| **North star** | Where this project is heading (1-3 years). Specific enough to make tradeoffs against. |
| **Goals (next 3-6 months)** | Concrete milestones. Specific enough to know if you've hit them. |
| **Current state** | Where the project actually is right now. Stage, what's working, what's blocked. |
| **Active priorities** | The 3-5 things getting attention this week or month. |
| **Key people** | Clients, collaborators, advisors. Who's relevant to this project specifically. |
| **Files and structure** | ASCII tree of the project folder. Where things live. |
| **Outstanding** | Loose ends. Things half-done or deferred. |

## What goes in CONTEXT.md vs CLAUDE.md vs NORTH-STAR.md

This is the structure that confuses people most. Quick guide:

| Question | Where it lives |
|----------|----------------|
| "Who am I?" | CLAUDE.md |
| "How do I want my AI to talk to me?" | CLAUDE.md |
| "Where am I heading in life and career?" | NORTH-STAR.md |
| "Where is this project heading?" | CONTEXT.md (this file) |
| "What's the project's current state?" | CONTEXT.md |
| "What's on my desk this month?" | CLAUDE.md (Current priorities) |
| "What's on this project's desk this month?" | CONTEXT.md (Active priorities) |

The trick is to keep each scoped tightly. CLAUDE.md is operational and personal. NORTH-STAR.md is visionary and personal. CONTEXT.md is operational and project-specific.

## License

MIT. Do whatever you want with it. Credit appreciated, not required.

Made by [Catrin Donnelly](https://catrinmd.netlify.app), North Wales.
