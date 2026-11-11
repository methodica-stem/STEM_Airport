# Open questions — שדה תעופה

For the content team unless it says otherwise. Each has the slide, what the
storyboard says, and what I suggest. Building does not wait for the answers;
the suggested answer is what I build with until then.

## Behaviour and scoring

**1 · Scoring: passing grade and "בוצע בהצלחה" (slide 42)**
The note says a score of 70 and above is reported as "בוצע בהצלחה", with the score. The lomda only sends the score (0–100) to the Moodle (`LOMDA_COMPLETE`). Does the Moodle apply the 70 rule itself, or must the lomda send a status as well?
*Suggestion:* the lomda sends the score only; the Moodle decides the status. Please confirm with whoever owns the Moodle side.

**2 · The ending's wording (slide 42, house text)**
The finish uses the approved house ending: score pop-up, then a dark screen: "כעת חזרו אל המודל, לחצו על הכפתור "העמוד הבא" וענו על השאלות." Is "העמוד הבא" the label of the next-page button in this Moodle quiz?

**3 · "זו טעות" and the partial result (every question)**
The storyboard's title is "צדקת! / זו טעות". The house wording for a final wrong answer is "זו טעות, כל הכבוד על הניסיון." I built the storyboard's "זו טעות". Please say which one you want.
Questions 2, 3, 4א, 4ב and 5 have several parts to get right, so they need a third result for an answer that is partly right: I wrote **"נכון חלקית"** (new wording, not in the storyboard) with the same explanation as "זו טעות". Please confirm the wording, and say whether a partly right answer earns part of the points (until you answer, it earns 0).

**4 · Retry text on the first wrong answer (slide 10 note)**
"זו אינה התשובה, נסו שוב. תוכלו ללחוץ על כפתור העזרה כדי לקבל רמז." is built for every question, as the note says "לאורך כל הלומדה". Question 7 and 8 have a typed answer: the same text fits. OK?

## Slide-by-slide

**5 · No opening screen (slide 1)**
Slide 1 is marked "לא להפקה", so the first screen of the lomda is the video (slides 2–8), with its play button. There is no title or "start" screen.
*Suggestion:* leave it as is. Please confirm that nothing should come before the video.

**6 · Stale slide numbers in the notes (slides 28 and 40)**
Slide 28 says "שקפים 35-37" and slide 40 says "שקף 50-51", but those videos are slides 28–30 and 40–41. I built them that way. Please confirm.

**7 · The line on slide 3: "המספרים במשימה מעובדים על פי נתונים משנת 2025"**
Is it painted into the video, or a line on the screen? *Suggestion:* a line on the screen, at the bottom of the video, visible all through the video (so it is real text and can be translated).

**8 · Stage directions inside speech balloons (slides 6 and 41)**
Slide 6: "(צוחקת)". Slide 41: "(אמא ומתן צוחקים ביניהם, והאחרים מביטים בהם בחיוך שמסגיר שלא הבינו את הבדיחה הפרטית)". These are directions for the video, not spoken words. *Suggestion:* take them out of the captions (captions follow the voice).

**9 · The news presenter's line (slide 2 note)**
The note quotes what the presenter says: "עונת הטיסות בשיאה!…". I put it as the first caption of the video. Is that right, or is the presenter silent on screen?

**10 · Narration of the story screens (slides 9, 17, 24, 27, 35)**
The notes say "קריינות לטקסט" / "הקראה של הטקסט". House rule: no sound plays on its own. *Suggestion:* a small "listen" button beside the text. Does the lomda need an auto-play instead? Who records the narration?

**11 · The small animations are replaced by still pictures (slides 17, 24, 35)**
The notes ask for "אנימציה קטנה (כמו תמונת לייב באייפון)". The script had 7 videos and now has 4, so these scenes are pictures with narration. We will use the lomda's repeating pictures and make slightly altered versions where a scene needs one (see `SCENE_IMAGES_BRIEF.md`). Please confirm that the animation notes are dropped.

## Question 1 (slides 10–11)

**12 · Audio or video? And which one is right?**
The storyboard shows four cards with a sound symbol and a wave; the note speaks of "כתוביות גדולות" and "הסרטון המוצג על המסך"; the design calls them "סרטון 1–4" and says "בחרו את הסרטון". Are the four readings audio clips (with captions) or video clips? The design settles it only in part: each card shows a picture of Matan holding a paper, with a play button (so, video), while the storyboard draws a sound wave.
The correct card is not marked in the text. From the readings in the note, **טוקיו** is the only one read correctly (the tick on slide 11 is on it too). Please confirm. The reading of the numbers in the note for דובאי, פרנקפורט and פריז are wrong on purpose (e.g. פריז "מאה וארבעים אלף" instead of "ארבעה עשר אלף").

**13 · Help button on question 1**
The design has a help button and a hidden help bubble on question 1; the storyboard has no help button and no hint on slide 10. Note "זו העזרה… לאורך כל השאלות בלומדה" suggests every question has one. What is the hint of question 1? (I left the button out until I hear.)

**14 · Wording differs between the storyboard and the design (slide 10)**
Design: "הקשיבו להקראה ובחרו את הסרטון שבו הוא הקריא נכון את מספר הנוסעים". Storyboard (language-edited): "הקשיבו להקראות ובחרו את ההקראה שבה מתן קרא נכון את מספר הנוסעים." I use the storyboard's. The designer should update the design.

## Questions 2–5

**15 · Question 4ב: the order of the numbers (slides 22–23)**
For the subtraction, the numbers must be in the order 1,800,000 − 1,600,000 (slide 23). The note on slide 21 says that for the addition either order counts. I built: addition — either order; subtraction — only 1,800,000 first. Also: are the chips' places (number, sign, number, result) fixed, so that "200,000" cannot sit before the "="? *Suggestion:* yes, fixed.

**16 · Question 3: the flags (slide 18 note)**
"לשים דגל מדינה ליד כל שדה תעופה." Flags come from the pictures on the slide/design. Please confirm the six countries: בריטניה, צרפת, גרמניה, ספרד, הולנד, איטליה.

**17 · The info icons (slides 18 and 20)**
The note opens a text when the learner presses an information icon. The icon has no label in the storyboard. I label it "מידע" for screen readers. The same goes for the sound symbols on question 1 (I will label them "השמעה"). OK?

**18 · The "עיצוב" notes (slides 15, 18, 20, 22, 25, 31, 33, 36, 38)**
There is a purple box "עיצוב" with no instruction on each. Was there a design remark that went missing, or are they leftovers?

## Questions 6–8

**19 · Question 6: the answer when the learner draws a column (slides 31, 33)**
The learner drags a column up to a height. How near to 2,400,000 / 2,900,000 counts as right? *Suggestion:* a small tolerance, about half a division of the axis (I will look at the two applet files you sent before I fix a number). Does a wrong try give the retry text, then the solution on the second? (As in the other questions.)

**20 · Question 6: feedback text of 6א is damaged in the file (slide 32)**
The text reads "× 2 = 2,400,0001,200,000" and ends with a doubled "נוסעים. נוסעים." The slide's picture shows it right. I used: "פי 2 מ-1,200,000 הם: 1,200,000 × 2 = 2,400,000 כלומר, בנובמבר-דצמבר עברו כ-2,400,000 נוסעים." Please confirm. (The feedback box in the storyboard is also too small for its text.)

**21 · The graph's alt text (slides 31 and 33)**
The design note asks for accessible numbers, months and alt text. I need the wording for the chart's description. *Suggestion:* I write one from the chart's data (five columns and their values), and you approve it.

**22 · Question 8: spacing in the stem (slide 38)**
The stem reads "כ- 75,000נוסעים" (a space is missing and one is in the wrong place). I wrote "כ-75,000 נוסעים", as on the slide. OK?

**23 · Typed answers (slides 36–39)**
Q7: 200. Q8: 100,000. I will accept "100000" and "100,000" and any other way of writing the same number. OK?

## For the designer

**24 · The design has no frames for 9 screens**
The PSD has the 10 question frames only. The video screens and the five picture-and-narration screens have no frame, because the scenes that were videos were cut back. They use the pictures in the storyboard (image2, 3, 7, 9, 17, 19, 30) and the new variants in `SCENE_IMAGES_BRIEF.md`. If a designed version exists, please send it.
