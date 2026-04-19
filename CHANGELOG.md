# 📜 transmute Changelog

## v0.2.0 — 2026-04-18

**World-Class Overhaul shipped.** Part of the fleet-wide upgrade to tree+plugin+unix architecture.

- 🌳 **Tree:** `domain:` field added to frontmatter (general)
- 🎮 **Plugin:** `capabilities:` block declares reads / writes / calls / cannot
- 🐧 **Unix:** `unix_contract:` block declares data_format / schema_version / stdin_support / stdout_format / composable_with
- 🛡️ Schema v0.3 validation required at install (via `future-proof/scripts/validate-skill.py`)
- 🔗 Install converted to symlink pattern (kills drift between Desktop source and live install)
- 🏷️ Tagged at `v-2026-04-18-world-class` for rollback

See `memory/project_world_class_architecture.md` for the full model.

---


## v1.0.0 — 2026-04-16 — Initial Release

### 🚀 Shipped
- **`SKILL.md`** — 6-step diagnostic + protocol-generation flow
  - STEP 1: Pre-flight (load agents, frameworks, schemas, existing profile)
  - STEP 2: Multi-persona diagnostic interview (4 psychologists take turns)
  - STEP 3: Diagnosis synthesis (root cause, not symptoms)
  - STEP 4: Protocol generation (pulls from 5 frameworks)
  - STEP 5: Ship as personal `.skill` (daily driver)
  - STEP 6: Report + next steps

- **4 psychologist personas** in `agents/`:
  - `behavioral-psychologist.md` — BJ Fogg / Skinner lineage (environment, triggers, routines)
  - `cbt-therapist.md` — Aaron Beck / David Burns lineage (cognitive distortions, inner dialogue)
  - `performance-coach.md` — James Clear / Cal Newport lineage (identity, systems, keystone habits)
  - `neuroscientist.md` — Huberman / Lembke lineage (sleep, dopamine, attention, biology)

- **6 evidence-based frameworks** in `frameworks/`:
  - `tiny-habits.md` — BJ Fogg's B=MAP formula, anchors, celebration
  - `identity-based-change.md` — James Clear's identity declarations, daily votes
  - `cbt-reframes.md` — Burns's 10 cognitive distortions + reframe protocol
  - `dopamine-balance.md` — Lembke's detox + rebuild + maintain phases
  - `deep-work.md` — Newport's 4 philosophies, rhythmic protocol template
  - `circadian-protocol.md` — Huberman's wake/sleep non-negotiables

- **2 output schemas** in `schemas/`:
  - `PROFILE.template.md` — 5-section diagnostic output (behavioral/cognitive/performance/biological/synthesis)
  - `PROTOCOL.template.md` — identity declaration, daily anchors, circadian anchors, weekly rituals, failure recovery script, 30-day milestone

- **README.md** — pitch, how it works, install, integration with sister projects
- **CONTRIBUTING.md** — guide for adding new frameworks, agents, schemas
- **MIT LICENSE**
- **.gitignore**

### 💡 Design principles
- **Diagnosis before prescription.** Generic advice fails because it skips diagnosis.
- **Multi-persona synthesis.** No single lens captures the whole picture.
- **Evidence-based only.** Every framework has peer-reviewed research backing.
- **Failure budgets baked in.** "Failure Recovery Script" is mandatory, not optional.
- **Ship as a personal `.skill`.** Output isn't advice — it's a daily tool.

### 🔗 Spawned from
Created during a long building session exploring `.skill`-based agent factories. Emerged from the insight that generic productivity advice fails because it skips the diagnostic step — and that multi-persona interviews produce better diagnoses than single-lens ones.

🔥🃏⚡
