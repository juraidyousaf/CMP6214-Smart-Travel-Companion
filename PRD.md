# Product requirements document

**Status: preliminary. Not a validated specification.**

Smart Travel Companion is a proposed mobile application for the CMP6214 theme **Interaction on the Move**. The audience under consideration is city tourists exploring landmarks and attractions on foot.

The audience, problems, and features below are **HYPOTHESIS** until each one is tied to a source ID in `research/source-register.md` and written up in your own words. The assessment brief does fix some submission scenarios. Those are coursework requirements. They are not user-research findings.

## Concept

| | |
|---|---|
| Working title | Smart Travel Companion |
| Theme | Interaction on the Move (travelling and tourism; outdoor sightseeing; pedestrian navigation) |
| Product form | Mobile application mock-up, plus a designed smart-glasses interface |
| Context of use | On foot, in an unfamiliar city, often outdoors |
| Validation state | Unvalidated |

## Target audience

**Coursework audience, confirmed as the group under study.** City tourists exploring landmarks and attractions on foot.

Age, trip length, tech confidence, group size, and language are still unknown. One persona must include an impairment or disability and mobile accessibility considerations. The opened evidence most relevant to that choice is S007, on people who are blind, have low vision, or are deafblind. Choosing that impairment, or a different one, is your decision after you read the source. See `research/RESEARCH_LIMITATIONS.md` and `research/secondary-research-synthesis.md`.

## Research questions

Secondary research is the current method, on your confirmation of 18 October 2026. A lecturer document is not yet filed.

| ID | Question | Status |
|---|---|---|
| RQ1 | How do tourists discover landmarks and attractions in unfamiliar cities? | Open. No source opened on 18 October 2026 answers this directly |
| RQ2 | What difficulties are documented for pedestrian navigation? | Working evidence in S004, S005, S006, and abstract-only S014 |
| RQ3 | What limitations of travel-planning applications are documented? | Partial. Official help for Google Maps and Wanderlog. Tripadvisor not opened. No sessions yet |
| RQ4 | What accessibility considerations affect travellers with disabilities? | Working evidence in S007, S006, S008, and S009. Not a persona |
| RQ5 | What uses and limits of smart glasses and hands-free navigation are documented? | Working evidence in S004 and S005. Not a validated premium requirement |
| RQ6 | Which improvements follow from the evidence? | Candidate opportunities only. See the synthesis |

## Proposed user flows

These flows are still hypotheses plus the scenarios the brief requires. Research has not validated them.

| Flow | Hypothesis or brief requirement | What research currently touches |
|---|---|---|
| A. Discover landmarks | Hypothesis F1, and the brief’s free-content path | RQ1 is unanswered. S006 discusses landmarks as navigation cues, not as a discovery catalogue |
| B. Plan a walking route | Hypothesis F2 | S011 shows a planner can display walking time between stops. S010 shows Maps can start walking navigation. Neither is your observation |
| C. Register and log in | Brief requirement | Not studied in the opened sources |
| D. Premium purchase and checkout | Brief requirement. One journey must include it | No opened source about willingness to pay |
| E. Smart-glasses assistance | Hypothesis F3, and the brief’s premium multimodal feature | S004 and S005. Mixed outdoor evidence. Not proof of demand |

## Problem hypotheses

These are starting points for research questions. They are not findings.

| ID | Hypothesis | What would count as evidence | Status |
|---|---|---|---|
| H1 | A tourist on foot in an unfamiliar city can find it difficult to discover landmarks that fit the time they have and where they are standing. | Published research, documented user feedback, or your own observation notes, with citations | HYPOTHESIS |
| H2 | Organising several sights into a walkable sequence may require more than one product, or more steps than the person can manage while moving. | Same as H1, plus competitor observation | HYPOTHESIS |
| H3 | Holding and looking at a phone while walking may conflict with the street environment. A hands-free glasses mode might reduce that conflict for some people. | Research on pedestrian navigation and wearable displays, if you find and read it. Direct product observation where a hands-free mode exists | HYPOTHESIS |
| H4 | Some tourists need accessibility adjustments while walking and sightseeing. The impairment and the interaction needs are not yet chosen. | S007, S006, S008, and S009 are opened starting points. The persona is still yours to write | HYPOTHESIS |

Do not promote a hypothesis to a problem statement in the checklist until the evidence column is filled.

## Feature hypotheses

The brief requires at least three main features informed by your three personas, including one premium smart-glasses feature, plus accounts and a premium payment path. The specific tourist features below are still hypotheses.

| ID | Feature | Tier | Brief link | Status |
|---|---|---|---|---|
| F1 | Discover city landmarks, attractions, and sightseeing locations | Free | Browse free content | HYPOTHESIS |
| F2 | Plan walking routes and organise sightseeing destinations | Free | Second free user flow | HYPOTHESIS |
| F3 | Smart-glasses travel assistance: visual direction overlays, voice guidance, and hands-free interaction | Premium | Multimodal smart-glasses feature | HYPOTHESIS |

F1–F3 must not be written up as user requirements until research supports them. If research points elsewhere, change the features. The brief still expects two free flows, one premium glasses flow, account access, and a membership checkout in the prototype.

### Coursework scenarios the prototype must be able to show

These come from the assessment brief (Theil, 2026), not from users:

1. Browse free content or features.
2. Register or log in.
3. Find a sign-up path for a premium membership.
4. Confirm an order.
5. Complete a payment checkout mock-up.
6. Reach content that is available only after membership.
7. Show the smart-glasses interface.

No real payment provider and no real glasses hardware are required.

## Design boundaries

- Figma (or a similar prototyping tool) for the interactive mock-up. No frontend or backend code is required for this assignment.
- Checkout demonstrates the interaction. It does not take money.
- The glasses UI demonstrates display, speech, and hands-free interaction. It does not integrate with a device SDK.
- Resources inside the app may be articles, video, or audio if your research shows they matter. None are specified yet.
- Account management in the brief includes profile and payment-detail management. Include those flows in later prototyping once the information architecture is agreed from your research.

## Out of scope unless your evidence adds them

Group planning, restaurant booking, live transit, hotel search, and social feeds are not part of the current hypothesis set. Add one only if a source you have logged supports it and the prototype remains demonstrable in Week 9.

## Pending research validation

| Decision | Owner | Blocker |
|---|---|---|
| Whether secondary research can stand in for interviews in Week 5 | You confirmed this on 18 October 2026 | User-reported. No lecturer document filed |
| How the accessibility persona is evidenced | You, after reading S007 and any further sources | Method is secondary research. The persona is not written |
| Which published sources actually support H1–H4 | You must re-read the register | Sources are logged. None are marked verified by you |
| Which competing products you observed, and what you saw | You | No observation sessions logged |
| Final Must / Should / Could / Won't list | You | Depends on personas and journeys |
| Visual design decisions in `DESIGN.md` | You | Proposals only |

## Relationship to other files

- Evidence rules: `RULES.md`
- Secondary-research method: `research/ALTERNATIVE_RESEARCH_PLAN.md`
- Working synthesis, not a submission: `research/secondary-research-synthesis.md`
- Blank write-up structure: `docs/phase-1/10-final-submission/week-5-checklist-outline.md`
