# 🔥🃏 life-coach

> **Turn laziness into discipline. Alchemy edition.**
>
> A Claude `.skill` that interviews you through 4 specialist psychologist personas, diagnoses the ROOT cause of your discipline failures (not the surface symptoms), then generates a personalized daily protocol grounded in evidence-based habit research.

```
YOU                       4 PSYCHOLOGIST AGENTS         OUTPUT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Conversation             ┌─────────────────────────┐
with /life-coach  ──────→ │  Behavioral Psych       │ ──→ profile.md
                         │  CBT Therapist          │ ──→ protocol.md
                         │  Performance Coach      │ ──→ personal .skill
                         │  Neuroscientist         │     (your daily driver)
                         └─────────────────────────┘
```

---

## 🎯 Why this is different

Most "discipline" advice fails because it assumes everyone's the same. **Transmute starts with the diagnosis.**

Your specific failure pattern might be:
- 🧪 **Dopamine dysregulation** — phone-first morning, can't engage with effort
- 👤 **Identity mismatch** — saying you want X, behaving as if you want Y
- 🧱 **Environmental design failure** — friction in the wrong direction
- 🔄 **Cognitive distortion** — perfectionism, all-or-nothing thinking
- 🌙 **Sleep/energy debt** — no biological fuel for discipline
- 🛡️ **Avoidance** — "laziness" as emotional regulation

**The protocol you need depends on which root cause is driving you.** Generic tips fail because they ignore which one is yours.

---

## 🚀 How it works

### Phase 1 — Diagnostic Interview (~15 min)
Four specialist personas take turns asking 3-4 questions each:

```
🧠 Behavioral Psychologist  → environment, triggers, current routines
🧠 CBT Therapist            → internal narratives, cognitive distortions
🧠 Performance Coach        → identity, systems, keystone habits
🧠 Neuroscientist           → sleep, dopamine, attention, biology
```

### Phase 2 — Diagnosis Synthesis
All 4 perspectives synthesize into ONE root cause + 1-2 secondary patterns.
Written to `profiles/{user-name}.md`.

### Phase 3 — Protocol Generation
Pulls from 5 evidence-based frameworks:
- **Tiny Habits** (BJ Fogg) — daily anchors
- **Identity-Based Change** (James Clear) — voting for who you want to be
- **CBT Reframes** (Beck/Burns) — failure recovery scripts
- **Dopamine Balance** (Lembke/Huberman) — biological resets
- **Deep Work** (Cal Newport) — for cognitive keystones
- **Circadian Protocol** (Huberman) — sleep/light/timing

Generates `profiles/{user-name}-protocol.md`.

### Phase 4 — Ship as a personal .skill
Your protocol gets bundled as `~/.claude/skills/{user-name}-discipline/SKILL.md`.

You invoke it daily:
```
/{user-name}-discipline
  → "what did you do today?"
  → tracks streaks, adapts when patterns emerge
```

---

## 🛠️ Install

```bash
# Drop into your skills directory
git clone https://github.com/DimmMak/life-coach.git
cd .. && zip -r ~/.claude/skills/life-coach.skill transmute/

# Or copy SKILL.md if you prefer manual setup
mkdir -p ~/.claude/skills/life-coach
cp SKILL.md agents/ frameworks/ schemas/ ~/.claude/skills/life-coach/
```

Then in any Claude Code session:
```
/life-coach
```

---

## 📂 Repo layout

```
transmute/
├── README.md                    # This file
├── SKILL.md                     # The diagnostic + generation protocol
├── agents/                      # 4 psychologist personas
│   ├── behavioral-psychologist.md
│   ├── cbt-therapist.md
│   ├── performance-coach.md
│   └── neuroscientist.md
├── frameworks/                  # 5 evidence-based methods
│   ├── tiny-habits.md           # BJ Fogg
│   ├── identity-based-change.md # James Clear
│   ├── cbt-reframes.md          # Aaron Beck / David Burns
│   ├── dopamine-balance.md      # Anna Lembke / Huberman
│   ├── deep-work.md             # Cal Newport
│   └── circadian-protocol.md    # Huberman / Walker
├── schemas/                     # Output templates
│   ├── PROFILE.template.md
│   └── PROTOCOL.template.md
├── profiles/                    # User-specific output (gitignored in real use)
└── examples/                    # Sample profiles
```

---

## 🎯 Design principles

- **Diagnosis before prescription.** Generic advice fails because it skips diagnosis. We don't.
- **Multi-persona synthesis.** No single psychological lens captures the whole picture.
- **Evidence-based frameworks.** All 5 frameworks have peer-reviewed research backing.
- **Failure budgets baked in.** The "Failure Recovery Script" is mandatory, not optional.
- **Ship as a personal .skill.** The output isn't advice — it's a tool you invoke daily.

---

## 🚫 What this is NOT

- ❌ Therapy (we're not licensed clinicians; we use clinical frameworks for self-improvement)
- ❌ Medical advice (sleep/dopamine recommendations are general, not personalized medicine)
- ❌ A motivational pep-talk system
- ❌ A productivity hack collection
- ❌ Replacement for professional help if you have clinical depression, ADHD, or other conditions

---

## 🔗 Pairs perfectly with...

- [courserafied](https://github.com/DimmMak/courserafied) — ingest a habit-formation course (Tiny Habits, Atomic Habits) for richer framework data
- [cowatch](https://github.com/DimmMak/cowatch) — pull live transcripts from discipline/habit lectures
- [claudenotes](https://github.com/DimmMak/claudenotes) — daily protocol becomes another agent in your factory

---

## 📜 License

MIT — do whatever you want with it.

---

## 🃏 Built by

[@DimmMak](https://github.com/DimmMak) — part of an exploration of `.skill`-based agent factories for self-directed change.

**Sister projects:**
- [cowatch](https://github.com/DimmMak/cowatch) — live lecture co-watcher
- [courserafied](https://github.com/DimmMak/courserafied) — courses → knowledge bases
- [claudenotes](https://github.com/DimmMak/claudenotes) — agent factory > Notion
- [promptlatro](https://github.com/DimmMak/promptlatro) — roguelike that drills prompt patterns
- [coderecall](https://github.com/DimmMak/coderecall) — first-letter recall for SQL/Python

🔥🃏⚡
