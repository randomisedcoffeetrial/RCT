# Randomised Coffee Trial (RCT)

A prototype for a platform that matches researchers – any field, any level, honours upward – with one other researcher nearby, once a week, for an in-person coffee. Social connection first, transdisciplinary thinking as the bonus.

**This is a demo, not a product.** Everything is simulated: the people are fictional, ORCID verification is mocked, matching runs locally in your browser, and nothing is sent or stored on a server.

## Running it

Open `index.html` in a modern browser (Chrome, Edge or Safari). No build step, no server, no dependencies – it works offline by double-click. All state lives in your browser's localStorage.

## How it works

- **Double-blind weekly matching.** Each week you privately pick topics you'd love to learn about, drawn from what researchers near you can talk about. Nobody sees anyone's profile or picks until a match is made at the Monday drop.
- **Mutual matches first.** When two people are each curious about the other's field, they're matched as a priority. Near-equivalent topics count (the similarity layer knows "chronic pain" and "low back pain" are neighbours). Otherwise you get an honestly-framed wildcard.
- **No hierarchy.** No titles, no career stages, no institutions required. A first-year honours student and a professor look the same.
- **In person, minimal online.** A small logistics chat exists only to plan the coffee: proposed times carry a venue and duration, accepted as a package, with a countdown to the meet-up.
- **Accountability.** Meetups are logged, followed by optional notes (shareable with your match) and an optional survey that feeds an aggregate-only impact dashboard and an anonymised "Sparks" wall.
- **Never re-matched.** Pairs can exchange contact details, revealed only if both opt in.

## Exploring the demo

Use the **Control Centre** (floating button, bottom right) to:

- switch between 36 seeded fictional personas and play both sides of a match
- run the weekly matching and advance weeks
- time-travel past an organised meet-up to reach the log and survey flow
- toggle Mobile (iOS-style frame) / Desktop layouts and light/dark theme
- open the "how was this decided?" explainer (demo/admin only) and reset the demo

The seed data is engineered so every matching scenario is demonstrable: perfect mutuals, similarity-based mutuals, one-way and open wildcards, carry-over priority for the unmatched, paused users, blocked pairs, availability clashes and never-re-match history.

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire prototype: HTML, CSS and vanilla JS in one file |
| `HANDOVER.md` | The original build brief and decisions |
| `NOTES.md` | Running build log and implementation notes |

## Status

Prototype under active iteration. The real version is planned for Firebase with genuine ORCID OAuth, server-side matching (maximum-weight matching), embedding-based topic similarity and notifications – see section 17 of `HANDOVER.md`.
