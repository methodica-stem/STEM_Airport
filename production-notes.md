# Production notes — שדה תעופה

Behaviour and gating from the storyboard's production notes, screen by screen.
Global ("גורף") rules first. Slide numbers are the storyboard's.

## Global rules
- **Forward arrow:** after a video it blinks; a click moves to the next screen, "לאורך כל הלומדה" (slide 8). House default: the arrow shows 3 s before the video ends.
- **Back arrow:** returns to the previous screen, throughout (slide 9).
- **"צדקתי?" button (slide 10):**
  - First wrong answer → the **retry** message: "זו אינה התשובה, נסו שוב." + "תוכלו ללחוץ על כפתור העזרה כדי לקבל רמז."
  - Second wrong answer, or a correct one → the feedback of the next slide (title "צדקת!" / "זו טעות", then the explanation).
- **Help ("עזרה"), slide 15:** shown and hidden by a click on the button, on every question. The hint is the speech bubble at the top of each question slide (listed per screen below).
- **Score (slide 42):** equal weight to each of the 8 questions; a question with parts (4, 6) splits its weight equally between its parts → 12.5 per question, 6.25 per part. Reported to the Moodle: 70 and above = "בוצע בהצלחה", the report includes the score.
- **Design notes "עיצוב" (purple labels on slides 15, 18, 20, 22, 25, 31, 33, 36, 38):** the label is empty of instructions (a leftover marker); nothing to build. Listed in open-questions.md in case a note went missing.
- **Learner text inside notes:** quoted below with its role.

## Screen 1 — video-intro (slides 2–8)
- **Built 2026-11-17:** `AIRPORT_PART1_V2.mp4`, captions from `AIRPORT_PART1_V2.srt`.
- Click on play shows the video of slides 2–8 (slide 2 note).
- Slide 2: a TV news report over footage of a crowded airport; a presenter says (quoted, spoken): "עונת הטיסות בשיאה! שדה התעופה מתמלא בנוסעים, והצוותים נערכים לאחת התקופות העמוסות בשנה." The "camera" moves to the kitchen and the conversation between the son and the mother begins.
- Captions, in order: the presenter line, then the balloons of slides 3, 4, 5, 6, 7, 8.
- Slide 3 carries a line at the bottom: "המספרים במשימה מעובדים על פי נתונים משנת 2025" (see open-questions).
- At the end of the video the arrow blinks (slide 8 note).

## Screen 2 — story-office (slide 9)
- **Built 2026-11-17:** the listen button in the bubble plays `screen2_narration.mp3` (since the later 2026-11-17 decision the voice starts by itself and the arrow waits for its end).
- Narration of the text ("קריינות לטקסט").
- Back arrow returns to the previous slide (note on the slide).

## Screen 3 — q1 (slides 10–11)
- **Built 2026-11-17:** the four reading cards play `q1_matan_narration_<city>.mp3`. The feedback lines' own sound symbols have no recordings yet.
- Four cards, one per city, each with a play symbol (audio): דובאי 95,200,060 · פרנקפורט 63,277,005 · טוקיו 91,679,814 · פריז 72,014,271. The learner chooses the card whose reading is right.
- Every reading needs large, clear captions (the video on screen may be enlarged if needed). What is said in each reading:
  - דובאי — תשעים וחמישה מיליון, אלפיים ושישים נוסעים
  - פרנקפורט — שישים ושלושה מיליון, מאתיים שבעים ושבעה אלף וחמש מאות נוסעים
  - טוקיו — תשעים ואחד מיליון, שש מאות שבעים ותשעה אלף, שמונה מאות וארבעה עשר נוסעים
  - פריז — שבעים ושניים מיליון, מאה וארבעים אלף ומאתיים שבעים ואחד
- Answer: **טוקיו** (the tick on slide 11; the only reading that says the number correctly). Confirm.
- Feedback (slide 11): title, then "לחצו על סמל השמע לצד כל מספר כדי לשמוע איך קוראים נכון את המספרים:" and four lines, each with a sound symbol:
  - פריז: שבעים ושניים מיליון, ארבעה עשר אלף, מאתיים שבעים ואחד נוסעים.
  - טוקיו: תשעים ואחד מיליון, שש מאות שבעים ותשעה אלף, שמונה מאות וארבעה עשר נוסעים.
  - פרנקפורט: שישים ושלושה מיליון, מאתיים שבעים ושבעה אלף וחמישה נוסעים.
  - דובאי: תשעים וחמישה מיליון, מאתיים אלף ושישים נוסעים.
- The PSD has a help button and a hidden help bubble for this question; the storyboard has neither (open-questions).

## Screen 4 — video-estimate (slides 12–14)
- **Built 2026-11-17:** `AIRPORT_PART2_V2.mp4`, captions from its `.srt`.
- Click on play shows the video of slides 12–14. Captions: the balloons of 12, 13, 14. End: arrow.

## Screen 5 — q2 (slides 15–16)
- Help hint (balloon, slide 15): "כאשר מעגלים מספרים, מציגים אותם בצורה פחות מדויקת אך נוחה יותר לאומדן. הסימן ≈ מציין את המספר המעוגל ש"קרוב" למספר הנתון אך אינו שווה לו."
- Three rows, each "city: exact number ≈ [box]" and two blue chips (the two candidate roundings). The learner drags the right chip into each box.
  - אמסטרדם 68,776,052 ≈ **68,780,000** (other chip 68,770,000)
  - ניו יורק 62,568,432 ≈ **62,570,000** (other chip 62,560,000)
  - וינה 32,634,803 ≈ **32,630,000** (other chip 32,640,000)
- Answer slide (16): the right chips are in the boxes; the wrong ones stay at the left.
- Feedback: "המספרים המעוגלים הנכונים מוצגים כעת. / כדי לעגל לעשרות אלפים, נבדוק את ספרת האלפים: / אם היא 5 ומעלה, נעגל כלפי מעלה, ואם היא קטנה מ-5, נעגל כלפי מטה."

## Screen 6 — story-data (slide 17)
- **Built 2026-11-17:** listen button + `screen6_narration.mp3`; the small animation is `screen6_animated.mp4`, a silent loop over the still (it replaces the "dropped" note below).
- Narration of the text. The note asked for a small animation (the mother smiles and looks at Matan); the video was cut, so this is now a still: a variant of the repeating picture (SCENE_IMAGES_BRIEF.md, prompt A).

## Screen 7 — q3 (slides 18–19)
- "שאלת גרירה וסידור על הקו האופקי. תגית הגדול ביותר מימין, הקטן ביותר בשמאל. לשים דגל מדינה ליד כל שדה תעופה."
- Six airport cards (name, city/country, passengers, flag), dragged onto a horizontal line, ends labelled "מספר הנוסעים הגדול ביותר" (right) and "מספר הנוסעים הקטן ביותר" (left). Right order, right → left, largest → smallest: הית'רו 15,000,000 · שארל דה גול 12,310,000 · פרנקפורט 11,890,000 · אל פראט 11,490,000 · סכיפהול 11,350,000 · פיומיצ'ינו 11,150,000.
- Help hint: "בשדה התעופה ברומא עובר מספר הנוסעים הנמוך ביותר."
- Info icon (opens): "כאשר מעגלים מספרים לעשרות אלפים, רושמים את המספר השלם בעשרות אלפים הקרוב לו ביותר. / לדוגמה: את המספר 12,486,743 מעגלים לעשרות אלפים ומקבלים 12,490,000."
- Answer slide (19): "הפקה: להציג את התשובה הנכונה" — the cards in the right order.
- Feedback: "כעת שדות התעופה מסודרים מהקטן לגדול לפי מספר הנוסעים שעברו בהם."

## Screen 8 — q4a (slides 20–21)
- Build an equation from chips: two numbers and an operation, then drag the result to its place too. Right: 1,600,000 + 1,800,000 = 3,400,000. **The two numbers may sit in either of their two places** (slide 21 note).
- Chips: 1,800,000 · 3,400,000 · 1,600,000 · 200,000 · − · 3,040,000 · 3,004,000 · 20,000 · 2,000 · +
- Help hint: "סך כל הנוסעים הוא תוצאה של תרגיל חיבור." Info icon (opens): "ניתן לעגל מספרים לעשרות אלפים, מאות אלפים, מיליונים וכדומה, לפי הצורך."
- Feedback: "מספר העוברים בשדה התעופה הוא הסכום של מספר היוצאים ומספר הנכנסים. / החישוב: 3,400,000 = 1,800,000 + 1,600,000"

## Screen 9 — q4b (slides 22–23)
- Same mechanism. Right: 1,800,000 − 1,600,000 = 200,000. Chips: 1,800,000 · 3,400,000 · 200,000 · 20,000 · 1,600,000 · − · +
- Help hint: "הפרש הוא תוצאה של תרגיל חיסור."
- Feedback: "יש להפחית את מספר הנוסעים שנכנסים ממספר הנוסעים שיוצאים. / החישוב: 200,000 = 1,600,000 – 1,800,000" (the line is typed in the RTL order of the storyboard; it reads 1,800,000 – 1,600,000 = 200,000 on the slide).

## Screen 10 — story-holiday (slide 24)
- **Built 2026-11-17:** the small animation is `screen10_animated.mp4` (silent loop over the still); listen button + `screen10_narration.mp3`.
- Narration of the text. The note asked for a small animation (Matan remembers the holiday happily); now a still, and the storyboard picture already shows it.

## Screen 11 — q5 (slides 25–26)
- Four descriptions (children / adults / all passengers in July–August; adults in one month) each with a box above it; six expression chips; **two chips have no description** ("שימו לב: יש שני תרגילים שאין להם תיאור מתאים").
- Right matches (as the slide shows them, RTL-ordered text):
  - מספר הילדים … יולי-אוגוסט → 62 × 10,000
  - מספר המבוגרים … יולי-אוגוסט → 62 × (10,000 - 70,000)
  - מספר הנוסעים … יולי-אוגוסט → 62 × 70,000
  - מספר המבוגרים … בחודש אחד → 2 : 62 × (10,000 - 70,000)
  - Not used: "62 × 10,000 - 70,000" and "2 : 62 × 10,000 - 70,000"
- Help hint: "מספר המבוגרים הוא ההפרש בין מספר הנוסעים למספר הילדים. / שימו לב לסדר פעולות חשבון."
- Feedback: "כדי לבחור את התרגיל הנכון, חשוב להבין מה מבקשים לחשב. / התשובות הנכונות מוצגות כעת, השוו אותן לתשובתכם."

## Screen 12 — story-team (slide 27)
- **Built 2026-11-17:** listen button + `screen12_narration.mp3`; code animation only (no clip).
- Narration of the text.

## Screen 13 — video-chart (slides 28–30)
- **Built 2026-11-17:** `AIRPORT_PART3_V2.mp4`, captions from its `.srt`.
- Click on play shows the video of slides 28–30 (the note says "35-37": a stale number, see open-questions). End: arrow.

## Screens 14, 15 — q6a, q6b (slides 31–34): the graph applet
- "ליצור יישומון גרפים": the learner draws **on the existing diagram**. The applet shows an interactive drawing area where the child "raises" the column's rectangle from the axis below, drags it up and stops at the right place against the left axis. A click on "צדקתי?" shows the solution and the feedback.
- The applet files are in `STEM/שדה תעופה/applets/` (one per part).
- q6a: draw the column for נובמבר-דצמבר = 2,400,000. q6b: the column for ספטמבר-אוקטובר = 2,900,000 (the Nov–Dec column is already drawn at 2,400,000).
- Help hints: q6a "כדי למצוא כמות שהיא פי 2 מכמות אחרת, כופלים את הכמות ב-2." · q6b "כדי למצוא את מספר הנוסעים שעברו בחודשים ספטמבר-אוקטובר, יש לבצע תרגיל חיסור."
- Design/production note: the numbers and the months must be accessible in size, readability and alt text.
- Feedback q6a: "פי 2 מ-1,200,000 הם: / 1,200,000 × 2 = 2,400,000 / כלומר, בנובמבר-דצמבר עברו כ-2,400,000 נוסעים." (garbled in the storyboard text, clean on the slide picture).
- Feedback q6b: "נחסר 1,400,000 ממספר הנוסעים בחודשים יולי-אוגוסט: / 4,300,000 – 1,400,000 = 2,900,000 / בספטמבר-אוקטובר עברו כ-2,900,000 נוסעים."

## Screen 16 — story-daily (slide 35)
- **Built 2026-11-17:** listen button + `screen16_narration.mp3`; the small animation is `screen16_animated.mp4`, a silent loop over the still (it replaces the "dropped" note below).
- Narration of the text. The note asked for a small animation (the mother looks at the data, then at the team, who nod); now a still: a variant of the repeating picture (SCENE_IMAGES_BRIEF.md, prompt C).

## Screens 17, 18 — q7, q8 (slides 36–39)
- Typed answer with a unit after the box ("טיסות." / "מזוודות."). q7: **200**. q8: **100,000**.
- Help hints: q7 "מספר הטיסות הוא תוצאה של תרגיל חילוק." · q8 "כדי למצוא שליש של מספר, עלינו לחלק אותו ב-3."
- Feedback q7: "כדי למצוא את מספר הטיסות יש לחלק את 60,000 ב-300, כך: / 200 = 300 : 60,000". Feedback q8: five steps (25,000 = 3 : 75,000; 50,000 = 2 × 25,000; 50,000 = 25,000 – 75,000; 100,000 = 50,000 + 50,000).
- q8's stem has a fraction, one third, written 1/3 in the slide's equation.

## Screen 19 — finish (slides 40–42)
- **Built 2026-11-17:** `AIRPORT_PART4_V2.mp4`, captions from its `.srt`.
- Click on play shows the video of slides 40–41 (note says "50-51": stale). At the end of the video the "סיימתי" button appears (slide 41 note).
- Slide 42 = the score pop-up: "כל הכבוד, המשימה הושלמה!" / "הציון שלך הוא __." / "יש לסגור את המשימה בלחיצה על X." The house ending (score pop-up → dark Moodle screen) applies.
