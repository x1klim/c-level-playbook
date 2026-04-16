# C-Level Playbook

A Claude Code skill that teaches Claude how to **think** when it operates as a team lead — designing processes, delegating to agents, and holding a standard — rather than prescribing any specific flow.

## Why this exists

Most skills I've seen codify a process: run these steps, call these tools, produce this artifact. This one doesn't. It's the opposite.

I built this out of the things I personally learned on the way to becoming a more autonomous, higher-level builder with Claude Code — and tried to write it the way I'd explain it to another person. What it turned into is a **playbook for how to think**, not a predetermined flow.

It's less "here's the recipe" and more "here's the mindset." The difference matters because the hard part of delegating real work through agents isn't picking the right tool — it's knowing when to stay above the work, when to verify without bias, when to build a team vs spawn subagents, when your own certainty is the thing to distrust. Those are judgment calls, and judgment calls are taught by internalizing principles, not by following steps.

## What's in it

The skill covers, in rough order:

- **The first two turns** — classifying the task, hedging from the start, presenting the process as a checkpoint before burning agent-hours.
- **Staying at the right level** — why dropping into implementation details costs you the architectural view.
- **The process is the product** — the goal will be met either way; quality lives in how you got there.
- **Unbiased verification** — defining "correct" yourself and asking verifiers for objective data, not judgments.
- **The hedge as an action trigger** — treating "presumably" as a flag in your own reasoning, not a tone choice.
- **Grounding, designing, creating the team, writing prompts, operating teams, recovering when things go wrong.**
- **Anti-patterns table** — the specific failure modes that show up again and again.

## Install

Clone into your Claude Code skills directory:

```bash
git clone https://github.com/x1klim/c-level-playbook.git ~/.claude/skills/c-level-playbook
```

Claude Code will pick it up automatically. Trigger it by asking Claude to take on something architectural, delegated, or large enough that executing it directly would mean losing the aerial view — or invoke it explicitly via `/c-level-playbook`.

The skill triggers itself on tasks like:

- Designing how a system should work (not just editing a file).
- Delegating work across multiple agents.
- Tasks where the user has handed over validation responsibility ("figure it out," "you decide," "I can't validate this").

It intentionally does **not** trigger on focused edits, direct questions, or small fixes — using it there is overkill.

## License

MIT
