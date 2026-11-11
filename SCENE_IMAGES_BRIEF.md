> **Update 2026-11-11:** the developer uploaded the generated pictures to `STEM/שדה תעופה/תמונות מגונרטות/` and they are the ones in the lomda. Variant A (screen 6) is not needed: the picture already shows the mother smiling at Matan. The scenes are animated in code (slow drift and pulsing light, like park-drones). Variants B and C are still optional.

# Scene pictures for the screens that lost their video

The script first had 7 videos; budget cut it to 4. Five screens that were once
videos are now **a picture with narration**: 2 (story-office), 6 (story-data),
10 (story-holiday), 12 (story-team), 16 (story-daily). They have no PSD frame.

**Decision (developer, 2026-11-11):** use the base pictures that already repeat
in the lomda, and generate a slightly altered version for the scenes that need
one. The "small animation" notes on slides 17, 24 and 35 no longer apply as
animations (confirm with the content team, open question 11).

The base pictures were taken from the storyboard and are in
`_design-reference/scene-bases/` (1672×941, 16:9; the lomda stage is 1920×1080,
so a generated version should be made at 1920×1080 or larger).

## What each screen needs

| Screen | Slide | Base picture now | What the storyboard note asks for | What to make |
|---|---|---|---|---|
| 2 story-office | 9 | `image3` — the mother's office, Matan leaning on the desk. The same picture is the background of question 1 | narration only | **Nothing new.** The picture as it is. |
| 6 story-data | 17 | `image7` — Matan with his chin on his hand beside his mother at the desk. The same picture is the background of the video "מה זה אומדן?" and of question 2 | the mother smiles and looks at Matan | **A variant** (prompt A) |
| 10 story-holiday | 24 | `image17` — Matan smiling, remembering. This picture is already its own variant | Matan looks up, remembering the holiday happily | **Nothing new.** Already made. |
| 12 story-team | 27 | `image19` — the mother and Matan with the team around the table. The same picture is the background of the chart video and of questions 6–8 | narration only: "אמא של מתן הציגה את הדו"ח לצוות שלה." | **Optional variant** (prompt B): the mother presenting to the team |
| 16 story-daily | 35 | `image19` — exactly the same file as slide 27 | the mother looks at the data, then at the team, who nod in agreement | **A variant** (prompt C), different from the one on screen 12 |

So the work is **two or three new pictures**: A, C, and B if you want screen 12
to differ from the chart video behind it.

## Prompts (for an image model, with the base picture attached as the reference)

Common part, put at the start of every prompt:

> Edit the attached picture. Keep everything the same: the same characters (same faces, hair, clothes and ages), the same room and window view, the same lighting, colours and 3D-animation style, the same camera position and framing, 16:9. Change only what is described below. Do not add text, logos or new people. Keep the top right corner of the picture calm: a text bubble will be placed there.

- **A — screen 6 (base `image7`):** "The mother is smiling warmly and looking down at her son Matan, who rests his chin on his hand. Her eyes are on him, not on the tablet. Matan keeps his thoughtful expression."
- **B — screen 12 (base `image19`), optional:** "The mother is presenting the report to the team: she holds the tablet up toward them with one hand and gestures at the screen with the other. The team members look at her with interest."
- **C — screen 16 (base `image19`):** "The mother looks at the tablet data in her hands, with a thinking expression. The four people around the table look toward her and nod in agreement with a small friendly smile. Matan leans on his hand and looks at the tablet."

## Rules for the result
- 1920×1080 or larger, 16:9, PNG or high-quality JPG. Send it to Claude; Claude resizes it, checks it against the base (the characters must still look like the same people, and the faces must not be covered by the narration bubble at the top right) and puts it in `assets/images/<sid>-bg.jpg`.
- Compare it with the base side by side before accepting: faces, hands and the tablet are where generated pictures drift.
- Any text in the picture is not allowed (it would need to be redone for Arabic).
- Record in `ASSET_LOCALIZATION.md` that these pictures are text-free.
