# Progress — שדה תעופה (airport)

Claude keeps this file up to date. Every session starts by reading it and ends
by updating it, so work can stop and resume at any point.

**Now:** Phase 4 · screens 1–10 built (batches A and B) and waiting for the developer's approval by screenshot; next batch C (screens 11–15: q5, story, video, the two graph applets)
**Waiting on you:** look at the screenshots of screens 1–10 and say "fine" or what to change; confirm the screen map (open since Phase 1)
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
- [x] 2 · Design reference — PSD inventory, frames mapped to screens (checked against the text layers), mockups for the overlay (12 files in `_design-reference/mockups/`), colour tokens set (2026-11-11)
- [x] 3 · ASSET_CHECKLIST.md written (2026-11-11; all 19 rows resolve in a dry run)
- [x] 3 · ✋ Assets exported and checked (check_assets.py: 23 files, 0 errors, 0 warnings); developer approved the contact sheet of batch 1 (2026-11-11); batch 2 (flags, airplane, suitcase) looked right on the sheet
- [ ] 4 · Screens built (tick per batch below) — batch A, screens 1–5, and batch B, screens 6–10, built 2026-11-11
- [ ] 5 · Applets built and signed off; videos and audio in
- [ ] 6 · Self-QA passed (qa_check.py 0 errors, walk-through done)
- [ ] 7 · Translation export done (both sweeps pass), ASSET_LOCALIZATION.md written
- [ ] 8 · ✋ Delivered: repo pushed (published to the org the first time), SharePoint shortcut and snapshot updated, links sent

## Screens
| # | sid | built | matches design | approved by developer |
|---|---|---|---|---|
| 1 | video-intro | ✔ | ✔ | ☐ |
| 2 | story-office | ✔ | ✔ | ☐ |
| 3 | q1 | ✔ | ✔ | ☐ |
| 4 | video-estimate | ✔ | ✔ | ☐ |
| 5 | q2 | ✔ | ✔ | ☐ |
| 6 | story-data | ✔ | ✔ | ☐ |
| 7 | q3 | ✔ | ✔ | ☐ |
| 8 | q4a | ✔ | ✔ | ☐ |
| 9 | q4b | ✔ | ✔ | ☐ |
| 10 | story-holiday | ✔ | ✔ | ☐ |
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

- 2026-11-11 · Design reference: PSD frames #2–#11 = Q1, Q2, Q3, Q4א, Q4ב, Q5, Q6א, Q6ב, Q7, Q8 (screens 3, 5, 7, 8, 9, 11, 14, 15, 17, 18). The comps deck has the same 10 plus two popup states (Q2 help bubble → mockup `screen-05-b`, Q4א info bubble → `screen-08-b`). Text in the PSD matches the storyboard except the known Q1 wording; the design adds a colon to "שאלה מס' N:" (the storyboard's text is used, no colon). Colours sampled from the comps into the tokens (panel white, black outline, pill blue #004CC4 / #B0CFFB, chip #B4BDCE, slot #E4EEFA, buttons #2B2B2B). · Claude
- 2026-11-11 · The design's white panel is almost the whole stage (1896×1056 at x 12, y 12, with the help button, arrows and "צדקתי?" inside it). The lomda uses the house panel (1800×798 at x 60, y 120), as the skill says, so the background picture stays visible and longer Arabic text has room. If the developer prefers the design's panel it is one CSS block. · Claude, to be told to the developer

- 2026-11-11 · The background of the 10 question screens is ONE picture, `bg-airport.jpg` (the same scene, already darkened by the designer, in every frame): exported once without the panel and buttons. So the starter's `.q-overlay` darkening must not be added on top of it. The 4 reading cards of Q1 are 4 near-identical pictures of Matan (small differences of expression). · Claude
- 2026-11-11 · Export fix: `[hide: …]` markers in the checklist take one layer name each (a `|` inside a markdown table breaks the list). Boxes of buttons in the checklist are the visible size; the inventory's larger box includes the shadow, which CSS draws (`filter: drop-shadow(0px 8px 12px rgba(0,0,0,0.38))`; bulb 0 5 4 .41). · Claude

- 2026-11-11 · Phase 4 layout decisions, batch A: the background is the shared `bg-airport.jpg` (no overlay); the nav arrows, help button, "צדקתי?" and chips use the PSD pictures; stepper pills restyled from the design (digits in dark blue on the light pills for contrast, not white as in the design). Q1: the four reading cards are 228 px wide on the right so the "try again" box fits on the free left; the long final feedback (four readings) covers the lower half of the cards, as the storyboard's own slide 11 does, and has a close X (`data-feedback-close`). (superseded by the large panel below: no overlaps on q1 any more). Q2: rows and chips are one grid; the final feedback sits over the locked chip bank. · Claude
- 2026-11-11 · Stand-in pictures from the storyboard (posters of videos 1, 2, 3 and the finish; backgrounds of the story screens) are in `assets/images/*-poster.jpg` and `*-bg.jpg`. `story-data-bg` and `story-daily-bg` are the BASE pictures until the altered versions (SCENE_IMAGES_BRIEF.md C, optional) exist; replace the files under the same names. · Claude

- 2026-11-11 · Developer's instruction: question screens (except question 1) follow the PSD; everything else (the video and picture screens, the finish and question 1) uses the generated pictures in `STEM/שדה תעופה/תמונות מגונרטות/` and the script. Mapping: video-intro poster = `ChatGPT Image Aug 17, 03_06_26 PM` (TV room); question background, video-estimate poster, story-data = `Aug 17, 04_50_12 PM`; story-office = `Sep 14, 03_53_03 PM`; story-team, story-daily, video-chart poster = `Jul 29, 10_32_34 AM`; finish poster = `Jul 29, 12_54_39 PM`; kitchen scene (`Jul 28`) is for the video; airplane = `Jul 29, 12_22_44 PM`; suitcase = `Jul 29, 12_35_31 PM`; question 1 = `Skyline Soundscapes Playlist Cards.png` (four cards cut out, audio bar painted in; city and number are live text in the white band). Not used: `Jul 29, 11_54_31 AM` (a 50-shekel note), `Sep 14, 03_14_24 PM` and `03_22_12 PM` (Matan reading; the PSD's old question 1). Holiday scene picture (slide 24) is not in the folder; the storyboard's own picture is used. · developer, applied by Claude
- 2026-11-11 · Narration bubbles use the park-drones style (translucent card flush to the top-right corner, 64 px corner at the bottom-left, same house text size), text from the script only. The five picture screens are animated in code like park-drones: a slow drift/zoom of the whole scene, a pulse of daylight over the windows, and soft pulses over screens and the tablet (opacity and transform only; reduced motion leaves the picture still). Screen 6 does not need a generated variant. · developer, applied by Claude

- 2026-11-11 · Developer's decision: the design's large white panel (1896×1056 at x 12, y 12, black outline) on ALL ten question screens, replacing the skill's smaller house panel. The help button, pills, arrows and "צדקתי?" sit inside it as in the PSD ("צדקתי?" at the design's height, bottom 88). The band under the content, between the two arrows, takes the feedback boxes. Question 1: cards 350 px wide, both feedback boxes in the band under them (layout_check clean on screens 3 and 5; the earlier expected final-state overlaps on q1 are gone). Question 1 uses only the script's skyline picture; the narration of the four readings (and of the feedback readings) is to be added later: the `.reader-media` hooks on each card are in place (audio pending). · developer, applied by Claude

- 2026-11-11 · Batch B decisions: q3 is the pre-filled swap variant (`data-dnd-mode="swap"`): the six airport cards start in the storyboard's order (slide 18; the two end cards are already right) and the learner swaps them into order; the check button appears after the first move. The cards, end labels and line are CSS; the flags are the PSD's exported pictures. q4a/q4b: the equation row reads left to right with five slots (number, sign, number, =, result); q4a takes the two numbers in either order, q4b only 1,800,000 first. Help and information texts open as popups beside their buttons (help at the top left, information near the bulb; Escape or a click outside closes). All retry and final boxes sit in the band under the content; `layout_check.py` is clean on screens 7–10. Screens 6 and 10 are the animated stills. · Claude

## Open items
- 24 questions to the content team (`open-questions.md`), not sent yet. The ones that change the build: Q1 audio or video and the missing help hint (12, 13); the partial result and its wording (3); the narration button (10); the scoring/"בוצע בהצלחה" report (1).
- Storyboard slide 40 says "שקף 50-51" and slide 28 "שקפים 35-37" (stale; built as slides 40–41 and 28–30).
- The PSD has frames for the 10 question screens only (the video scenes were cut from 7 to 4). The 4 video screens, the finish and the 5 picture screens use the storyboard's pictures; screens 6 and 16 (and maybe 12) need a generated variant (`SCENE_IMAGES_BRIEF.md`) — waiting on the developer.
- Q6א/Q6ב are **scored applet questions**: the engine has no `kind="applet"` yet. They need a custom piece: the applet posts the drawn height, a `HOOKS` entry grades it, the screen's check button and feedback do the rest. Plan in Phase 5, after looking inside the two applet files.
- Caption times in the 4 videos are even placeholders until the videos and their SRTs arrive. No videos, audio, narration or animations exist yet (question 10 decides the narration button; the small animations are replaced by stills).
- The 5 picture-and-narration screens wait for the generated variants (SCENE_IMAGES_BRIEF.md); the developer said "not now" on 2026-11-11, so screens 6 and 16 keep a placeholder until then.

## Delivery log
<!-- date · git commit · repo link · SharePoint link · what changed since the last one -->
