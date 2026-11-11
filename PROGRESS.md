# Progress — שדה תעופה (airport)

Claude keeps this file up to date. Every session starts by reading it and ends
by updating it, so work can stop and resume at any point.

**Now:** Phase 1 done (skeleton of 19 screens, `qa_check.py` contract OK) · waiting for the developer to confirm the screen map; Phase 2 (design reference) is next
**Waiting on you:** read `PROJECT_BRIEF.md` (the screen table) and say "the map is fine" or what to change; send `open-questions.md` to the content team (Claude can draft the message)
**Waiting on others:** content team — the 24 questions in `open-questions.md` (not sent yet)

## Inputs
All in `STEM/שדה תעופה/` (inputs stay there; never copied into the project):
- Storyboard: `שדה תעופה_אחרי עריכה לשונית וצמצום סרטונים.pptx` — 42 slides, language-edited, videos reduced
- PSD: `airport_stem.psd` — 1920×1080, 10 frames, **question screens only** (Q1, Q2, Q3, Q4א, Q4ב, Q5, Q6א, Q6ב, Q7, Q8)
- Comps: `airport_03.11.26.pptx` — 12 pictures of the design
- Applets: `applets/ספטמבר-אוקטובר.html`, `applets/נובמבר-דצמבר.html` (single-file "bundled" pages, 178 KB each; not looked inside yet)
- Project folder: `STEM/שדה תעופה/הפקה/airport/` · preview: `airport` on port 8135 (entry added to the launch.json of `פיתוח STEM`)

## Phases
- [x] 0 · Setup — inputs found, tools installed, project folder created (2026-11-11)
- [x] 1 · Storyboard read — screen map (screens.json, PROJECT_BRIEF.md), production-notes.md, open-questions.md; index.html is a 19-screen skeleton (2026-11-11)
- [ ] 1 · ✋ Developer reviewed the screen map; open questions sent (date: )
- [ ] 2 · Design reference — PSD inventory (done), frames mapped to screens (guessed in screens.json, to verify), mockups for the overlay
- [ ] 3 · ASSET_CHECKLIST.md written
- [ ] 3 · ✋ Assets exported and checked (check_assets.py clean)
- [ ] 4 · Screens built (tick per batch below)
- [ ] 5 · Applets built and signed off; videos and audio in
- [ ] 6 · Self-QA passed (qa_check.py 0 errors, walk-through done)
- [ ] 7 · Translation export done (both sweeps pass), ASSET_LOCALIZATION.md written
- [ ] 8 · ✋ Delivered: repo pushed (published to the org the first time), SharePoint shortcut and snapshot updated, links sent

## Screens
| # | sid | built | matches design | approved by developer |
|---|---|---|---|---|
| 1 | video-intro | skeleton | ☐ | ☐ |
| 2 | story-office | skeleton | ☐ | ☐ |
| 3 | q1 | skeleton | ☐ | ☐ |
| 4 | video-estimate | skeleton | ☐ | ☐ |
| 5 | q2 | skeleton | ☐ | ☐ |
| 6 | story-data | skeleton | ☐ | ☐ |
| 7 | q3 | skeleton | ☐ | ☐ |
| 8 | q4a | skeleton | ☐ | ☐ |
| 9 | q4b | skeleton | ☐ | ☐ |
| 10 | story-holiday | skeleton | ☐ | ☐ |
| 11 | q5 | skeleton | ☐ | ☐ |
| 12 | story-team | skeleton | ☐ | ☐ |
| 13 | video-chart | skeleton | ☐ | ☐ |
| 14 | q6a | skeleton | ☐ | ☐ |
| 15 | q6b | skeleton | ☐ | ☐ |
| 16 | story-daily | skeleton | ☐ | ☐ |
| 17 | q7 | skeleton | ☐ | ☐ |
| 18 | q8 | skeleton | ☐ | ☐ |
| 19 | finish | skeleton | ☐ | ☐ |

## Decisions
- 2026-11-11 · Version check storyboard ↔ design: same 8 questions, same numbering (1, 2, 3, 4א/ב, 5, 6א/ב, 7, 8 = the 10 PSD frames). Stems differ only in small wording (e.g. Q1: design "הקשיבו להקראה ובחרו את הסרטון שבו הוא הקריא נכון", storyboard "הקשיבו להקראות ובחרו את ההקראה שבה מתן קרא נכון"). The storyboard is the language-edited one, so learner text comes from it and looks from the PSD. Build goes ahead. · Claude
- 2026-11-11 · Screen map: 19 screens (4 videos, 5 narration screens, 10 question screens, finish). Slide 1 is the cover and not a screen. No opening screen: the first screen is the video. Slides 40–42 are one finish screen (video, then "סיימתי", then the house score pop-up). · Claude, awaiting the developer
- 2026-11-11 · Scoring built from slide 42: equal weight per question → 12.5 each; parts of Q4 and Q6 6.25 each (sums to 100). Slide 42 is the only scoring source. · Claude
- 2026-11-11 · Button label is the storyboard's "צדקתי?" (not the house "האם צדקתי?"); final-wrong title is the storyboard's "זו טעות"; partial title "נכון חלקית" is new wording (open question 3). · Claude
- 2026-11-11 · The 9 screens without a PSD frame: the script had 7 videos, cut to 4 for budget, so 5 former video scenes (screens 2, 6, 10, 12, 16) are now a still picture with narration. Developer's decision: reuse the repeating base pictures and generate slightly altered versions where needed (screens 6 and 16, optionally 12; 2 and 10 stay as they are). Brief with prompts: `SCENE_IMAGES_BRIEF.md`. The "small animation" notes are treated as dropped (open question 11). · developer
- 2026-11-11 · Engine change: typed answers accept `data-maxlen` (default 4 digits). Q8's answer 100000 has 6 digits, so its box has `data-maxlen="6"`. · Claude
- 2026-11-11 · q3, q4a, q4b are left without `data-dnd-final="compare"` (qa_check warns): the storyboard says to show the correct answer on those screens (slide 19 note, slides 21 and 23 show the solved line), and they are one line of slots, not labelled rows. q2 and q5 have `compare`. To re-decide in Phase 4 if the walk-through looks wrong.

## Open items
- 24 questions to the content team (`open-questions.md`), not sent yet. The ones that change the build: Q1 audio or video and the missing help hint (12, 13); the partial result and its wording (3); the narration button (10); the scoring/"בוצע בהצלחה" report (1).
- Storyboard slide 40 says "שקף 50-51" and slide 28 "שקפים 35-37" (stale; built as slides 40–41 and 28–30).
- The PSD has frames for the 10 question screens only (the video scenes were cut from 7 to 4). The 4 video screens, the finish and the 5 picture screens use the storyboard's pictures; screens 6 and 16 (and maybe 12) need a generated variant (`SCENE_IMAGES_BRIEF.md`) — waiting on the developer.
- Q6א/Q6ב are **scored applet questions**: the engine has no `kind="applet"` yet. They need a custom piece: the applet posts the drawn height, a `HOOKS` entry grades it, the screen's check button and feedback do the rest. Plan in Phase 5, after looking inside the two applet files.
- Caption times in the 4 videos are even placeholders until the videos and their SRTs arrive. No videos, audio, narration or animations exist yet (question 10 decides the narration button; the small animations are replaced by stills).
- Slide-to-PSD-frame mapping in screens.json (`psd`) is by question number, to be checked in Phase 2.

## Delivery log
<!-- date · git commit · repo link · SharePoint link · what changed since the last one -->
