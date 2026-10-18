# Visual design proposals

**Status: PROPOSAL. You evaluate every choice. None of this is a validated brand or a user requirement.**

These suggestions are for a later Figma file. They are not Phase 1 research. Changing them after you know your accessibility persona is expected.

Working name for the direction: **Street level**. The aim is a travel interface that stays readable outdoors, in one hand, with enough quiet structure for landmarks and routes. It is not a marketing landing page.

## Principles to test, not claims

| Proposal | Why it is on the table | How you should judge it |
|---|---|---|
| Warm paper surfaces rather than pure white | Pure white can glare in daylight. This is a lighting hypothesis. | Look at a phone outdoors before you commit |
| Deep green for primary actions | Associates with “go” and parks without using a default blue app chrome | Check contrast, and check that green is not the only “success” signal |
| Amber reserved for wayfinding emphasis | Direction needs to be seen at a glance | Use it on large elements. Do not use amber for small text until contrast passes |
| Short type, large targets | The person may be walking | Time a few taps while standing and walking slowly |
| A separate glasses overlay | A phone layout scaled down will not read as glasses | Sketch the overlay before styling the phone |

## Colour

Measure every pair you intend to ship with a contrast checker before calling it accessible. Ratios below are **not** pre-certified.

| Token | Hex | Intended use |
|---|---|---|
| `ink` | `#1C241F` | Primary text on light surfaces |
| `paper` | `#F6F3EC` | App background |
| `card` | `#FFFDF8` | Raised cards |
| `line` | `#DDD6C8` | Hairline borders |
| `canopy` | `#0E6B52` | Primary buttons and key selected states |
| `canopy-ink` | `#F6F3EC` | Text and icons on `canopy` |
| `moss` | `#E5F2EC` | Selected row or success surface |
| `waymark` | `#A35D00` | Large wayfinding marks only |
| `clay` | `#8E342C` | Errors and destructive actions |
| `slate` | `#3C4741` | Secondary text |
| `glasses-bg` | `#101410` | Scrim behind glasses content, if the design uses a dark overlay |
| `glasses-fg` | `#F4F1E8` | Glasses text and glyphs on that scrim |

`slate` on `paper`, and `waymark` on `paper`, are the pairs most likely to fail for small text. Check them first. Do not use colour alone to show selected, error, or premium state.

## Typography

Font choices are proposals. Confirm the licence inside Figma before you depend on one.

| Role | Proposed family | Compare against | Notes |
|---|---|---|---|
| UI text | Source Sans 3 | Atkinson Hyperlegible | Humanist sans, large x-height. Atkinson Hyperlegible is the comparison if your accessibility evidence points to low vision. It may be wrong for a different impairment. |
| Place names | Fraunces | None, or keep Source Sans 3 | Use for a landmark title only. UI controls stay in the sans. |
| Glasses | Source Sans 3, semibold | A single weight if the hardware is crude | Fewer sizes than the phone |

Proposed phone scale:

| Style | Size / line-height | Use |
|---|---|---|
| Place title | 28 / 34 | Landmark name |
| Screen title | 22 / 28 | Page title |
| Section | 18 / 24 | Group headings |
| Body | 16 / 24 | Instructions and descriptions |
| Meta | 13 / 18 | Distance, time, secondary facts |

Body text at 16px is the proposal for walking use. Do not go below 16px for instructions. Meta at 13px is optional and only where contrast is strong and the fact is repeated elsewhere.

## Spacing, shape, and targets

Base unit: 4px.

| Token | Value |
|---|---|
| `space-1` | 4 |
| `space-2` | 8 |
| `space-3` | 12 |
| `space-4` | 16 |
| `space-5` | 24 |
| `space-6` | 32 |
| `space-7` | 48 |

| Element | Proposal |
|---|---|
| Screen horizontal margin | 16px |
| Card padding | 16px |
| Gap between cards | 12px |
| Corner radius, cards | 12px |
| Corner radius, buttons | 12px |
| Primary control height | 48px |
| Minimum tap target | 48 × 48px |

WCAG 2.2 success criterion 2.5.8 (Target Size Minimum, AA) is a 24 × 24 CSS pixel floor with exceptions. A 48px target is a **stricter project proposal** because the context is walking. It is not a research result. Read the criterion before you cite it: https://www.w3.org/TR/WCAG22/

## Layout frames

| Frame | Width × height | Role |
|---|---|---|
| Primary | 390 × 844 | Interactive phone prototype |
| Compact | 360 × 800 | Check navigation and long place names |
| Glasses | Define and document | Short and wide enough for one instruction. Do not reuse 390 × 844 |

Respect the status-bar and home-indicator regions on the phone frames. Bottom navigation sits above the home indicator.

## Component patterns

Use placeholder labels such as `[Landmark name]` until content comes from a real place you decide to feature. Do not invent reviews or star ratings.

| Component | Anatomy | States to design later |
|---|---|---|
| Top bar | City or area, search, account | Default, search active |
| Landmark card | Image, name, distance, walking time if known, save | Default, saved |
| List / map switch | Two options, current one indicated by more than colour | List, map |
| Place detail | Name, facts, short description, add to walk | Loading, missing photo |
| Stop list | Order, name, remove, reorder | One stop, many stops, empty |
| Primary button | Verb, full width on forms | Default, pressed, disabled |
| Secondary button | Quieter action | Default |
| Text field | Label above the field, hint, error text | Empty, focus, error |
| Premium lock | What is locked, why, link to membership | Locked, owned |
| Checkout steps | Plan, payment details mock-up, confirm | Editing, error, success |
| Glasses overlay | One glyph, distance, one line of instruction, voice state | Idle, speaking, listening, unavailable |

Empty states need a next action: no saved places, no route yet, location unavailable, membership not active. Write that copy yourself later. It is part of the design, not part of this proposal.

## Smart-glasses overlay

**PROPOSAL.**

- One instruction on screen. A second line only for distance or a street name.
- A single direction glyph.
- Voice state is visible: idle, listening, speaking, or unavailable.
- High contrast light-on-dark scrim, until you know the display technology. Transparent waveguide displays do not behave like a phone. If you later pick a real device, replace this scrim with that device’s constraints and cite the specification.
- The phone remains the place for search, long lists, payment, and account detail.
- Provide a way to repeat the instruction and a way to stop guidance.
- Do not put paragraphs, cards, or a bottom tab bar on the glasses.

These overlay rules are interaction hypotheses. Published wearable studies, if you find them, should override the ones they contradict. Log those studies before you treat them as requirements.

## Accessibility checks before hi-fi sign-off

Complete this list after the accessibility persona exists. Until then, leave the MoSCoW column blank.

| Check | Question | MoSCoW | Evidence |
|---|---|---|---|
| Contrast | Do text and icons meet the WCAG level you are targeting? | | |
| Non-colour cues | Can someone see state without hue? | | |
| Text size | Can body text scale, or is an in-app size offered? | | |
| Targets | Are walking-context controls at least your chosen minimum? | | |
| Names | Do icon-only controls have visible text or an accessible name in the prototype notes? | | |
| Motion | Is anything moving that should have a reduced-motion alternative? | | |
| Voice | If speech is essential to glasses, what happens if the street is loud or the person cannot use voice? | | |
| Persona fit | Which checks exist because of the impairment in your evidence, not because they were on a generic list? | | |

## Heuristics to apply in Phase 2

When you design screens, judge them yourself against Nielsen’s ten usability heuristics. Confirm the current wording and cite the Nielsen Norman Group article only after you open it:

https://www.nngroup.com/articles/ten-usability-heuristics/

The Week 9 review expects you to explain how heuristics and UX principles informed decisions. That explanation is assessed speaking and writing. Draft it after the screens exist, from your choices.

## What this file must not become

A style sheet does not demonstrate user research. Do not paste these tokens into the Week 5 checklist as market findings.
