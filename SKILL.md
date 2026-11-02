---
name: "newsroom"
description: "Multi-agent team that researches, fact-checks and builds moderator or interview questions grounded in verified facts, guest asks and boundaries. Use for panels, interviews and podcasts."
---

# Newsroom

A team that turns research, guest input and the user's limits into a question set where every premise is verified and every question respects what each guest agreed to.

The lead (you) runs intake, dispatches agents with the Agent tool, merges results and delivers. Research agents run in parallel in the background. The Fact Desk and the Editor run fresh, after drafting, so the work is never checking itself.

## Team

| Desk | Job |
|---|---|
| Lead | Intake, briefs, merge, final delivery |
| Research Desk (1 agent per guest) | Guest's verified public record: roles, published work, talks, quotes, company context |
| Topic Desk | Recent incidents, data and frameworks on the session topic |
| Question Desk | Drafts the arc and questions from verified material only |
| Fact Desk (fresh) | Checks every factual premise inside every question |
| Editor (fresh) | Checks tone, boundaries, structure, audience fit |

## Phase 1: Intake (Lead)

Collect, asking with AskUserQuestion only for what is missing from the conversation or attached files:

1. **Event:** name, date, length, format (panel, 1:1, podcast).
2. **Audience:** who they are and how technical. Target depth on a 1 to 10 scale.
3. **Guests:** names, titles as confirmed by the guest, profiles or bios provided.
4. **Guest asks:** topics each guest wants to cover, quoted from their emails or notes.
5. **Guest boundaries:** what each guest will not discuss, quoted exactly. These are hard rules.
6. **User's limits and voice:** tone, banned phrasing, style preferences, the user's own background and what they can credibly ask.
7. **Thesis:** the one idea the session should leave behind. If none yet, the Question Desk proposes two options.

Write a **Brief** with all seven. Every agent gets it.

## Phase 2: Research (parallel)

If briefs on the guests already exist in the conversation or the user's artifacts, reuse them and research only gaps.

**Research Desk, one per guest.** Find the guest's own verified public voice and record: roles, published content, talks, quotes, company filings and releases. Prioritize material tied to the guest's stated asks.

**Topic Desk.** Find recent, citable material on the session topic: named incidents, survey statistics, regulation, frameworks. For each statistic record the exact figure, sample, date and publisher.

**Shared rules for both desks:**
- Tiers: T1 primary (company sites, filings, official releases, the guest's own content, government and standards bodies). T2 credible press with editorial standards. T3 banned: data brokers, people-search sites, SEO farms, AI-generated pages, aggregators, vendor blogs restating others' reporting.
- Vendor research and whitepapers may be used for ideas, never as the sole source for a statistic.
- Separate an incident's verified facts from estimates. "Potentially impacted" is not "breached."
- No inference. If the page does not say it, it is not a fact.
- Never collect personal information about guests beyond their professional public record.
- Return one row per claim: claim | URL | tier | date | exact excerpt under 15 words.

## Phase 3: Question Desk

Given the Brief and verified rows only, draft:

1. **Arc:** an opening, 3 to 5 acts, Q&A and a close. Each act answers one question that moves the thesis forward and ends with a one-line transition into the next.
2. **Questions:** for each, a lead guest, the question, one follow-up, and the source row(s) behind any factual premise.

Question standards:
- **Anchored:** tied to the guest's verified work or stated asks. No questions that only work if an unverified claim is true.
- **Mechanism over feeling:** name the specific control, process, system or failure. Not "what surprises you" but "which of these channels carries the most risk, and why."
- **Setup plus ask:** one plain sentence the whole audience can follow, then the question an expert answers.
- **One question per turn.** A second part becomes the follow-up.
- **Respect boundaries:** a guest who keeps their employer out of it gets industry-level framing ("what does good look like," "where do companies fail"), never "what do you do."
- **No leading assumptions:** don't build a claim into the question that the guest should be the one to state, such as "companies are keeping up, right?"
- **Balance:** every guest leads at least two questions. Note the count.
- **Reserve list:** mark which questions are core and which are reserve for the time slot. Assume about 3 to 4 minutes per question including follow-up.

## Phase 4: Fact Desk (fresh agent)

Give it the draft questions and the research rows. It does not see how they were written.

For every factual statement inside a question, setup line, opening or closing:
- Re-open the source and confirm the page supports the wording as written.
- Flag quantifiers the sources do not support: most, all, every, majority, always, never.
- Flag figures that need softening ("potentially" vs "confirmed").
- Flag anything from the model's own memory with no source this session.

Verdict per premise: **Verified**, **Rewrite** (with the supported wording), or **Cut**. The Lead applies every change.

## Phase 5: Editor (fresh agent)

Give it the Brief and the fact-checked draft. It checks:

- **Boundaries:** any question that breaks a guest's stated limit. Zero tolerance.
- **Guest asks:** each guest's stated topics appear at least once.
- **Tone:** professional and neutral. Cut sensational or loaded phrasing ("rubber stamp," "nightmare," "no matter how good it gets," "struggled for years"). Cut questions that set a guest up to defend their product.
- **Voice:** apply the user's style rules. Remove filler and AI tells: actually, genuinely, really, truly, crucial, delve, landscape, em dashes, "not just X, it's Y." Short declarative sentences.
- **Depth:** matches the target on the 1 to 10 scale. Technical terms get a plain setup line.
- **Structure:** one ask per question, arc flows, timing fits.

Returns a marked-up list of changes. The Lead applies them.

## Phase 6: Deliver (Lead)

Deliver in the conversation, or as a Docs artifact if the user wants something to keep or share:

1. The arc with timings and transition lines.
2. Questions by act: lead guest, question, follow-up. Core and reserve marked.
3. **Fact sheet:** every factual premise used, with source and tier, and how to say it on stage.
4. **Boundary check:** each guest, their stated limits, and confirmation that no question crosses them.
5. **Open items:** anything to confirm with a guest before the event (titles, quoting their emails back to them on stage, sensitive topics).

Keep it short. No recap of the process.

## Revisions

When the user edits a question, run only the Fact Desk and Editor on the changed question. When new guest input arrives, update the Brief first, then re-run the Question Desk on affected acts.

## Guest-facing versions

When the user wants to send questions to guests: drop follow-ups, drop fact-sheet sources, keep the arc and one question per item, and add a line inviting changes. Never quote a guest's private email back to the group without the user confirming.