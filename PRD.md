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

**HYPOTHESIS / coursework choice.** City tourists exploring landmarks and attractions on foot.

This sentence names who the project intends to study. It does not describe a researched segment. Age, trip length, tech confidence, group size, language, and disability are unknown until you collect evidence. One of the three personas must include an impairment or disability and mobile accessibility considerations. Which impairment, and which needs follow from it, must come from sources you examine. See `research/RESEARCH_LIMITATIONS.md`.

## Problem hypotheses

These are starting points for research questions. They are not findings.

| ID | Hypothesis | What would count as evidence | Status |
|---|---|---|---|
| H1 | A tourist on foot in an unfamiliar city can find it difficult to discover landmarks that fit the time they have and where they are standing. | Published research, documented user feedback, or your own observation notes, with citations | HYPOTHESIS |
| H2 | Organising several sights into a walkable sequence may require more than one product, or more steps than the person can manage while moving. | Same as H1, plus competitor observation | HYPOTHESIS |
| H3 | Holding and looking at a phone while walking may conflict with the street environment. A hands-free glasses mode might reduce that conflict for some people. | Research on pedestrian navigation and wearable displays, if you find and read it. Direct product observation where a hands-free mode exists | HYPOTHESIS |
| H4 | Some tourists need accessibility adjustments while walking and sightseeing. The impairment and the interaction needs are not yet known. | Published accessibility research and documented accounts you read. Not an invented persona | BLOCKED |

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
| Whether secondary research can stand in for interviews in Week 5 | You, after lecturer reply | Email not sent |
| How the accessibility persona is evidenced | You, after lecturer reply | No interviews; method not approved |
| Which published sources actually support H1–H4 | You | No student reading logged |
| Which competing products you observed, and what you saw | You | No observation sessions logged |
| Final Must / Should / Could / Won't list | You | Depends on personas and journeys |
| Visual design decisions in `DESIGN.md` | You | Proposals only |

## Relationship to other files

- Evidence rules: `RULES.md`
- What you will do instead of interviews, pending approval: `research/ALTERNATIVE_RESEARCH_PLAN.md`
- Blank write-up structure: `docs/phase-1/10-final-submission/week-5-checklist-outline.md`
