# real-estate

A personal Claude Code skill repo for managing a custom home build and learning the real estate / general contracting trade.

## What this is

A set of slash commands (skills) that turn Claude Code into a structured assistant for every phase of a custom home build — from lot analysis through closeout — while building transferable GC knowledge along the way.

## Skills

### Pre-design
| Skill | What it does |
|-------|-------------|
| `/lot-analysis` | Assess zoning, setbacks, buildable area, utilities, soil, slope |
| `/budget-plan` | Build a realistic budget: hard costs, soft costs, contingency, financing |
| `/architect-brief` | Turn family needs/wants into a structured program for an architect |

### Design & permitting
| Skill | What it does |
|-------|-------------|
| `/plan-review` | Review drawings for constructability, code issues, value engineering |
| `/permit-tracker` | Track permits, submissions, comment responses, inspection sequence |
| `/spec-review` | Review project specs for gaps, ambiguity, owner-unfavorable language |

### Builder selection
| Skill | What it does |
|-------|-------------|
| `/bid-leveling` | Compare bids apples-to-apples, normalize scope gaps, flag lowball traps |
| `/builder-due-diligence` | Research a builder: license, insurance, liens, references |
| `/contract-review` | Red-flag a construction contract: payment terms, change orders, disputes |

### Construction
| Skill | What it does |
|-------|-------------|
| `/schedule-review` | Critique a construction schedule for realistic sequencing and float |
| `/inspection-prep` | Checklists for each inspection: framing, rough-in, insulation, final |
| `/change-order-review` | Evaluate a change order: scope, price, fault |
| `/draw-review` | Review a payment draw request against schedule and completion |
| `/site-visit` | Structured site visit checklist for a specific phase |

### Closeout
| Skill | What it does |
|-------|-------------|
| `/punch-list` | Generate and track a punch list by trade |
| `/warranty-tracker` | Document warranties, specs, maintenance schedules |

### Learning track
| Skill | What it does |
|-------|-------------|
| `/learn-trade` | Deep dive on a trade: electrical, plumbing, HVAC, structural, framing |
| `/cost-estimate` | Learn to estimate a scope item: materials + labor + overhead + margin |
| `/code-lookup` | Research building code requirements for your jurisdiction |
| `/gc-license-path` | Research GC licensing requirements, exam prep, experience hours |
| `/debrief` | After any phase, extract lessons learned into KNOWLEDGE.md |

## Key workflows

**Starting the project:**
```
/lot-analysis → /budget-plan → /architect-brief
```

**Choosing a builder:**
```
/builder-due-diligence → /bid-leveling → /contract-review
```

**During construction (recurring):**
```
/site-visit → /draw-review → /change-order-review (as needed)
```

**Learning loop:**
```
/debrief → updates KNOWLEDGE.md
```

## Setup

```bash
./setup    # register all skills with Claude Code
```

## Project files

- `KNOWLEDGE.md` — living document of lessons learned (written by /debrief)
- `budget.md` — actual project budget tracked across phases
- `project.md` — project details: lot address, key contacts, timeline, current phase
