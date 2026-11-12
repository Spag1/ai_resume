# Enhancv resume templates

Checked against the live site and the live editor on 11 November 2026.

The editor contains **17 templates**. The public gallery at [enhancv.com/resume-templates/](https://enhancv.com/resume-templates/) shows **23 cards**. Sixteen of the seventeen editor templates have their own card there. Multicolumn is described on [the ATS templates page](https://enhancv.com/resume-templates/ats/) and is absent from that gallery of 23. The other seven cards are the same template with a photo, company logos, or a projects section turned on. They are not extra layouts.

Three sources are kept separate below.

- **Enhancv’s sentence** is copy fetched from the live page that day. It is quoted.
- **The picture** is the preview file the editor itself ships, at `https://app.enhancv.com/images/…`. That is the picture in the template picker.
- **The layout rule** is the column, color, font, and spacing default in the editor bundle that was live that day. Column count does not change when the user picks another column-width thumbnail. Width does.

A4 and US Letter are not part of a template. They sit under the picker. The signed-in session had A4 selected.

The numbers required to rebuild a template — page size, the factory color pair, font families, name and section sizes, column widths, and line height — are in [enhancv-template-reproduction.md](enhancv-template-reproduction.md).

## How a template is built

The editor assigns a column count from the template id:

| Columns | Templates |
| --- | --- |
| 1 | Ivy League, Crest, Imprint, Timeline, Single column, Classic |
| 2 | Double column, Elegant, Modern, Polished, Contemporary, Creative, Stylish, Compact, High Performer, Minimal |
| 3 | Multicolumn |

The default width is the second of four column thumbnails (`columnLayoutOption` 1, shown in the design panel as 2 of 4).

For Double column, Modern, Creative, Compact, High Performer, and Minimal, that default is a left column plus a right column at **40%** of the grid (`1fr 40%`). The four width steps for this group are 36%, 40%, 44%, and 48% on the right column.

Multicolumn uses the same steps on the **middle** column: `1fr 40% 1fr` at the default.

Elegant, Polished, Stylish, and Contemporary use a fixed sidebar. Its width is `326 − adjustment − page padding` pixels. The default adjustment is 0. The four steps are +10, 0, −10, and −20 pixels, so the sidebar grows as the user moves to a later thumbnail. Page padding comes from the template’s margin step: 28, 36, 44, 50, or 60 pixels.

| Template | Sidebar | Default sidebar width |
| --- | --- | --- |
| Elegant | Right | 290px (page padding 36) |
| Polished | Left. The main column is moved to the right. | 290px (page padding 36) |
| Stylish | Left. The main column is moved to the right. | 276px (page padding 50) |
| Contemporary | Left. The main column is moved to the right. | 266px (page padding 60) |

Elegant adds 22px of padding on the left edge of the sidebar. Polished adds 22px of padding on the right edge of the sidebar.

Section spacing and page padding are indexed the same way for every template:

| Step | Page padding | Space under a section |
| --- | --- | --- |
| 0 | 28px | 8px |
| 1 | 36px | 12px |
| 2 | 44px | 14px |
| 3 | 50px | 16px |
| 4 | 60px | 18px |

The stored color pair is the factory pair. The gallery recolors the same template, so a rust sidebar or a pink header on the marketing site is a color variant, not a different template. Background `b00` means no background image.

The sample section order on a preview is the sample resume. Sections can be added, removed, and moved. The column count cannot.

The picker shows Crest and Imprint with a New badge. In French, Ivy League is labeled Harvard. The other French labels are the translations of the English names.

Enhancv’s FAQ on the gallery names Double Column, Modern, and Creative as the templates people use most, and names Modern as the default recommendation, including a “My Time” section when the user wants it.

## The 17 editor templates

### 1. Double column

French: Deux colonnes. Internal id: `double`.

Enhancv, on the gallery: “This timeless template features a clear, compact layout. Your highlights are balanced with your career story. Ideal for consulting, project management, and executive roles that value clarity, impact, and leadership.”

The gallery’s own alt text calls the first sample “a two-column resume with a blue accent color and focus on experience and achievements.” Two further samples recolor that accent brown and green.

Picture: [layoutDouble](https://app.enhancv.com/images/layoutDouble-b220e1d3109de8a1737b.png). The sample is Ethan Smith. The header spans the page: name, a blue title line, then phone, email, LinkedIn, and city with small icons. There is no photo on this preview. A rule separates the header from the columns. Section names are uppercase with a rule under them. The left column holds Summary, Experience, and Languages. The right column holds Key achievements, Skills, Education, Training / Courses, and Interests. Experience puts the job title on its own line, the employer in the accent color, and the dates and city on the next line with icons. Languages are a name, a level word, and a row of squares. The footer is www.enhancv.com on the left and “Powered by Enhancv” on the right.

Factory defaults: two colors `#000000` and `#1E90FF`. Body Inter, headings Rubik. Name in capitals. Icons on. Page padding 50px. Section spacing 8px, the tightest step. No background image.

### 2. Ivy League

French: Harvard. Internal id: `ivyleague`.

Enhancv, on the gallery: “The classic, sleek design favored by recruiters. Ideal for serious professionals who want to put their experience front and center. Suitable for academic CVs and Ivy League-style resumes, too.”

On the ATS page, Enhancv calls it “a modernized Harvard template.” A Workday article on the same site calls it “a single-column, no-frills layout modeled on traditional academic and consulting resume formats.”

Picture: [ivyleagueResume](https://app.enhancv.com/images/ivyleagueResume-19a6bc72d6acd8c9327d.png). The sample is Abigail Hall. One column. The name, title, and contact line are centered. Contacts are separated by dots. Section names are centered title case, with a rule above and below. Job, school, and dates sit on one row: the organization and title on the left, the city and dates on the right. Key achievements is three equal text columns inside that single page column. Skills is one line with middle dots. The official preview has no photo.

Factory defaults: `#000000` and `#6F7878`. Body PT Sans, headings Volkhov. Section names are not forced to capitals, unlike the other sixteen. Name in capitals. Photo shape, if a photo is turned on, is a circle. Page padding 50px. Section spacing 12px. No background image. The right-side background flag is set in the template record, but the column count is 1, so there is no second column to paint.

The gallery also sells “Ivy League with Photo” and “Ivy League with Logos.” Both use `template-ivy-league`.

### 3. Elegant

French: Élégant. Internal id: `elegant`.

Enhancv, on the gallery: “Your achievements and highlights stand out on the right, while your career narrative leads the story. Best for professionals in consulting, communications, client-facing, or project management roles.”

The gallery alt text says the same thing in layout terms: a wider column for experience and a narrower colored column for highlights.

Picture: [layoutElegant](https://app.enhancv.com/images/layoutElegant-303644c7a3563fa95067.png). The sample is Aiden Williams. White left column, dark sidebar on the right. The sidebar starts with a circular photo, then Key achievements (each with an icon), Skills as a short paragraph, Courses, Passions, and Languages with dot meters. The left column is the name, a colored title, icon contacts, Summary, Experience, Education, and Languages does not repeat there. Experience dates sit on the right of the job title. The employer is in the accent color. The “Powered by” mark sits on the white side. The site link sits at the right of the white column, short of the sidebar.

Factory defaults: `#008CFF` and `#22405C`. Body Inter, headings Rubik. Name in capitals. Round photo. Icons on. The sidebar is painted (`showRightSideBackground`). Page padding 36px, which is what produces the 290px sidebar. Section spacing 14px. Dates use numbers rather than month names (`isMonthName` is off). No background image. Company logos can be turned on. The gallery’s “Elegant with Logos” card is that option, still `template-elegant`.

### 4. Crest

French: Crête. Internal id: `crest`. Badged New in the editor.

Enhancv, on the gallery: “A refined, traditional layout with a distinguished, executive feel. Ideal for senior professionals and leadership roles in law, finance, consulting, and other established fields.”

A Workday article describes one Crest example as a two-page resume with a creamy background, a custom font, and subtle icons. Two pages is that example’s length. The template itself is one column and does not force a second page.

Picture: [crest](https://app.enhancv.com/images/crest-7e6817f35cdd13658721.webp). The sample is Samuel Moore. One column on a cream page. The name is a large serif, not in capitals. The target title is small, widely tracked, and in capitals. A hairline rule, then a centered contact line with middle dots, then another hairline. The summary is italic and centered. Section labels are small and tracked. A job title and its dates share a row. The employer and city sit underneath. Bullets are em dashes. There is no photo.

Factory defaults: `#2B1D14` and `#756C64`. Body and headings are both EB Garamond. Name is not in capitals. Photo is off, and the shape used if it is turned on is a circle. Icons are off. The icon set, if turned on, is `enhancv-outline`. Skill marks use the “lolly” indicator. The summary is pinned. Line-height step 2 of the three-step control, the highest. Page padding 50px. Section spacing 18px, the loosest step. Background `b36Cream`. Body text color `#1f1b17`.

“Crest with Projects” on the gallery is the same template with a projects section. Enhancv describes it for students, recent graduates, self-employed people, and outsourcing work.

### 5. Imprint

French: Empreinte. Internal id: `imprint`. Badged New in the editor.

Enhancv, on the gallery: “Inspired by classic single-column resume templates, Imprint helps you land jobs in traditional corporations, finance institutions and law firms, and just as well in the start-up and tech niche, too, if you turn on the creative twist.”

Picture: [layoutImprint](https://app.enhancv.com/images/layoutImprint-efeaf54a3a4b56c5721c.webp). The sample is Daniel Anderson. One column, white page, no photo. The name is a large serif. The title and the contact line are smaller, with middle dots between contacts. The summary is italic. Section labels are small capitals. Dates sit on the right of the job title. The employer and city are on the next line, joined by an em dash. Bullets are round. Key achievements uses a small line icon beside each title. Skills is one running line separated by middle dots.

Factory defaults: `#000000` and `#6F7878`. Body Inter, headings Cormorant Garamond. Name is not in capitals. Photo off. Round photo if it is turned on. Icons on, from the outline set. Skill marks are dashed. The summary is pinned. Line-height step 1. Page padding 50px. Section spacing 14px. No background image.

### 6. Modern

French: Moderne. Internal id: `newcondensed`.

Enhancv, on the gallery: “A go-to template for upper management, project managers, and product owners. It emphasizes your strengths and measurable achievements without overwhelming the reader.”

The gallery alt text calls the samples two-column, one of them with a photo in the header. The FAQ calls Modern the template to pick when the choice is unclear.

Picture: [layoutNewcondensed](https://app.enhancv.com/images/layoutNewcondensed-9136b5d635d4b4777842.png). The sample is Ellen Johnson. Header across the page: name, a cyan title, icon contacts, and a circular photo at the right. Two columns under a rule. Left: Experience, Education, Languages. Right: Summary, Key achievements with icons inside pale circles, Skills as underlined tags in a grid, Certification. A job line is title, then employer in the accent color, then a calendar icon, dates, a pin, and the city on the same line. Languages use dot meters.

Factory defaults: `#343334` and `#00B6CB`. Body Inter, headings Rubik. Name in capitals. Icons on. Page padding 50px. Section spacing 14px. No background image.

### 7. Polished

French: Raffiné. Internal id: `polished`.

Enhancv, on the gallery: “Structured to lead with measurable results. Ideal for sales leaders, business development managers, and other customer-facing professionals who sell on outcomes.”

The gallery alt text places the highlight column on the **left**, and shows it recolored rust and navy. The editor default is teal.

Picture: [layoutPolished](https://app.enhancv.com/images/layoutPolished-00b4295becfa23bdd555.png). The sample is Jason Reed. A dark teal sidebar on the left holds the name, Key achievements with icons, Certification, Passions, a favorite quote, and Languages with dot meters. The official preview has no photo in that sidebar. The right column is white: a colored title, icon contacts, Summary, Experience, Skills as a dotted line, and Education. Dates and cities sit on the right of each role. “Powered by” is inside the sidebar. The site link is on the white side.

Factory defaults: `#1AB0B3` and `#006666`. Body Inter, headings Rubik. Name in capitals. Photo shape is a rectangle if a photo is added. Icons on. Sidebar painted. Page padding 36px, so the left sidebar is 290px. Section spacing 12px. Month names off. No background image. The main column is drawn on the right of the sidebar.

### 8. Contemporary

French: Contemporain. Internal id: `stockholm`.

Enhancv, on the gallery: “This modern template combines a bold layout with a clean, professional flow. Ideal for dynamic roles or industries that value innovation and momentum, such as startups or forward-thinking leadership positions.”

The ATS page calls it “our most modern template.” A Workday example is tagged “double-column, icons, accent color.” The gallery alt text for the one sample is “a contemporary entry-level marketer resume template with green accent colors and a photo.”

Picture: [layoutContemporary](https://app.enhancv.com/images/layoutContemporary-5df8b7a6b8680b357c6b.png). The sample is Aiden Williams. The left rail holds a circular photo over pale green shapes, then Contacts, Key achievements, Skills, and Certification. Section labels in that rail have icons. The right side leads with the name stacked on two lines and the title inside a green pill. Summary, Experience, and Education follow, and those headings have icons too. A role is employer, then job title, with the city and dates on the right. Skills in the rail is a dotted list.

Factory defaults: `#124F44` and `#3CB371`. Body Inter, headings Rubik. Name in capitals. Photo on, circular. Icons on. Page padding 60px, the widest step, which makes the left rail 266px. Section spacing 14px. Month names off. No background image. The header height record is 0.

### 9. Creative

French: Créatif. Internal id: `double_colored`.

Enhancv, on the gallery: “This template draws attention to your header and invites recruiters to read more. Fit for design, marketing, and other creative fields—while remaining versatile across industries.”

The gallery samples recolor that header purple and pink and include a photo. The editor default is navy.

Picture: [layoutDoubleColored](https://app.enhancv.com/images/layoutDoubleColored-3831ccff493a154ede68.png). The sample is Brandon Hale. A full-width dark header carries the name and title in white, white icon contacts, and a circular photo on the right. Below it, two columns. Left: Experience, Education, Skills as underlined tags. Right: Summary, Key achievements with icons, Courses, Passions. Section names are uppercase with a colored rule. Job dates and city sit under the title, with icons.

Factory defaults: `#235986` and `#14324c`. Body Inter, headings Rubik. Name in capitals. Icons on. `coloredHeader` is on. The header band is 200px tall, or 240px when a photo is shown. Page padding 36px. Section spacing 12px. No background image. The columns are the ordinary 40% split, not the fixed sidebar used by Elegant.

### 10. Timeline

French: Chronologique. Internal id: `timeline`.

Enhancv, on the gallery: “Built on the classic reverse-chronological format, this template uses a timeline to show your career path clearly. Ideal for experienced professionals or those who want to emphasize progression.”

The ATS page adds that it suits operations, business, and logistics, and that it is meant for entry through senior level. The gallery alt text calls it a single-column timeline. “Timeline with Logos” is the same template.

Picture: [layoutTimeline](https://app.enhancv.com/images/layoutTimeline-1f35864e8d43109ab932.png). The sample is Grace Jackson. The header is full width: a large colored name, an orange title, and icon contacts spread across the line. Summary is a normal paragraph. Experience is the timeline: the date and city sit in a left rail, a vertical rule with a dot marks each entry, and the title, colored employer, and bullets sit to the right of the rule. Education uses the same rail. Skills are underlined tags. Key achievements is two items side by side, each with an icon. The page is still one layout column. The rail is part of the entry, not a second template column.

Factory defaults: `#002B7F` and `#F96B07`. Body Open Sans, headings Montserrat. Name in capitals. Icons on. `isTimeline` is on. Page padding 36px. Section spacing 12px. Font-size step 1. No background image.

### 11. Stylish

French: Stylé. Internal id: `flipped_modern`.

Enhancv, on the gallery: “A clean, recruiter-friendly layout that reads well across industries. Built to keep your experience clear and easy to scan, whatever field you're in.”

The ATS page says it is designed to turn a two- or three-page resume into one page. One gallery alt text calls a sample a double-column resume. Another sample is an artist resume. Those are the same template.

Picture: [layoutFlippedModern](https://app.enhancv.com/images/layoutFlippedModern-123051a78b4317742fa5.png). The sample is Violet Rodriguez. The header spans the page: name, title, and a long icon contact line that includes GitHub. There is no photo on this preview. Under it, the narrow column is on the left and holds Skills as a three-across grid of underlined tags, My projects, and Key achievements with icons. The wide column on the right holds Summary, Experience, and Education. Employer names are in the accent color. Dates and city sit on the job line with icons.

Factory defaults: `#000000` and `#1E90FF`. Body Inter, headings Rubik. Name in capitals. Icons on. Page padding 50px, so the left rail is 276px. Section spacing 14px. No background image. The main column is placed on the right.

### 12. Single column

French: Une colonne. Internal id: `single`.

Enhancv, on the gallery: “A classic single-column format designed for experienced professionals and optimized for recruiters and applicant tracking systems. It also works well for students and entry-level applicants, helping resumes feel more substantial even with limited experience.”

The ATS page says the headings are highlighted so a recruiter can scan the application. “Single Column with Photo” is the same template.

Picture: [layoutSingle](https://app.enhancv.com/images/layoutSingle-7fd107802c252553ad75.png). The sample is Mason Turner. One column. The name is not in capitals. The title is blue. Contacts use icons and wrap under the title. Each section name is uppercase with a heavy rule beneath it. Jobs are separated by a dotted rule. The employer is in the accent color. Dates and city sit on their own line with icons. Key achievements is two items side by side. No photo on this preview.

Factory defaults: `#19273C` and `#3C6DF0`. Body Inter, headings Rubik. Name is not in capitals. Icons on. Page padding 50px. Section spacing 12px. No background image.

### 13. Compact

French: Compact. Internal id: `condensed`.

Enhancv’s two live pages do not agree about who it is for.

- Gallery: “A one-page template designed for mid-level professionals with up to 10 years of experience. Perfect when you want to include most of your career history, while keeping it concise.”
- ATS page: “Maximizes space to fit more than 90% template… If you have 15 years of experience or more and have had many different roles, this is a perfect fit for you.”

Both sentences are on Enhancv.com. They were not edited into one claim. “One-page” and “more than 90%” describe density. The layout is two columns, not one.

Picture: [layoutCondensed](https://app.enhancv.com/images/layoutCondensed-9188d456eaef6a8d04fe.png). The sample is Isabella Adams. A pale blue decorative background frames the page. The header has the name, a light-blue title, icon contacts, and a circular photo at the right. The left column is dense: Experience, Education, Skills as underlined tags, Languages as horizontal bars. The right column is Summary, Key achievements, Courses, and Passions. A role is title, then employer, then dates and city on the same line, without a separate icon row. Section labels are small.

Factory defaults: `#002B7F` and `#56ACF2`. Body Inter, headings Rubik. Name is not in capitals. Icons on. Page padding 36px. Section spacing 12px. Background `b22Colored`, which is a colored background rather than `b00`.

### 14. Multicolumn

French: Multicolonne. Internal id: `multicolumn`.

This is the editor template that the gallery of 23 does not list as its own card. Enhancv, on the ATS page: “The ATS-friendly multicolumn template is perfect for candidates with extensive experience who want to put more on their resume and still fit into one page. It's also a good choice for the ones who would like to present their information more uniquely.”

Picture: [layoutMulticolumn](https://app.enhancv.com/images/layoutMulticolumn-21d802646e3d10341f41.png). The sample is Luke Adams. The header spans the page: name, blue title, icon contacts, circular photo at the right. Three columns. Left: Summary, Key achievements with icons, Passions. Center: Experience only. Right: Education, Skills as underlined tags, Courses, Languages with dot meters. The center column is the 40% middle. The two side columns share the rest.

Factory defaults: `#000000` and `#1E90FF`. Body Inter, headings Rubik. Name in capitals. Icons on. Page padding 36px. Section spacing 12px. Font-size step 1. No background image.

### 15. Classic

French: Classique. Internal id: `classic`.

Enhancv, on the gallery: “As the name suggests, this classic resume template is a safe choice for conservative industries like law, finance, or government, while remaining versatile for most roles.”

The ATS page calls it “a traditional resume with a modern touch.” Gallery alt text: a single-column template focused on experience and side projects. A Workday example is tagged single column with accent colors.

Picture: [layoutClassic](https://app.enhancv.com/images/layoutClassic-ce514599bb366b7c6f05.png). The sample is Scarlett Anderson. One column, no icons, no photo. The name is not in capitals. Contacts are a plain line under the title, with no icon glyphs. Section names are small capitals. The employer is in the accent color. City and dates are right-aligned on their own two lines. Key achievements is set as two pairs across the page. There is no language meter on this preview, and the template turns the language slider off.

Factory defaults: `#000000` and `#1E90FF`. Body Inter, headings Rubik. Name is not in capitals. Icons off, including header icons. Border styling off. Company logos are not offered. Language slider off. `isClassicStyle` is on. Page padding 50px. Section spacing 12px. No background image.

### 16. High Performer

French: Performance. Internal id: `high_performer`.

Enhancv, on the gallery and again on the ATS page: “A data-driven resume template, perfect for project and product managers, or anyone who wants to display achievements through visual elements, like tables. Fully ATS-compatible.”

The gallery samples are described as gray and purple. Those are recolors. The editor default is charcoal and cyan.

Picture: [highPerformer](https://app.enhancv.com/images/highPerformer-b94261b59e773579da81.png). The sample is Isaac Hall. Header across the page, no photo on this preview: name, cyan title, icon contacts. Two columns. Left: Experience and Skills. Right: Summary, Key achievements with icons in circles, Education, Courses. Inside Experience, under the bullets, a real table appears with the headers “Project name” and “Description.” That table is the `showTable` flag, and the editor only offers that option on this template. Skills are underlined tags.

Factory defaults: `#343334` and `#00B6CB`. Body Open Sans, headings Raleway. Name in capitals. Icons on. Page padding 50px. Section spacing 12px. Font-size step 1. No background image. Columns are the ordinary 40% split.

### 17. Minimal

French: Minimal. Internal id: `minimal`.

Enhancv, on the gallery and the ATS page: “For those who want to blend whitespace and content, without clutter.”

A Workday example is tagged double columns, accent colors, a background, and icons. Icons are off in the factory default. That example was customized. The official preview is the factory look.

Picture: [layoutMinimal](https://app.enhancv.com/images/layoutMinimal-8b66db23b68bd5aacad8.png). The sample is Elise Carter. Two columns with more air than Compact. The header is the name, a plain title, icon-free contacts, and a circular photo at the right. Section labels are green and small, not underlined bars. Left: Summary, Experience, Education. A role keeps the title, then the employer, dates, and city on one line, then a short paragraph, then bullets. Right: Strengths, Skills as a dotted list, Projects, and “How I split my time,” drawn as a green doughnut with a lettered legend. No icon set is drawn on the section labels.

Factory defaults: `#124F44` and `#3CB371`. Body Inter, headings Rubik. Name in capitals. Icons off. Company logos are not offered. Border styling off. Page padding 36px. Section spacing 18px, the same loose step as Crest. Font-size step 1. No background image. Columns are the ordinary 40% split.

## Gallery cards that are not new templates

Fetched from the same gallery JSON. The `templateName` is the editor template.

| Gallery card | Same template as | What Enhancv changes |
| --- | --- | --- |
| Ivy League with Photo | Ivy League | A photo is added. |
| Ivy League with Logos | Ivy League | Company logos are added. Enhancv calls this “a 21st-century update to the classic Harvard template.” |
| Single Column with Photo | Single column | “A profile photo at the top.” |
| Elegant with Logos | Elegant | Company logos in the same two-column layout. |
| Double Column with Logos | Double column | “Enhancv's most popular layout adds company logos.” |
| Timeline with Logos | Timeline | The timeline plus company logos. |
| Crest with Projects | Crest | A projects section, described for students, graduates, self-employed people, and outsourcing. |

Classic and Minimal do not offer company logos. The logo cards above are the templates that do.

## Cover-letter thumbnails

The resume picker and the cover-letter picker are not the same list. These resume templates ship a separate cover-letter picture: Ivy League, Modern, Timeline, Single column, Compact, Multicolumn, Classic, and High Performer. Minimal reuses the Modern cover-letter picture. The others use the resume picture when a cover letter is chosen, or have no separate file. A cover letter is always one column, even when the resume template has two or three.

## What was not done

No second template was applied to the signed-in test resume. The pictures and the layout rules above are the editor’s own files, not a re-render of that account. Switching templates is what the picker promises (“you can always change it later”). That click was not repeated for all 17.

The four column-width thumbnails were not each applied. The widths in the table are the four values the bundle stores, and the default is the second one.
