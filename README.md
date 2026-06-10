# Antikode Lead Radar — How to Use

Skill file: `antikode-lead-radar-1.3.0.skill`
Output: a single Markdown (`.md`) lead intelligence report. No HTML.

---

## What it does

Generates a BD lead research report for Antikode pitches. For each lead it
finds and verifies:

- Company basics + a 1–10 fit score with rationale
- Client / outlet portfolio (10+) mapped by loyalty status
- 3–5 direct competitors and their loyalty schemes
- 2–4 decision-maker contacts (Manager–VP) with LinkedIn search links
- 2–3 current promotions running now
- Value proposition + outreach strategy tailored to Antikode
- 4+ source links behind every major claim

---

## How to run it

Say any of these:

- "run lead radar"
- "generate leads"
- "find leads for antikode"
- "start the lead form"
- "lead research"

Claude goes straight to the intake form. No setup needed.

---

## The 4 questions

A single form (one screen) asks:

1. **Geography** — Indonesia, Singapore, Malaysia, SEA, or Other
2. **Project types to pitch** — loyalty app, revamp, gamification, web redesign (pick any)
3. **Company size** — Enterprise (50+), Mid-market (10–50), or Both
4. **How many leads** — 3, 5, 8, or 10 (5 recommended)

PIC depth is fixed at Manager-to-VP. There is no styling question — the
output is plain Markdown.

---

## Optional: upload a credential deck first

Before the form, Claude asks if you have a pitch/credential PDF.

- Upload one → outreach strategies get personalized with your real proof points.
- Skip it → defaults to known Antikode clients (HokBen, Maybank, AXIS, Paragon Corp, Tzu Chi Hospital).

---

## What you get

A file at:

```
leads/antikode-leads-[geography]-[YYYY-MM].md
```

Plain Markdown, sorted by score. Each lead has 9 sections: Score Rationale,
Client Portfolio, Competitors, PICs, Promos, Value Prop, Outreach Strategy,
Conversation Starters, Sources.

Use it directly:
- Paste into a Lark Doc or deck
- Drop into Obsidian
- View on GitHub
- Edit in any text editor

---

## Scoring quick reference

| Signal | Score |
|---|---|
| No loyalty app + enterprise scale + expansion | 9–10 |
| Basic program + clear gap + good size fit | 7–8 |
| Has program, strategic but less urgent | 5–6 |

Modifiers: +1 if their own clients lack loyalty, +1 if competitors are weak,
+1 if only running generic promos, −1 if they already run mature gamification.

---

## Notes

- All companies are real and web-searched — no placeholders, no hallucinated names.
- Each lead carries a ✓ Verified / ⚠ Unverified flag based on live sources.
- Output is Markdown only. The old HTML/React report (v1.2.0) is retired.

---

## Version history

- **v1.3.0** — Markdown-only output. Styling/HTML removed. Research depth unchanged.
- **v1.2.0** — HTML report (React + Babel CDN) with verification, portfolio mapping, competitor schemes, multi-PIC, promos, sources.
- **v1.0.0** — Initial HTML lead report.
