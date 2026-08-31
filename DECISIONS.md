# DECISIONS — repo level

> One entry per significant choice. Format for each: **the decision · alternatives considered · why · what would change my mind.**
> Hiring managers often read this file first — it shows reasoning, which is the actual job.

---

## D-001: One monorepo instead of four repos

- **Decision.** Keep all four portfolio projects in a single `ai-pm-portfolio` repo, organized by `projects/` (the showcase) and `phase-N/day-NN/` (daily notes).
- **Alternatives considered.**
  - *Four separate repos*, one per project (what the source plan literally suggests, and what GitHub's "pin 4–6 repos" model rewards).
  - *Monorepo* (chosen).
- **Why.** At Day 11, one continuously-updated repo tells a single coherent story and is far cheaper to maintain daily; the narrative and cross-project through-line stay in one place. The main cost — GitHub pins repos, not folders, so I can only pin one thing — is mitigated by making *this README* do the curation work: it foregrounds the four projects with status and direct links, which is what pinning would otherwise achieve.
- **What would change my mind.** If the capstone (Project 4) becomes a genuinely standalone launched product with its own users, it earns its own repo so it can be starred, forked, and pinned independently — I'll split it out then and cross-link.

---

## D-002: Projects are the spine; daily notes are the depth layer

- **Decision.** Foreground `projects/` in the README and top-level navigation; keep `phase-N/day-NN/` folders as the working log that project READMEs reference.
- **Alternatives considered.** Organize purely by day (chronological), or purely by project (no visible daily cadence).
- **Why.** Recruiters care about 3–5 deep projects, not 90 day-folders — so projects lead. But the daily folders are evidence of consistency and show reasoning as it formed, which reads well to engineers. Keeping both, with projects on top, serves both readers.
- **What would change my mind.** If the daily folders start diluting the showcase (a reviewer gets lost), collapse older days into a single phase summary and keep only project folders prominent.

---

## D-003: Status is shown honestly, including "not done yet"

- **Decision.** Use ✅ / 🚧 / ⏳ status markers and truthful "starts Day NN" labels rather than presenting a finished-looking portfolio.
- **Alternatives considered.** Hide unfinished work; only publish once all four projects are complete.
- **Why.** The whole positioning depends on honesty reading as senior. Documenting failures and in-progress state publicly is a feature, not a liability, for this audience.
- **What would change my mind.** Nothing on honesty. If a specific unfinished stub looks like clutter, I'll hide the folder until there's real content, but I won't fake completion.

<!-- Add D-004+ as real choices arise: model selection, RAG vs fine-tune, pricing assumptions, eval design, etc. -->
