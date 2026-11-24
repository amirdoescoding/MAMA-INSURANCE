# Architecture Overview

Living map of the repo. Update when the structure changes.

## 1. Project structure

```
MAMA-INSURANCE/
├── .claude/              # Agent setup: CLAUDE.md, DESIGN.md, MEMORY.md, RESTART.md, TODOS.md, agents/, skills/
├── assets/
│   ├── Brand kit/        # Logos (orange, white), Mama m.svg, brand kit docx, company deck pptx
│   ├── design/           # Brand reference board (canvas-design)
│   └── videos/           # Screen recordings
├── data/                 # D1 Household survey, D2 Search demand, D3 Funnel benchmarks (xlsx, synthetic)
├── docs/                 # Case brief, data analysis report, research, extracted/ (text of binary docs)
├── graphify-out/         # Knowledge graph, local only (gitignored)
└── .graphifyignore       # Paths kept out of the graph
```

## 2. Flow

```
D1, D2, D3 + public data ──> analysis ──> strategy memo, marketing plan, pitch
                                            │
Free tool (TBD) ──> core task ──> consent ──> "Fai un preventivo" (UTM) ──> mamainsurance.it quote ──> policy
       └──────────── every step logged ──> funnel dashboard
```

## 3. Tool stack

**TBD**, decided once the tool is chosen (≥8 ideas scored). Constraints: mobile first, live at a public link,
built with AI coding tools, free-plan hosting where possible, funnel events recorded, follows `.claude/DESIGN.md`.

## 4. External

- mamainsurance.it: every policy is sold there; quote link carries `utm_source=mama_tools`.

## 5. Last update

2026-11-24
