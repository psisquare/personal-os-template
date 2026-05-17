# Personal OS Template

A Claude Code workspace scaffold that turns into your personalized second brain in minutes.

---

## What is a Personal OS?

A Personal OS is a structured local folder that Claude Code uses as persistent context about you — your role, your people, your commitments, your decisions. It's not a note-taking app or a project manager. It's the **WHY layer** that makes Claude's advice actually useful to your specific situation.

Once set up:
- Claude knows your key people and how they communicate
- Claude tracks your commitments and decisions without you re-explaining every session
- Every answer is grounded in your actual context, not generic advice
- Memory persists across sessions via `.claude/projects/memory/`

Works for any domain: engineering, coaching, consulting, product, research, operations.

---

## Setup

### 1. Download the template

**Option A — Download ZIP (easiest, no Git needed)**

1. Click the green **Code** button at the top of this page
2. Click **Download ZIP**
3. Unzip the file anywhere on your computer (Desktop, Documents, etc.)
4. Rename the folder to something meaningful, e.g. `my-os`

**Option B — GitHub Desktop (visual Git app)**

1. Install [GitHub Desktop](https://desktop.github.com) if you haven't
2. Click the green **Code** button → **Open with GitHub Desktop**
3. Choose where to save it on your computer

**Option C — Terminal (for developers)**

```bash
git clone https://github.com/psisquare/personal-os-template.git my-os
cd my-os
```

### 2. Open in Claude Code

```bash
claude
```

### 3. Run the setup prompt

Paste this into Claude Code. It will interview you in batches and fill everything in:

```
Set up my personal OS workspace.

1. Read current directory structure
2. Interview me in batches (max 3 questions at a time) — gather only what's needed to
   populate context
3. Fill files + create any missing folders the OS needs

Fill these:
- `CLAUDE.md` — role, tools, domain terms, working style
- `context/people.md` — key people, roles, communication style
- `context/cadences.md` — recurring meetings, reporting beats
- `context/commitments.md` — promises, to whom, by when
- `MOC.md` — owner, entry point links

Memory (`.claude/projects/<dir>/memory/`):
- `user_role.md`, `project_active.md`, `reference_tools.md`, `feedback_work_mode.md`
  (stub), `MEMORY.md` (index)

Create if missing: `inbox/` `context/` `projects/` `meetings/` `log/` `writing/`
Ask first: do I manage people? do I report upward? → create `people/` `one-on-ones/`
`updates/` if yes.

Rules: absolute dates only · leave blanks if unanswered · link don't duplicate · never
invent

Done: print files created/updated → suggest 3 next steps → stop.
```

Claude will interview you, fill the files, and set up memory. Takes ~5 minutes.

---

## Folder structure

```
my-os/
├── CLAUDE.md              # Claude's instructions for this vault
├── MOC.md                 # Map of contents — start here
├── README.md              # This file
├── inbox/                 # Capture first, sort later
├── context/
│   ├── people.md          # Key people + relationships
│   ├── cadences.md        # Recurring rhythms + deadlines
│   ├── commitments.md     # Promises, append-only log
│   └── decisions.md       # Decision log, append-only
├── projects/              # One file per project
├── meetings/              # Processed notes + _inbox/ for raw
├── log/                   # Dated captures: moments, learnings, ideas
├── people/                # People profiles (created if you manage people)
├── one-on-ones/           # 1:1 notes (created if you manage people)
└── writing/               # Polished output worth keeping
```

---

## Design principles

- **Link, don't duplicate** — external tools stay authoritative; this OS links to them
- **Append-only logs** — `decisions.md` and `commitments.md` never lose history
- **Inbox first** — capture without friction, sort later
- **Absolute dates** — no "next Thursday", always YYYY-MM-DD
- **Context layer** — `context/` is the WHY behind every Claude recommendation
- **No speculation** — Claude never invents data or creates folders without need

---

## Requirements

- [Claude Code](https://claude.ai/code) (CLI or desktop app)
- Claude Pro plan or higher (required for Claude Code access)
