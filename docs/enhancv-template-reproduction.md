# Reproducing the Enhancv resume templates

Measured from the editor bundle and the preview files served by app.enhancv.com on 11 November 2026. These are the factory settings a new resume receives when a template is chosen. The design panel can change color, font, spacing, and column width afterward. It cannot change the column count.

Use this with [enhancv-resume-templates.md](enhancv-resume-templates.md), which has Enhancv’s own description of each layout and what the official preview shows.

## Page

The editor draws the page at **940 × 1330 px** for A4. US Letter keeps the width and uses height **1216 px**.

Page padding is one of 28, 36, 44, 50, 60 px, taken from the template’s page-margin step (0 through 4). The bottom padding of the page box is 0. A footer, when shown, consumes 50 px of the content height. The footer is “www.enhancv.com” on the left and “Powered by Enhancv” on the right, in the body color, until branding is removed.

Body text color is **#3e3e3e**, except Crest, which sets **#1f1b17**.

## Color

Each template stores two colors. Index 0 is primary. Index 1 is the accent.

| Use | Color |
| --- | --- |
| Name, on the headers that set a text color | Primary |
| Target title | Accent |
| Section title | Primary, in the heading font |
| Job title | Primary, in the heading font |
| Employer | Accent, in the heading font |
| Contact icons | Accent |
| Elegant and Polished sidebar fill | Accent |
| Creative header band | Accent |
| Skill meter, second stop | Accent |

Creative’s header stylesheet paints the name and title **white**, which replaces the primary and accent on that band. Crest’s name is **#392716** at weight 300. Imprint’s name is **#1d1d1f** at weight 300. Those stylesheet colors replace the primary on the name only.

Background `b00` means no background image. Compact uses `b22Colored`. Crest uses `b36Cream`.

The gallery recolors the same template. A rust sidebar or a pink header on enhancv.com is a recolor, not a second template. The pairs below are the factory pairs.

## Type

Heading weight is **500 for Rubik** and **700 for every other heading family**, unless a stylesheet overrides it. The overrides are the Crest and Imprint names at 300, Classic and Compact names at 400, and Modern and Multicolumn names at 500.

| Template | Headings | Body |
| --- | --- | --- |
| Double column, Single column, Classic, Modern, Stylish, Elegant, Polished, Contemporary, Creative, Compact, Multicolumn, Minimal | Rubik | Inter |
| Ivy League | Volkhov | PT Sans |
| Timeline | Montserrat | Open Sans |
| High Performer | Raleway | Open Sans |
| Crest | EB Garamond | EB Garamond |
| Imprint | Cormorant Garamond | Inter |

The font-size control has five steps, indexed 0 to 4. Every size below is the pixel size at the template’s factory step. The five-step list is included so a rebuild can offer the same slider.

Line height, in pixels, is the font’s metric for that pixel size, plus the template’s line-height step. Crest’s step is 2. Imprint’s step is 1. Every other template’s step is 0. If the metric table has no entry for that size, the line height is the unitless value 1. The metrics for the factory fonts are at the end.

## Columns

| Columns | Templates |
| --- | --- |
| 1 | Ivy League, Crest, Imprint, Timeline, Single column, Classic |
| 2 | Double column, Elegant, Modern, Polished, Contemporary, Creative, Stylish, Compact, High Performer, Minimal |
| 3 | Multicolumn |

The factory column-width step is the second of four (index 1).

Double column, Modern, Creative, Compact, High Performer, and Minimal use `1fr 40%`. The left column is the story. The right column is 40%. The four steps are 36%, 40%, 44%, 48% on the right column. The column gap is 12, 12, 16, 16, or 24 px at the same index, so the factory gap is **16 px**.

Multicolumn uses `1fr 40% 1fr`. The middle column is the 40% one.

Elegant, Polished, Stylish, and Contemporary use a fixed sidebar of `326 − adjustment − page padding` pixels. The factory adjustment is 0. The four adjustments are +10, 0, −10, −20, so later thumbnails make the sidebar wider.

| Template | Sidebar | Factory width |
| --- | --- | --- |
| Elegant | Right. 22 px extra padding on its left edge. | 290 px. Page padding is 36. |
| Polished | Left. The story column is placed on the right. 22 px extra padding on the sidebar’s right edge. | 290 px. Page padding is 36. |
| Stylish | Left. The story column is placed on the right. | 276 px. Page padding is 50. |
| Contemporary | Left. The story column is placed on the right. | 266 px. Page padding is 60. |

The painted sidebar, on Elegant and Polished only, is `326 − adjustment` pixels wide and uses the accent. At the factory adjustment that is 326 px, which is wider than the content column because the content column also subtracts the page padding.

Section spacing under each block is 8, 12, 14, 16, or 18 px at margin steps 0 through 4.

## The 17 factory specs

Sizes are the factory step. “Name / title” is the header. “Section” is the section label. “Job / employer / body” is one experience entry: job title, employer, then the description size. Dates follow the body unless a separate date size is given.

### 1. Double column

Id `double`. French: Deux colonnes.

Two columns, story on the left, right column 40%. No sidebar paint.

Colors **#000000**, **#1E90FF**. No background. Rubik and Inter. Name in capitals. Icons on. Page padding 50. Section gap 8, the tightest step. Font step 2. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name, five steps | 30, 34, **38**, 42, 42 |
| Title | 15, 17, **19**, 21, 21 |
| Contacts | 12, 12, **12**, 13, 13 |
| Photo diameter | 110, 125, **135**, 150, 150 |
| Section label | 16, 18, **20**, 22, 24 |
| Job title | 14, 15, **17**, 18, 19 |
| Employer | 13, 14, **15**, 16, 17 |
| Description and bullets | 12, 12, **13**, 14, 15 |
| Date and location | 11, 11, **12**, 13, 13 |

The official preview has no photo. The header still supports one, on the right, at 135 px.

### 2. Ivy League

Id `ivyleague`. French: Harvard.

One column. Centered header. Section labels are title case, not capitals. This is the only template with section capitals turned off.

Colors **#000000**, **#6F7878**. No background. Volkhov and PT Sans. Name in capitals. Page padding 50. Section gap 12. Font step 2. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 18, 20, **22**, 24, 28 |
| Title | 14, 16, **18**, 20, 20 |
| Contacts | 13, 13, **13**, 14, 14 |
| Photo diameter | 96, 100, **110**, 130, 130 |
| Section label | 14, 16, **18**, 20, 20 |
| Job title | 13, 14, **15**, 16, 16 |
| Employer | 14, 16, **18**, 20, 20 |
| Description and bullets | 12, 12, **13**, 14, 15 |
| Dates | 13, 14, **15**, 16, 16 |

The official preview has no photo. The photo shape, if turned on, is a circle. Key achievements in that preview is three text columns inside the one page column. Skills in that preview is one dotted line.

### 3. Elegant

Id `elegant`. French: Élégant.

Story on the left. Accent sidebar on the right, 290 px of content, 326 px of paint. Round photo at the top of the sidebar.

Colors **#008CFF**, **#22405C**. No background. Rubik and Inter. Name in capitals. Icons on. Page padding 36. Section gap 14. Font step 1. Line-height step 0. Month names are off, so dates are numeric.

| Piece | Size |
| --- | --- |
| Name | 24, **28**, 32, 36, 36 |
| Title | 15, **16**, 18, 20, 20 |
| Contacts | 12, **13**, 13, 13, 14 |
| Photo diameter | 116 at every step |
| Section label | 16, **16**, 20, 20, 20 |
| Job title | 14, **15**, 18, 20, 20 |
| Employer | 13, **14**, 17, 18, 18 |
| Description and bullets | 12, **12**, 13, 14, 15 |
| Dates | 11, **12**, 14, 14, 14 |

Sidebar text on the right is white. The “Powered by” mark stays on the white column.

### 4. Crest

Id `crest`. French: Crête. Badged New.

One column. Photo off. Icons off. Summary is pinned to the top. Skill marks use the lolly indicator. Language slider is off. Icon set, if icons are turned on later, is the outline set.

Colors **#2B1D14**, **#756C64**. Background **b36Cream**. Both families are EB Garamond. Name is not in capitals. Page padding 50. Section gap 18, the loosest step. Font step 2. Line-height step 2.

| Piece | Size |
| --- | --- |
| Name | 40, 48, **52**, 56, 60 |
| Title | 12, 12, **13**, 13, 14 |
| Contacts | 15, 15, **16**, 17, 18 |
| Photo diameter, if enabled | 110, 110, **120**, 130, 130 |
| Section label | 12, 12, **13**, 13, 14 |
| Job title | 17, 18, **18**, 19, 20 |
| Employer, dates, description, bullets | 15, 15, **16**, 17, 18 |

Name line height at 52 px is 65 + 2 = **67 px**, because EB Garamond has a metric for 52. The title is tracked at 0.18 em. The name is tracked at 1 px, weight 300, color #392716. Contacts sit between two hairline rules in #1f1b17 at about 18% opacity. The official preview sets the summary in italic and uses em dashes as bullets.

### 5. Imprint

Id `imprint`. French: Empreinte. Badged New.

One column. Photo off. Icons on, from the outline set. Summary pinned. Skill marks are dashed. Language slider is off.

Colors **#000000**, **#6F7878**. No background. Cormorant Garamond headings, Inter body. Name is not in capitals. Page padding 50. Section gap 14. Font step 2. Line-height step 1.

| Piece | Size |
| --- | --- |
| Name | 40, 48, **52**, 56, 60 |
| Title | 14, 15, **15**, 16, 17 |
| Contacts | 13, 13, **14**, 15, 16 |
| Photo diameter, if enabled | 110, 110, **120**, 130, 140 |
| Section label | 11, 11, **12**, 13, 14 |
| Job title and dates | 17, 18, **20**, 20, 20 |
| Employer, description, bullets | 13, 13, **14**, 15, 16 |

Name line height at 52 px is 65 + 1 = **66 px**. The name is weight 300 and #1d1d1f. The official preview sets the summary in italic, puts the dates on the right of the job title, and separates skills with middle dots.

### 6. Modern

Id `newcondensed`. French: Moderne.

Two columns, right column 40%. Circular photo on the right of the header.

Colors **#343334**, **#00B6CB**. No background. Rubik and Inter. Name in capitals. Icons on. Page padding 50. Section gap 14. Font step 2. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 30, 34, **36**, 38, 40 |
| Title | 15, 16, **18**, 21, 21 |
| Contacts | 13, 13, **13**, 14, 14 |
| Photo diameter | 108, 108, **108**, 108, 116 |
| Section label | 14 at the factory step. The stored list is 14, 14, 14, 14 |
| Job title | 14, 15, **17**, 18, 18 |
| Employer | 13, 14, **15**, 16, 16 |
| Description and bullets | 12, 12, **13**, 14, 15 |
| Dates | 12, 12, **13**, 14, 15 |

### 7. Polished

Id `polished`. French: Raffiné.

Accent sidebar on the left, 290 px. Story on the right. The official preview has no photo. The photo shape, if added, is a rectangle, 116 px.

Colors **#1AB0B3**, **#006666**. No background. Rubik and Inter. Name in capitals. Icons on. Sidebar painted. Page padding 36. Section gap 12. Font step 2. Line-height step 0. Month names off.

| Piece | Size |
| --- | --- |
| Name | 24, 28, **32**, 36, 36 |
| Title | 15, 16, **18**, 20, 20 |
| Contacts | 12, 13, **13**, 13, 14 |
| Photo diameter | 116 at every step |
| Section label | 16, 16, **20**, 20, 20 |
| Job title | 14, 15, **18**, 20, 20 |
| Employer | 13, 14, **17**, 18, 18 |
| Description and bullets | 12, 12, **13**, 14, 15 |
| Dates | 11, 12, **14**, 14, 14 |

Sidebar text is white. “Powered by” sits in the sidebar.

### 8. Contemporary

Id `stockholm`. French: Contemporain.

Narrow column on the left, 266 px. Story on the right. Photo is on, circular, in the left column, over the accent at low opacity. The name is in the right column, not across the page.

Colors **#124F44**, **#3CB371**. No background. Rubik and Inter. Name in capitals. Icons on. Page padding 60, the widest step. Section gap 14. Font step 2. Line-height step 0. Month names off.

| Piece | Size |
| --- | --- |
| Name, in the right column | 32, 40, **48**, 56, 60 |
| Title | 16, 18, **20**, 22, 24. The preview draws it inside a pill. The title is tracked at 2 px. |
| Photo diameter, in the left column | 127, 152, **170**, 190, 200 |
| Left-column contacts | 12, 13, **13**, 14, 15 |
| Section label | 14, 16, **18**, 20, 20 |
| Section icon | 16, 18, **20**, 24, 24, inside a 6 px radius chip filled with the accent at 30% opacity |
| Job title and employer | 14, 15, **16**, 17, 18 |
| Description and bullets | 12, 13, **13**, 14, 15 |
| Dates | 13, 13, **14**, 15, 15 |

### 9. Creative

Id `double_colored`. French: Créatif.

Full-width header band in the accent, then two columns with the right column at 40%. Header text is white. The band is 200 px tall, or 240 px when a photo is shown. The official preview puts a circular photo on the right of the band.

Colors **#235986**, **#14324c**. No background. Rubik and Inter. Name in capitals. Icons on. Page padding 36. Section gap 12. Font step 2. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 30, 34, **38**, 42, 42 |
| Title | 15, 17, **19**, 21, 21 |
| Contacts | 12, 12, **12**, 12, 13 |
| Photo diameter | 110, 125, **125**, 125, 150 |
| Section label | 16, 18, **20**, 22, 24 |
| Job title | 14, 16, **18**, 20, 20 |
| Employer | 13, 13, **14**, 15, 16 |
| Description and bullets | 12, 12, **13**, 14, 15 |
| Date and location | 11, 11, **12**, 12, 13 |

### 10. Timeline

Id `timeline`. French: Chronologique.

One page column. Dates sit in a rail inside each entry, with a vertical rule and a dot. That rail is not a second template column.

Colors **#002B7F**, **#F96B07**. No background. Montserrat and Open Sans. Name in capitals, in the primary. Title in the accent. Icons on. Page padding 36. Section gap 12. Font step 1. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 30, **34**, 38, 42, 42 |
| Title | 15, **17**, 19, 21, 21 |
| Contacts | 12, **12**, 12, 13, 13 |
| Photo diameter | 110, **125**, 125, 150, 150 |
| Section label | 16, **18**, 22, 24, 24 |
| Job title | 14, **15**, 17, 18, 19 |
| Employer | 13, **14**, 15, 16, 17 |
| Description and bullets | 12, **12**, 13, 14, 15 |
| Dates | 13, **13**, 15, 15, 15 |

The official preview has no photo. Skills in that preview are underlined tags. Achievements sit side by side.

### 11. Stylish

Id `flipped_modern`. French: Stylé.

Same type, colors, and entry sizes as Modern. The columns are swapped: the narrow column is on the left and is **276 px**, because the page padding is 50. The story is on the right. The header still spans the page.

Colors **#000000**, **#1E90FF**. No background. Rubik and Inter. Name in capitals. Icons on. Section gap 14. Font step 2. Line-height step 0.

Name **36 px**. Title **18 px**. Photo **108 px** if one is added. The official preview has none. Section label **14 px**. Job title **17 px**, employer **15 px**, description **13 px**, dates **13 px**.

### 12. Single column

Id `single`. French: Une colonne.

One column. Same header size table as Double column, and the same entry sizes. Name is **not** in capitals.

Colors **#19273C**, **#3C6DF0**. No background. Rubik and Inter. Icons on. Page padding 50. Section gap 12. Font step 2. Line-height step 0.

Name **38 px**. Title **19 px**, in the accent. Contacts **12 px**. Photo **135 px** if added. The official preview has none. Section label **20 px**. Job title **17 px**, employer **15 px**, description **13 px**, dates **12 px**.

### 13. Compact

Id `condensed`. French: Compact.

Two columns, right column 40%. This is a dense two-column page, not a single column. Circular photo on the right of the header. Background **b22Colored**. The official preview is pale blue with shapes in the corners.

Colors **#002B7F**, **#56ACF2**. Rubik and Inter. Name is not in capitals. Icons on. Page padding 36. Section gap 12. Font step 2. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 26, 28, **29**, 31, 33 |
| Title | 16, 16, **17**, 18, 21 |
| Contacts | 12, 13, **13**, 13, 13 |
| Photo diameter | 108, 108, **108**, 108, 124 |
| Section label | 11 at every step |
| Job title | 14, 15, **17**, 18, 18 |
| Employer | 13, 14, **14**, 15, 16 |
| Description and bullets | 12, 12, **13**, 14, 15 |
| Date and location | 11, 11, **12**, 12, 13 |

Enhancv’s gallery says this is for up to 10 years. The ATS page says 15 years or more. Both sentences are live. The layout numbers are the same either way.

### 14. Multicolumn

Id `multicolumn`. French: Multicolonne.

Three columns. The middle one is 40% and holds the experience in the official preview. The header spans the page, with a circular photo on the right.

Colors **#000000**, **#1E90FF**. No background. Rubik and Inter. Name in capitals. Icons on. Page padding 36. Section gap 12. Font step 1. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 30, **32**, 34, 36, 42 |
| Title | 15, **16**, 16, 17, 17 |
| Contacts | 12, **12**, 13, 13, 14 |
| Photo diameter | 108 at every step |
| Section label | 14 at every step |
| Job title | 14, **15**, 16, 18, 18 |
| Employer | 13, **13**, 15, 16, 16 |
| Description and bullets | 12, **12**, 13, 14, 15 |
| Dates | 11, **11**, 12, 12, 13 |

### 15. Classic

Id `classic`. French: Classique.

One column. Icons off, including in the header. Language slider off. Company logos are not offered. No border styling.

Colors **#000000**, **#1E90FF**. No background. Rubik and Inter. Name is not in capitals, and the name weight is 400. Page padding 50. Section gap 12. Font step 2. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 24, 28, **34**, 38, 38 |
| Title | 14, 16, **18**, 21, 21 |
| Contacts | 12, 13, **13**, 13, 14 |
| Photo diameter | 90, 90, **90**, 110, 110 |
| Section label | 16 at every step |
| Job title | 14, 15, **18**, 21, 21 |
| Employer | 13, 14, **15**, 17, 17 |
| Description and bullets | 12, 13, **13**, 14, 15 |
| Dates | 11, 11, **12**, 12, 13 |

The official preview has no photo and no icon glyphs. City and dates are right-aligned.

### 16. High Performer

Id `high_performer`. French: Performance.

Two columns, right column 40%. This is the only template with the experience table turned on. The official preview shows a table whose headers are “Project name” and “Description” under each role.

Colors **#343334**, **#00B6CB**. No background. Raleway and Open Sans. Name in capitals. Icons on. Page padding 50. Section gap 12. Font step 1. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 30, **32**, 34, 36, 38 |
| Title | 15, **16**, 17, 18, 18 |
| Contacts | 12, **13**, 13, 13, 14 |
| Photo diameter | 108 at every step |
| Section label | 14 at every step |
| Job title | 14, **15**, 16, 17, 17 |
| Employer | 13, **14**, 14, 15, 15 |
| Description and bullets | 12, **13**, 13, 14, 15 |
| Date and location | 11, **11**, 12, 12, 13 |

The official preview has no photo.

### 17. Minimal

Id `minimal`. French: Minimal.

Two columns, right column 40%. Icons off. Company logos are not offered. No border styling. Circular photo on the right of the header. Section labels are the accent, at 11 px, with no icon and no rule.

Colors **#124F44**, **#3CB371**. No background. Rubik and Inter. Name in capitals. Page padding 36. Section gap 18. Font step 1. Line-height step 0.

| Piece | Size |
| --- | --- |
| Name | 26, **28**, 30, 32, 32 |
| Title | 14, **16**, 17, 18, 18 |
| Contacts | 12, **12**, 12, 12, 14 |
| Photo diameter | 110, **124**, 124, 124, 132 |
| Section label | 11 at every step |
| Job title | 14, **15**, 16, 18, 18 |
| Employer | 13, **14**, 14, 15, 16 |
| Description and bullets | 12, **12**, 13, 14, 15 |
| Date and location | 11, **11**, 12, 12, 13 |

The official preview draws “How I split my time” as a doughnut. That is a section, not part of the column geometry. The doughnut uses the accent greens.

## What is shared, and what is only the sample

A section can be added, removed, or moved. The column count cannot. The sample on the preview image chooses which sections exist and, for skills, whether they are tags, a sentence, or a meter. The factory meter is:

| Template | Skill meter | Language meter |
| --- | --- | --- |
| Crest | Lolly | Off |
| Imprint | Dashed | Off |
| Classic | Default | Off |
| The other 14 | Default | On |

Company logos can be turned on for every template except Classic and Minimal. The gallery cards “with Logos” and “with Photo” are that switch, on the same template.

A cover letter is always one column, even when the resume has two or three.

## Line-height metrics

Look up the pixel size in the font’s row. Add the template’s line-height step. Crest adds 2. Imprint adds 1. The others add 0. A size that is not in the row uses line height 1.

Rubik, used for most headings. Sizes stop at 31, so a 34 px or larger Rubik name uses line height 1.

| px | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 22 | 24 | 28 | 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Rubik | 14 | 15 | 17 | 18 | 19 | 20 | 21 | 23 | 24 | 26 | 28 | 33 | 36 |

Inter, the usual body, and the body of Imprint:

| px | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 20 | 22 | 24 | 28 | 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Inter | 15 | 16 | 17 | 18 | 19 | 21 | 22 | 24 | 27 | 29 | 34 | 36 |

Open Sans, the body of Timeline and High Performer:

| px | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 20 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Open Sans | 16 | 18 | 19 | 20 | 22 | 23 | 25 | 27 |

PT Sans, the Ivy League body:

| px | 12 | 13 | 14 | 15 | 16 | 18 | 20 | 22 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| PT Sans | 15 | 16 | 17 | 18 | 19 | 22 | 24 | 27 |

Volkhov, the Ivy League headings. Montserrat, the Timeline headings. Raleway, the High Performer headings.

| px | 13 | 15 | 16 | 17 | 18 | 20 | 22 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Volkhov | 17 | 19 | 21 | 22 | 23 | 26 | 28 |
| Montserrat | 16 | 18 | 20 | 21 | 22 | 24 | 27 |
| Raleway | 15 | 18 | 19 | 20 | 21 | 23 | 26 |

EB Garamond and Cormorant Garamond, for the large names:

| px | 13 | 15 | 16 | 18 | 20 | 40 | 48 | 52 | 56 | 60 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Either serif | 17 | 19 | 21 | 23 | 26 | 50 | 60 | 65 | 70 | 75 |

Crest’s 52 px name is 65 + 2. Imprint’s 52 px name is 65 + 1. A 13 px Crest section label is 17 + 2. A 12 px Imprint section label is 15 + 1, from the Cormorant row, because the section label uses the heading font.
