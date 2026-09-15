# Project Management Agent

The Project Management Agent is a specialist agent designed to support a broader Chief of Staff Agent. It converts authorized initiatives into executable plans, monitors delivery, manages change, and maintains project risks, assumptions, issues, dependencies, and decisions.

This repository is an early prototype exploring how specialized agents can improve executive visibility, project accountability, and delivery decisions.

## Role in the Agent System

The Chief of Staff Agent acts as the orchestrator. It assigns project-management work to the Project Management Agent and combines its findings with input from other specialist agents.

The Project Management Agent may recommend involvement from:

- Innovation Agent for value, feasibility, or solution-design questions
- Compliance Agent for requirements, controls, approvals, and compliance readiness
- Data Analyst Agent for baselines, forecasting, performance measures, and quantitative validation

The Project Management Agent provides planning and delivery-management support. It does not authorize initiatives, approve funding or changes, commit resources, accept risk, or make executive decisions.

## Core Skills

### 1. Project Planning and Mobilization

Converts an authorized initiative into an executable plan with defined scope, deliverables, acceptance criteria, milestones, ownership, dependencies, resources, governance, and success measures.

[View the Project Planning and Mobilization skill](.agents/skills/project-planning-mobilization/SKILL.md)

### 2. Execution and Status Management

Monitors delivery against approved scope, schedule, budget, resource, quality, and benefits expectations. It identifies variances, manages change information, recommends corrective actions, and produces executive status reporting.

[View the Execution and Status Management skill](.agents/skills/execution-status-management/SKILL.md)

### 3. RAID and Decision Management

Identifies, evaluates, tracks, and escalates project risks, assumptions, issues, dependencies, and decisions.

[View the RAID and Decision Management skill](.agents/skills/raid-decision-management/SKILL.md)

## Typical Workflow

1. Convert an authorized initiative into an executable project plan.
2. Establish milestones, ownership, governance, and success measures.
3. Monitor delivery and compare actual progress with the approved baseline.
4. Manage variances, changes, corrective actions, and forecasts.
5. Track RAID items and decisions throughout the project lifecycle.
6. Escalate material blockers, tradeoffs, and decisions to the Chief of Staff Agent.

Not every assignment requires all three skills. The agent begins at the stage appropriate to the project’s authorization, available evidence, and current lifecycle phase.

## Example Use Case

**Assignment:** Develop and manage a pilot for an AI tool that summarizes executive meeting materials.

The Project Management Agent can:

- Translate the approved pilot into scope, deliverables, milestones, owners, and acceptance criteria
- Incorporate compliance reviews and data-measurement requirements into the plan
- Track progress, variances, changes, and upcoming milestones
- Maintain risks, assumptions, issues, dependencies, and decisions
- Identify recovery options and leadership decisions
- Provide the Chief of Staff Agent with a concise delivery-health summary

## Repository Structure

```text
project_management_agent/
├── AGENTS.md
├── README.md
└── .agents/
    └── skills/
        ├── project-planning-mobilization/
        │   └── SKILL.md
        ├── execution-status-management/
        │   └── SKILL.md
        └── raid-decision-management/
            └── SKILL.md
```

## Status

Early-stage prototype for professional development and concept validation. The current version establishes the Project Management Agent’s role, routing instructions, core skills, outputs, handoffs, evidence expectations, and guardrails.
