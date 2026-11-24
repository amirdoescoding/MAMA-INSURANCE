# MAMA TOOLS BDD

## 0. Project context

Albert School 2nd-year Business Deep Dive with **Mama Insurance** (Italian AI native MGA, home insurance sold on
mamainsurance.it). We are the **Head of Mama Tools**: build a free tool that reaches Italians who have never
searched for home insurance and turns users into policyholders without losing their trust.
Final pitch to CEO, CMO (Giulia Ferraris) and CFO (Marco Bellini, the hardest to convince).

- **Targets at month 6:** 90,000 activated users, 600 paid policies started in the tool, credible path to a
  12-month cost per policy < €110 (vs ~€70 on paid channels). €120k pays months 1 to 6; months 7 to 12 costs
  must also be budgeted and count in the 12-month cost per policy.
- **Rules:** no lease contract generator (Exhibit 2). Core task works with no purchase. Insurance offer optional
  and clearly separate. Policy sold only on mamainsurance.it. Live by the final, tried by ≥5 people outside the
  squad. Marketing consent separate and explicit. Disclaimer on any legal, fiscal or technical advice. Every
  funnel step tracked.
- **Deliverables:** 4-page strategy memo (≥8 tool ideas scored), live tool + 1-page build log, marketing plan
  (monthly cost table ≤ €120k, funnel at M6 and M12, 3 KPIs with triggers, 2 month-1 experiments), 10-min pitch
  opening with a live demo.
- **Grading:** working tool 50% (usefulness 20, build quality 15, bridge to insurance + measurement 15),
  analysis 15, strategy 15, marketing plan 15, clarity 5.
- **Brief:** `docs/Mama Tools_ Building Demand Before It Exists (case).docx`. Company deck:
  `assets/Brand kit/Mama Insurance company presentation (English).pptx` (text in `docs/extracted/`).
- **Data:** `data/D1 Household survey.xlsx` (500 respondents, duplicates, free text),
  `data/D2 Search demand.xlsx` (50 keywords, Dec 2025 to Nov 2026, brand and generic mixed),
  `data/D3 Funnel benchmarks.xlsx` (some rates monthly, others per user). Analysis:
  `docs/Mama Tools - Data analysis report.pdf`. Research: `docs/Home_and_content_insurance_research.md`.
- Every number maps to D1 to D3 or a named public source (ISTAT, ANIA, Google Trends, rate cards). State VAT on
  every price. No automated scraping of third-party sites. Case data is synthetic. Key facts in @MEMORY.md.

## Design

- UI and every visual deliverable (tool, memo, deck) follow @DESIGN.md (brand kit + mamainsurance.it).
- Exhibit 5 checklist in DESIGN.md is the tool's definition of done.

## Context via Graphify (read first)

- **Before starting any task**, query the knowledge graph in `graphify-out/` first:
  `graphify query "<question>"`, `graphify path "<A>" "<B>"`, `graphify explain "<node>"`.
  Read only the files the graph points to. `graphify-out/GRAPH_REPORT.md` is for broad overviews.
- Graph covers `docs/`, `data/`, `assets/Brand kit/` and `.claude/*.md`. Noise is excluded in `.graphifyignore`.
- After code changes, run `graphify update .` (AST-only, free; the post-commit hook does it too).
  After doc/data changes, run `/graphify . --update`.
- `graphify-out/` is gitignored; each teammate builds it locally with `/graphify .`. First install the
  extras so docx/xlsx/pdf are read: `uv tool install "graphifyy[office,pdf]"`.

## gstack

Use /browse from gstack for all web browsing. Never use mcp__claude-in-chrome__* tools.
Lean on `/office-hours` and `/plan-ceo-review` for strategy, `/qa` for the live tool, `/review` before merging,
`/context-save` and `/context-restore` between sessions.

## Agents and skills

- Always use the relevant subagents (`.claude/agents/`) and skills for the task: gstack, canvas-design,
  impeccable, xlsx/docx/pptx/pdf, dataviz. Run independent work in parallel.

## **GIT**

- Always create a new branch for every new feature. Never work on `main`.
- Split work into small, focused commits.

## 1. Think Before Coding

**Don't assume. Don't hide confusion. Surface tradeoffs.**

Before implementing:

- State your assumptions explicitly. If uncertain, ask.
- If multiple interpretations exist, present them - don't pick silently.
- If a simpler approach exists, say so. Push back when warranted.
- If something is unclear, stop. Name what's confusing. Ask.

## 2. Simplicity First

**Minimum code that solves the problem. Nothing speculative.**

- No features beyond what was asked.
- No abstractions for single-use code.
- No "flexibility" or "configurability" that wasn't requested.
- No error handling for impossible scenarios.
- If you write 200 lines and it could be 50, rewrite it.

Ask yourself: "Would a senior engineer say this is overcomplicated?" If yes, simplify.

## 3. Surgical Changes

**Touch only what you must. Clean up only your own mess.**

When editing existing code:

- Don't "improve" adjacent code, comments, or formatting.
- Don't refactor things that aren't broken.
- Match existing style, even if you'd do it differently.
- If you notice unrelated dead code, mention it - don't delete it.

When your changes create orphans:

- Remove imports/variables/functions that YOUR changes made unused.
- Don't remove pre-existing dead code unless asked.

The test: Every changed line should trace directly to the user's request.

## 4. Goal-Driven Execution

**Define success criteria. Loop until verified.**

Transform tasks into verifiable goals:

- "Add validation" → "Write tests for invalid inputs, then make them pass"
- "Fix the bug" → "Write a test that reproduces it, then make it pass"
- "Refactor X" → "Ensure tests pass before and after"

For multi-step tasks, state a brief plan:

```
1. [Step] → verify: [check]
2. [Step] → verify: [check]
3. [Step] → verify: [check]
```

Strong success criteria let you loop independently. Weak criteria ("make it work") require constant
clarification.

---

**These guidelines are working if:** fewer unnecessary changes in diffs, fewer rewrites due to
overcomplication, and clarifying questions come before implementation rather than after mistakes.

---

## Session close

1) Run `/qa` (when the tool exists), write the recap + self-rating to `.logs/YYYY-MM/DD/<slug>.md`.
2) Update @MEMORY.md with key facts & decisions so far
3) Update @RESTART.md with what you were doing and where you stopped
4) Update the backlog in @TODOS.md with everything still left to do
5) Update @ARCHITECTURE.md if any changes were made to the structure
