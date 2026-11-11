# Progress — שדה תעופה (airport)

Claude keeps this file up to date. Every session starts by reading it and ends
by updating it, so work can stop and resume at any point.

**Now:** Phase 0 done · waiting for the developer to confirm folder and inputs, then Phase 1 (read the storyboard, build the screen map)
**Waiting on you:** confirm the inputs below are the right ones (see "Inputs")
**Waiting on others:** nothing yet

## Inputs
All in `STEM/שדה תעופה/` (inputs stay there; never copied into the project):
- Storyboard: `שדה תעופה_אחרי עריכה לשונית וצמצום סרטונים.pptx` — 42 slides, language-edited, videos reduced
- PSD: `airport_stem.psd` — 1920×1080, 10 frames, **question screens only** (Q1, Q2, Q3, Q4א, Q4ב, Q5, Q6א, Q6ב, Q7, Q8)
- Comps: `airport_03.11.26.pptx` — 12 pictures of the design
- Applets: `applets/ספטמבר-אוקטובר.html`, `applets/נובמבר-דצמבר.html`
- Project folder: `STEM/שדה תעופה/הפקה/airport/` · preview: `airport` on port 8135 (entry added to the launch.json of `פיתוח STEM`)

## Phases
- [x] 0 · Setup — inputs found, tools installed, project folder created (2026-11-11)
- [ ] 1 · Storyboard read — screen map (screens.json, PROJECT_BRIEF.md), production-notes.md, open-questions.md
- [ ] 1 · ✋ Developer reviewed the screen map; open questions sent (date: )
- [ ] 2 · Design reference — PSD inventory, frames mapped to screens, mockups for the overlay
- [ ] 3 · ASSET_CHECKLIST.md written
- [ ] 3 · ✋ Assets exported by the developer and checked (check_assets.py clean)
- [ ] 4 · Screens built (tick per batch below)
- [ ] 5 · Applets built and signed off; videos and audio in
- [ ] 6 · Self-QA passed (qa_check.py 0 errors, walk-through done)
- [ ] 7 · Translation export done (both sweeps pass), ASSET_LOCALIZATION.md written
- [ ] 8 · ✋ Delivered: repo pushed (published to the org the first time), SharePoint shortcut and snapshot updated, links sent

## Screens
| # | sid | built | matches design | approved by developer |
|---|---|---|---|---|
| — | screen map not made yet (Phase 1) | | | |

## Decisions
- 2026-11-11 · Version check storyboard ↔ design: same 8 questions, same numbering (1, 2, 3, 4א/ב, 5, 6א/ב, 7, 8 = the 10 PSD frames). Stems differ only in small wording (e.g. Q1: design "הקשיבו להקראה ובחרו את הסרטון שבו הוא הקריא נכון", storyboard "הקשיבו להקראות ובחרו את ההקראה שבה מתן קרא נכון"). The storyboard is the language-edited one, so learner text comes from it and looks from the PSD. Build goes ahead. · Claude

## Open items
- Slide 40 of the storyboard refers to slide 51, which does not exist (reader flag) → goes to open-questions.md in Phase 1.
- The PSD has frames only for the question screens. The video, story and finish screens (storyboard slides 2–9, 40–42) have no PSD frame: their looks come from the storyboard's pictures. To raise with the developer / designer in Phase 2.

## Delivery log
<!-- date · git commit · repo link · SharePoint link · what changed since the last one -->
