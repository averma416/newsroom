# Newsroom

A multi-agent skill for Claude that researches guests, fact-checks every premise, and builds moderator or interview questions. Built for panels, interviews and podcasts where every question has to be accurate and respect what each guest agreed to.

## What it does

Newsroom runs as a team. A lead agent handles intake and delivery. Separate agents do the research, drafting, fact-checking and editing, so no work checks itself.

| Desk | Job |
|---|---|
| Lead | Intake, brief, merge, final delivery |
| Research Desk | One agent per guest. Verified public record: roles, published work, talks, quotes, company context |
| Topic Desk | Recent incidents, statistics and frameworks on the session topic |
| Question Desk | Drafts the arc and questions from verified material only |
| Fact Desk | Fresh agent. Re-checks every factual premise in every question |
| Editor | Fresh agent. Checks tone, guest boundaries, structure and audience fit |

## How it works

1. **Intake.** Event, audience and technical depth, guests, what each guest wants to cover, what each guest won't discuss, your voice and limits, and the one idea the session should leave behind.
2. **Research.** Primary sources and credible press only. Data brokers, people-search sites, SEO farms, AI-generated pages and aggregators are banned. Estimates are kept separate from confirmed facts.
3. **Questions.** Each one names a specific mechanism, opens with a plain setup line, asks one thing, and comes with one follow-up. Guest boundaries are hard rules.
4. **Fact check.** Every premise is re-opened against its source. Unsupported words like "most," "all" and "never" get flagged.
5. **Edit.** Boundaries, tone, filler, sensational phrasing, and coverage of each guest's asks.
6. **Deliver.** The arc with timings, questions by act marked core or reserve, a fact sheet with sources, a boundary check, and open items to confirm with guests.

Every desk runs as its own agent on every run, including revisions. The lead never drafts or checks its own work. Existing research or drafts go to the right desk as input, not around it. The Fact Desk marks anything it did not re-open this run as Unconfirmed. If subagents aren't available, Newsroom says so and asks before running single-agent.

Edits to a single question re-run a fresh Fact Desk and Editor on that question.

## Install

Copy `SKILL.md` into your Claude skills folder, or upload it as a skill in Claude. Then ask Claude to run newsroom, or describe a panel or interview you're preparing.

## License

MIT. See [LICENSE](LICENSE).
