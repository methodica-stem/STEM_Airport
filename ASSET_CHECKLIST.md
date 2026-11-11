# Asset checklist — pictures exported from the PSD

Everything goes into `assets/images/`. Claude exports the rows with
`psd_export.py`, then ticks them (☐ → ✔) once `check_assets.py` agrees.
All text is live HTML, so no picture is exported with words in it.

## Shared (once for the whole lomda)
| ✔ | file | PSD layer | x | y | w | h | how |
|---|---|---|---|---|---|---|---|
| ✔ | `assets/images/bg-airport.jpg` | `#2 10` | 0 | 0 | 1920 | 1080 | the airport-office background with its darkening; the same in all 10 question frames; no white panel, no buttons. [hide: משטח שאלה] [hide: עזרה - חלונית] [hide: כפתור עזרה] [hide: תוכן שאלה] [hide: סרטונים] [hide: בחירת סרטון] [hide: צדקתי?] [hide: חיצים] [hide: מספרי שאלות] |
| ✔ | `assets/images/ui-help.png` | `#2 10/כפתור עזרה` | 71 | 48 | 120 | 120 | blank chalkboard circle, the label "עזרה" is HTML (the inventory box 162×162 includes the shadow, which CSS draws) [shadow] |
| ✔ | `assets/images/ui-check.png` | `#2 10/צדקתי?` | 250 | 857 | 227 | 155 | blank chalkboard button, the label "צדקתי?" is HTML [shadow] |
| ✔ | `assets/images/ui-btn-next.png` | `#2 10/חיצים/כפתור קדימה` | 71 | 936 | 103 | 103 | forward arrow (left side, RTL) [shadow] |
| ✔ | `assets/images/ui-btn-prev.png` | `#2 10/חיצים/כפתור אחורה` | 1720 | 936 | 103 | 103 | back arrow (right side, RTL) [shadow] |
| ✔ | `assets/images/ui-chip.png` | `#3 15/תוכן שאלה/כרטיס` | 311 | 445 | 290 | 76 | the blue-grey glass button every drag chip uses; stretched with border-image so the text can grow |
| ✔ | `assets/images/ui-bulb.png` | `#4 20/תוכן שאלה/נורה` | 1137 | 299 | 95 | 95 | the light-bulb "information" button, used in questions 3 and 4א [shadow] |

## Screen 3 — q1 (PSD frame 2)
| ✔ | file | PSD layer | x | y | w | h | how |
|---|---|---|---|---|---|---|---|
| ✔ | `assets/images/q1-reader-1.png` | `#2 10/סרטונים/סרטון 1` | 1314 | 339 | 304 | 342 | the picture of Matan reading, card 1 (right) [shadow] |
| ✔ | `assets/images/q1-reader-2.png` | `#2 10/סרטונים/סרטון 2` | 993 | 339 | 304 | 342 | card 2 [shadow] |
| ✔ | `assets/images/q1-reader-3.png` | `#2 10/סרטונים/סרטון 3` | 674 | 339 | 304 | 342 | card 3 [shadow] |
| ✔ | `assets/images/q1-reader-4.png` | `#2 10/סרטונים/סרטון 4` | 353 | 339 | 304 | 342 | card 4 (left) [shadow] |

## Screen 7 — q3 (PSD frame 4)
| ✔ | file | PSD layer | x | y | w | h | how |
|---|---|---|---|---|---|---|---|
| ☐ | `assets/images/q3-flag-uk.png` | `#4 20/תוכן שאלה/שדות תעופה/דגלים/1 copy` | 1600 | 611 | 512 | 170 | the flag under הית'רו (United Kingdom); the box is wider than a flag, check the result [trim] |
| ☐ | `assets/images/q3-flag-de.png` | `#4 20/תוכן שאלה/שדות תעופה/דגלים/2` | 1323 | 610 | 165 | 93 | Germany, under פרנקפורט |
| ☐ | `assets/images/q3-flag-es.png` | `#4 20/תוכן שאלה/שדות תעופה/דגלים/3` | 1032 | 601 | 195 | 98 | Spain, under אל פראט |
| ☐ | `assets/images/q3-flag-nl.png` | `#4 20/תוכן שאלה/שדות תעופה/דגלים/4` | 768 | 608 | 172 | 89 | Netherlands, under סכיפהול |
| ☐ | `assets/images/q3-flag-fr.png` | `#4 20/תוכן שאלה/שדות תעופה/דגלים/5` | 493 | 601 | 184 | 95 | France, under שארל דה גול |
| ☐ | `assets/images/q3-flag-it.png` | `#4 20/תוכן שאלה/שדות תעופה/דגלים/6` | 216 | 609 | 172 | 83 | Italy, under פיומיצ'ינו |

## Screen 17 — q7 (PSD frame 10)
| ✔ | file | PSD layer | x | y | w | h | how |
|---|---|---|---|---|---|---|---|
| ☐ | `assets/images/q7-airplane.png` | `#10 43/תוכן שאלה/מטוס` | 616 | 651 | 760 | 473 | the airplane picture; it runs below the panel in the design, so the whole picture is exported [original] |

## Screen 18 — q8 (PSD frame 11)
| ✔ | file | PSD layer | x | y | w | h | how |
|---|---|---|---|---|---|---|---|
| ☐ | `assets/images/q8-suitcase.png` | `#11 45/תוכן שאלה/תמונה - מזוודה` | 22 | 327 | 771 | 514 | the suitcase on the conveyor belt; the design crops it at the panel's left edge, so the whole picture is exported [original] |

## Rebuilt in code (not exported, on purpose)
- **The white question panel** (layer `משטח שאלה`): drawn in CSS at the house size, not exported with the background.
- **Stepper pills 1–8** (group `מספרי שאלות`): the engine draws them; the colours are in the tokens.
- **Drag cards, drop slots, answer boxes, the airport cards and end labels of question 3, the line between them** (`כרטיס`, `כרטיס פעולה`, `שדה הקלדה`, `אזור שחרור`, `כרטיס שדה`, `תווית - …`, `פס סדר`): CSS shapes; the chips use `ui-chip.png` as their skin.
- **The two help bubbles** (`עזרה - חלונית`, `מידע - חלונית`): CSS popups; the PSD's help bubble is a picture the designer's own layer name calls "not good" (פופואפ לא טוב), and the text is HTML anyway.
- **The fraction bar of question 8** (`קו שבר`): the fraction is live text.
- **The radio circles of question 1** (`בחירה 1–4`): CSS radios.
- **The bar charts of question 6** (`גרף/תרשים`, the columns): the two applets draw the chart. The design's chart picture has Hebrew painted into it, so it would need re-making for Arabic.
- **The picture-and-narration screens, the four video screens and the finish screen**: no PSD frame (see `SCENE_IMAGES_BRIEF.md`).
