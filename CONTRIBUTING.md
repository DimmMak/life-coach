# 🤝 Contributing to transmute

PRs welcome. Highest-impact contributions:

---

## 🧠 New psychologist agents

Current roster covers 4 major lineages (behavioral, cognitive, performance, neuroscience). Other perspectives worth adding:
- **Acceptance & Commitment Therapy (ACT)** — values-based, defusion from thoughts
- **Internal Family Systems (IFS)** — "parts" that drive procrastination vs parts that drive discipline
- **Stoic philosopher** — Marcus Aurelius / Epictetus lineage on voluntary discomfort
- **Attachment theorist** — how relational patterns drive self-discipline

Each agent is its own markdown file in `agents/` following the existing template:
- Identity + lineage
- Core beliefs (bullet list)
- 4-6 diagnostic questions
- What to listen for
- Red flags
- Diagnostic output format
- Don't / Do lists

---

## 📚 New frameworks

Evidence-based methods we don't yet cover:
- **Implementation intentions** (Peter Gollwitzer) — "if X then Y" planning
- **The 5AM Club** (Robin Sharma) — morning routine architecture
- **GTD** (David Allen) — external memory for reduced cognitive load
- **Oblique strategies** (Brian Eno) — for creative blocks specifically
- **The Power of Habit** (Charles Duhigg) — habit loop model

Bar: must have **peer-reviewed research OR decades of clinical use** behind it. No self-help fluff.

---

## 📐 New output schemas

If you find a diagnostic or protocol category we miss:
1. Create `schemas/{NAME}.template.md` following existing format
2. Update `SKILL.md` to reference it
3. PR with rationale

---

## 🐛 Bug reports

Open an issue with:
- Your profile (sanitized — no personal info needed)
- Which framework was applied
- Where the protocol felt generic vs personalized
- What you expected vs got

---

## 🚫 We reject contributions that...

- Recommend specific supplements or drugs (liability, not our lane)
- Moralize about laziness as character flaw
- Use pseudoscience (crystals, astrology, etc.)
- Promote specific commercial products
- Give clinical advice (this isn't therapy)

---

## 📜 Code style

- Markdown with functional emojis paired
- Cite sources (books, papers, podcasts) in each framework file
- Templates must work for ANY user — no embedded personal info

---

🔥🃏 Thanks for contributing.
