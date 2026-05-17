# CLAUDE.md — Personal OS

Personal workspace OS. Read `context/` before advising.

---

## Who uses this

- **[Owner]** — [role]
- **[Person 2]**, **[Person 3]** — [relationship/role]
- **[Primary tool]** — [purpose]

---

## Always

- **Date everything** — convert "Thursday" / "next week" to absolute YYYY-MM-DD
- **Cite sources** — link to meeting note, tool record, or person who said it
- **Tight structure** — tables, bullets, headings. No long paragraphs
- **Preserve domain terms verbatim** — don't paraphrase jargon
- **Read `context/` first** — it's the WHY layer before any recommendation
- **Unsure where something goes → `inbox/`**
- **Decision changes → update every file that references it**

---

## Never

- Write into external tools — link instead
- Share or publish content externally without confirmation
- Create new folders speculatively — only when a real need appears
- Edit old rows in `context/decisions.md` or `context/commitments.md` — append only

---

## File conventions

| Pattern | Location |
|---------|---------|
| Raw capture, unsorted | `inbox/` |
| Processed meeting notes | `meetings/YYYY-MM-DD-[person-or-topic].md` |
| Unprocessed meeting notes | `meetings/_inbox/` |
| Project files | `projects/[project-slug].md` |
| People profiles | `people/[name].md` |
| 1:1 session notes | `one-on-ones/YYYY-MM-DD-[name].md` |
| Dated log entries | `log/YYYY-MM-DD-[slug].md` |
| Polished writing | `writing/[slug].md` |

---

## External systems

- **[Tool name]** — [purpose]. Link records, don't copy.

---

## Decision log format

`context/decisions.md` — append only. Format:

```
| D-NNN | YYYY-MM-DD | [Title] | [Decision] | [Rationale] |
```

## Commitments format

`context/commitments.md` — append only. Format:

```
| YYYY-MM-DD | [To whom] | [What] | [Due YYYY-MM-DD] | [Status] |
```
