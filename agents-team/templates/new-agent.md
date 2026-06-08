# Agent Name

> One-line description of who this agent is and what it is responsible for.

## Identity & Role

Define who this agent is and how it fits into the team.

- **Name:**
- **Role:** What seat does this agent hold on the team?
- **Mission:** What outcomes is it accountable for?
- **Tone:** How should it communicate (e.g. direct, thorough, concise)?

## Specialty

The domain expertise and task types this agent owns.

- Primary focus areas
- Types of work it should accept vs. decline
- What makes this agent the right choice over others

## Loaded Skills (links to skill files)

Skills this agent should read and apply. Link to skill files under `skills/`.

| Skill | Path | When to use |
|-------|------|-------------|
| | `../skills/example-skill.md` | |

## System Prompt

The core instruction block that defines how this agent operates. Write in second person, as if speaking directly to the agent.

```
You are [Agent Name], a [role] on the MyTeam agents team.

Your job is to …

You specialize in …

When working, you …

You defer to other agents when …
```

## Behavioral Rules

Day-to-day habits and decision patterns beyond the system prompt.

- Always …
- Prefer …
- Ask clarifying questions when …
- Escalate or hand off when …
- Confirm before …

## Constraints

Hard limits this agent must never cross. Align with team-wide rules in `../context/constraints.md` where applicable.

- Do …
- Do not …
- Never …
- Must verify … before …

## Bootstrap Block

Paste-ready block to initialize a session with this agent. Include identity, loaded skills, and context files in one shot.

```
# Agent Bootstrap: [Agent Name]

## Identity
[Copy or summarize Identity & Role + Specialty]

## Skills to load
- ../skills/example-skill.md

## Context to load
- ../context/active-projects.md
- ../context/brand-voice.md
- ../context/constraints.md

## Session start
1. Read the skills and context files above.
2. Confirm the user's goal and any missing inputs.
3. Proceed using your System Prompt and Behavioral Rules.
```

## Context Files to Load

Shared context this agent should read at session start or when relevant.

| File | Path | Purpose |
|------|------|---------|
| Active projects | `../context/active-projects.md` | Current work in flight |
| Brand voice | `../context/brand-voice.md` | Tone and communication style |
| Constraints | `../context/constraints.md` | Team-wide guardrails |
