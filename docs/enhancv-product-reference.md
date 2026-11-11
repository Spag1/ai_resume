# Enhancv product reference

Observed 11 November 2026. This document combines a logged-out pass through enhancv.com and app.enhancv.com with a signed-in pass on the test account. It is a functional and visual reference for a similar product. It is not an implementation.

## How to read the evidence

| Label | Meaning |
| --- | --- |
| Seen, logged out | Watched on the public site or in the guest app, with no account. |
| Seen, signed in | Watched after login. The account language was French. English names in parentheses are the same control in the English strings. |
| In the product | Present in Enhancv’s shipped interface copy, help articles, or the pricing page structured data. The control was not clicked in either pass. |
| Inferred | Two observed facts joined into a sequence that was not watched as a whole. |

The signed-in display name is Overy. The trial was created 11 November 2026. Billing says it expires in 7 days, on 18 November 2026, and that editing stops when the free plan ends until a paid plan is added. The password was not changed. Checkout was not submitted. No AI rewrite was accepted.

The research left two resumes in Documents: the original nearly empty resume, and a second resume created by uploading a one-page sample PDF.

## 1. Executive summary

Enhancv is a job-search workspace whose center is a resume you edit on the page itself. Around that document it sells a cover letter, a job tracker, a job feed, an ATS-style match against one posting, and an assistant that can rewrite the document in place.

There are two products in one brand.

- enhancv.com is the marketing site: homepage, pricing, a template gallery, a features page, examples, and a blog.
- app.enhancv.com is the application. A guest can walk onboarding and open a preloaded editor. Saving, Fix Mistakes, and download ask for an account. After login the home is a dashboard, not the editor.

The public pricing page shows a 7-day free card at $0 and a Pro Monthly card at $39.00 a month. The signed-in plans page, which was not submitted, defaults to $23.00 a month marked most popular, with the line “$69 billed quarterly.” Account cards say Pro starts at $16.50 a month. Those three numbers are different presentations of term pricing, not three different products seen side by side.

The editor has 17 templates. In the French UI, Ivy League is labeled Harvard. Crest and Imprint are badged New. On the trial, download offers PDF, send the PDF by email, and TXT. A Word button was not on that dialog.

Import does not show a field-by-field review. A PDF dropped into the AI column becomes a new resume already laid out in the template, then a dialog offers to keep the original wording or improve it with AI.

## 2. Logged-out marketing site

Seen, logged out, on 11 November 2026.

### Homepage

URL: https://enhancv.com/

The hero headline is “Land more interviews with Enhancv's Resume Builder.” The subhead names AI Resume Writer, ATS Check, and One-Click Job Tailoring. Primary actions are a green “Build Your Resume” and an outlined “Get Your Resume Score.” A review line sits with the hero. The page then walks a template carousel, editing and download claims, testimonials including video, an ATS section, statistics, an AI section, text improvement, one-click tailoring, resume sections, example resumes, the wider job-search suite, a research or resources block, an FAQ, and a footer.

Header navigation: Resume, Tools, Organizations, Pricing, Sign In, and a green Get Started.

Footer groups cover product, tools, resources, and company, with social links.

### Public pricing

URL: https://enhancv.com/pricing/

Two cards were on screen together.

| Card | Price | What the card lists |
| --- | --- | --- |
| Free plan | $0, valid for 7 days | All resume templates. Basic resume sections. Enhancv branding. Maximum 12 section items. Access to all design tools. Button: Build My Resume. |
| Pro Monthly | $39.00 a month, billed once a month | 300 resumes and cover letters. All resume templates. Real-time content suggestions. ATS check. Pro resume sections. No branding. Unlimited section items. Thousands of design options. Button: Build My Resume. |

The Pro card has tabs labeled Pro Monthly, Pro Quarterly, and Pro Semiannual. Only the monthly tab was read. Payment marks under the cards: Mastercard, Maestro, Visa, American Express, PayPal.

An earlier read of the pricing page structured data listed Pro Quarterly at $69 for the quarter and Pro Semiannual at $99 for six months. That structured data was not re-opened as a rendered tab in this pass. $99 divided by six is $16.50, which matches the “from $16.50” line on the signed-in account cards. $69 divided by three is $23, which matches the signed-in plans default. Treat $39, $69, and $99 as the published US list from that schema, and treat $23 and $16.50 as the per-month readings of the longer terms.

### Template gallery

URL: https://enhancv.com/resume-templates/

The page is a grid of resume thumbnails with a filter bar. Filters described on the page cover industry, experience, style, and format. Clicking a template does not demand an account first. It asks whether the visitor already has a resume, with “Yes, I have a resume” and “No, start from scratch,” and then continues into the app.

Thumbnails on the marketing gallery are sample people in sample layouts. Those names are content, not the 17 editor template names. The 17 names were read inside the signed-in editor and are listed later.

### Features page

URL: https://enhancv.com/features/

Headline: “Enhancv Features: AI-Powered Tools to Get More Interviews.”

The subhead names AI resume tailoring, a 27-point resume checker, ATS-friendly templates, and a job tracker “built for quality applications, not mass applications.”

Sections on the page:

- Instant resume feedback, with a hard-skills overlay and the actions “Get Feedback Now.”
- One-click targeted objectives.
- AI interview help: sample questions, a sample role, an assistant prompt, and “Try AI Interview Help Now.”

### A dead URL

https://enhancv.com/ats-resume-checker/ returned a 404. The error page still offers build, ATS check, examples, and home. The live checker path used elsewhere is under /resources/resume-checker/ and inside the app.

## 3. Logged-out application

### Onboarding

URL pattern: https://app.enhancv.com/onboarding with a hash for the step. A Login button stays in the top right. A back arrow sits on the left. The guide is a portrait of a woman on a soft colored shape, then one question, then one or two actions.

The progress control is four circles.

| Step | What was on screen |
| --- | --- |
| Existing resume | “Do you have an existing resume ready?” with “Yes, I have a resume” and “No, start from scratch.” |
| Role | “Please tell me your position so I can recommend templates.” Placeholder: “e.g. Software Engineer, Marketing Manager...” Next stays inactive until there is text. Skip this step is a link. |
| Goal | “Is your main goal to stand out to recruiters or pass ATS (Applicant Tracking System) filters?” Impress Recruiters is green. Pass ATS is purple. This is onboarding#6, with steps 1 and 2 checked and step 3 current. |
| After Pass ATS | onboarding#7. “Great - and this is the correct approach!” Then: “While Enhancv templates are perfectly readable by ATS systems, more than 92% of the decision making is still in the hands of recruiters.” Source line: “Enhancv recruiter survey Q4 2025.” Next continues. |
| Template | “Please select a template for your resume. You can always change it later.” A note says modern ATS systems read double-column templates and do not care about color, and that recruiters still want a readable one-page resume. Thumbnails are a horizontal carousel of full-page samples. |
| LinkedIn | “Finally, would you like to save time by importing your LinkedIn?” Field placeholder https://linkedin.com/in/... Import stays inactive until there is a value. Skip This Step is a link. |
| Handoff | “I now have enough to show you the first draft of your new resume. Let's take a look!” The screen advances on its own. |

The “Yes, I have a resume” branch was not walked in this pass. The signed-in import, below, is the upload behavior that was watched.

### Guest editor

URL: https://app.enhancv.com/resume/new?preloaded=true

Title pattern: “New Resume (2) | Resume Editor.”

A red line under the logo says “Sign up to save your work.”

Top right: Help, Upload Resume, Login, and a green Sign Up.

Toolbar, left to right: AI Assistant, Fix Mistakes, Check & Tailor, Rearrange, Templates, Design & Font, then undo, redo, and History.

Right rail on the page: an eye (preview), download, a link, and a gold crown. The crown is an upgrade mark. It is not a social share button.

Left column, AI Assistant:

- The same portrait, with the word Empty.
- “Whatever you are in, the page as a whole is still too thin to send.”
- Chips: “Not ready to tailor — help me expand my resume”, “Ask me questions and write it for me”, “Would this get me an interview?”
- A box: “Make changes, edit or ask for anything about your resume”, with a send arrow.

The page is a two-column resume already filled with placeholders, not a blank sheet.

| Region | Placeholder content |
| --- | --- |
| Header | YOUR NAME. “The role you are applying for?” Phone, Email, LinkedIn/Portfolio, Location as blue links. |
| Left | SUMMARY, then several EXPERIENCE entries: Title, Company Name, date period, location, and a bullet “Highlight your accomplishments, using numbers if possible.” |
| Right | KEY ACHIEVEMENTS, SKILLS, EDUCATION, TRAINING / COURSES, LANGUAGES. Languages show a name, a level (Native, Advanced), and a row of blue squares. |

A green plus sits on an experience entry, at the end of the bullet list. That is the add-entry control the help article describes. The purple “Add a new section” buttons appear when a column has no section yet. Both were seen. They are not the same control.

Clicking into a company field shows a green outline. Typing was not completed in the guest session, so it is not confirmed that keystrokes persist without an account.

### Auth walls on the guest editor

| Action | Wall |
| --- | --- |
| Fix Mistakes | Modal titled “Save & Check.” “Already have an account? Log in.” |
| Download | Modal titled “Save & Download.” Same providers. |
| Sign Up | Modal titled “Create free account.” Google, LinkedIn, then “or continue with” and an email field, then Continue. Terms of service and privacy policy under the button. Facebook is not on this card. |
| Login | Modal titled “Welcome back.” Google, Facebook, LinkedIn, then email and password, a show-password eye, Forgot password, and Log in. |

The dedicated page https://app.enhancv.com/login is the same Welcome back card, centered on a pale page, with the Enhancv wordmark above it.

What a guest can do, seen: finish the question flow, pick a template, open the preloaded editor, see every placeholder section, see the AI chips, and open the toolbar labels.

What a guest cannot do, seen: Fix Mistakes, download, and save. Check & Tailor, Rearrange, Templates, and Design & Font were not each forced through a wall in the guest session. On the signed-in account those four open without an extra wall.

## 4. Signed-in application

Login with email and password succeeds and lands on https://app.enhancv.com/ with the title Tableau de bord (Dashboard). The interface of this account is French.

### Global chrome

Top links: Tableau de bord (Dashboard), Documents, Offres d'emploi (Job offers), Emplois enregistrés (Saved jobs), Préparer pour l'entretien (Prepare for interview). Then a green Mettre à niveau (Upgrade) and the account avatar.

Footer: resume examples, upgrade, terms, privacy, blog, log out, and a language control. A reCAPTCHA line sits under the footer.

| Direct URL | Where it actually opens |
| --- | --- |
| / | Dashboard |
| /documents | Documents |
| /job-feed | Job offers |
| /jobs | Redirects to the dashboard |
| /job-applications | Saved jobs / application tracking |
| /interview-help | Interview prep |
| /profile | Account, profile tab |
| /billing | Account, billing tab |
| /autofill | Account, autofill tab |
| /credits | Redirects to profile |
| /plans | Plans and a payment step. Not submitted. |
| /linkedin-resume-import | A parse checklist, then a visible reCAPTCHA. Not finished. |
| /resume/:id | Editor |

### Dashboard

Purpose: a home for the search, not a list-only library.

Regions, top to bottom:

- Nouvelles offres (New jobs). A pale green panel: “Find jobs that match your experience.” The action is Télécharger le CV (Upload your resume). A text link goes to more job offers.
- Postulez aujourd'hui (Apply today). Empty state: “Add your first job.” The card says it is a bit empty and offers Ajouter un emploi (Add a job).
- Documents. A table with Nom (Name), Emploi (Job), Type, Créé le (Created), Dernière modification (Last modified). One row, “Nouveau CV”, type CV, created 11 Nov 2026. Row actions include add and download. Tous les documents (All documents) and Créer (Create) sit above the table.
- Commencer (Get started), a checklist: upload your resume, add a job and get a match score, save 3 jobs you want to apply to.
- A promo for the free Chrome extension, “2 in 1”: save a job without copy-paste, and fill an application without typing. The button is “Get the free 2-in-1 extension.”

### Documents

Title: Mes documents (My documents).

Greeting uses the profile name and the count: “Welcome back, Overy! You have 1 document” before the import, and a second document after it.

Actions and structure:

- Créer un nouveau (Create a new one), a purple button.
- Tabs: Tous les documents (All documents), CV with a count, Lettres de motivation (Cover letters).
- Search. The field placeholder is “Rechercher”. A view toggle switches list and grid.
- Columns: name, job, created, modified.
- On the row: pin, add a tag, add a job, download, and a more menu. The more menu includes Dupliquer (Duplicate), Adapter pour un emploi (Tailor for a job), and Supprimer (Delete). Delete was not confirmed.

The create button is present. The menu it opens was not captured, because the click did not land on the control. The creation path that was watched is the AI-column import, which creates a document by itself.

### Job offers

URL: /job-feed. Title: Offres d'emploi.

A single search, centered. Headline: “Find recent openings that are worth applying to.” The line under it: “No ghost jobs. No ads with 500 applicants. Only real open jobs.”

The box contains a sample query. Under it, ESSAYEZ (TRY) chips:

- “Product designer near New York”
- “Remote product designer with Figma”
- “Business Analyst Manager roles paid around $80k”

A comment button sits at the bottom right. No search was submitted, so result cards, filters, and match scores were not seen on this screen.

### Saved jobs

URL: /job-applications. Title: Candidatures. The page title in the header is Suivi des candidatures (Application tracking).

Chrome: search, Tous les statuts (All statuses), Colonnes (Columns), Voir les statistiques (View statistics), a purple Nouvelle candidature (New application), and a Menu overflow. A small “Saved” check appears in the top bar after an edit.

The status filter that opened has two entries: All statuses, and Inactive over 30 days. The status pill on the empty row was not opened, so the pipeline names Bookmarked, Applied, Interviewing, Negotiating, Accepted, Rejected, No Answer, and Archived stay in the product copy and were not read off this menu.

The column picker is a real control. Each row has a checkbox and a drag handle. “Nouvelle colonne” (New column) is at the top.

| Column | On when the picker was opened |
| --- | --- |
| Poste (Job) | Yes, and the checkbox is locked |
| Entreprise (Company) | Yes, locked |
| Statut (Status) | No |
| Date de sauvegarde (Date saved) | Yes |
| Date de candidature (Date applied) | Yes |
| Type | Yes |
| CV | Yes |
| Lettre de motivation (Cover letter) | Yes |
| Notes | Yes |
| URL | No |
| Tâches (Tasks) | No |
| Lieu (Location) | No |
| Description du poste (Job description) | No |
| Salaire (Salary) | No |
| Contact | No |
| Source | No |

The empty row still shows inline adders: add a job title, add a company, a status pill, add an applied date, a type menu, add a resume, add a cover letter, and “Write a note.” The footer says 0 jobs and links to more jobs.

This is the custom-field surface. It is a column list plus New column, not a separate settings page.

### Interview prep

URL: /interview-help.

Headline, stacked: “Two steps. Three clicks. Ready for the interview.” The promise is a personal prep guide in a few minutes, listing a short company brief, STAR scenarios, talking points, and practice questions. A pill reads “Efficient and kind.”

The only control on the card is step 1, “Select a job,” which is a dropdown whose placeholder is “Select an application.” With zero saved jobs there is nothing to select. The rest of the interview flow was not opened.

### Account

Three tabs in a left card: Votre Profil (Your profile), Facturation (Billing), Remplissage automatique (Autofill). A back link returns to the app.

Profile fields and actions:

- Full name. The value is Overy.
- Email, shown in full, with Changer l'adresse email (Change email address) and Modifier les préférences d'e-mail (Edit email preferences). Neither was submitted.
- Password, masked, with Changer le mot de passe (Change password). Not submitted.
- Language. The closed value is Français. The menu lists English, Français, Deutsch, Español, Svenska, Português, Italiano, Nederlands, Dansk, Suomi, Čeština, Polski, Norsk.
- Modifier les préférences de cookies (Edit cookie preferences).
- Se déconnecter de tous les appareils (Log out of all devices).
- Supprimer le compte (Delete account). Not confirmed.

A side card repeats the Pro upsell: from $16.50 a month, add Pro sections, compact template, unlimited entries, 300 resumes and cover letters, remove branding.

### Billing

“Votre essai gratuit expire dans 7 jours (18e nov. 2026).” The plan name is Essai gratuit (Free trial). “This free account was created on 11 Nov 2026.” The next sentence says that after the free plan expires the resume cannot be edited until a paid plan is added.

Invoice history is a table: Date, Amount, Plan, Payment method, Receipt. The empty line is “Your transaction history will appear here.”

### Plans, signed in

URL: /plans. Title: Enhancv Plans.

The page is a long feature story on the left and a two-step purchase on the right. The story is organized as Week 1 (build a resume), Weeks 2–4 (tailor), Month 2+ (track), Before each interview, and Always. Claims on that page include a 27-point style of ATS check described here as 19 deep checks plus a score, 12 ATS templates, CPRW-reviewed templates, translation into 9 languages, export without the Enhancv mark, up to 300 documents, and support within 24 hours. Those sentences are marketing on the plans page. They are not measurements from this session.

Step 1 is “Choose how often to pay.” The selected row is $23.00 a month, badge “Most popular,” and “$69 billed quarterly.” “See other plans” is a collapsed row. It did not open. Step 2 is “Billing and payment” with a green “Continue to payment.” That button was not pressed. A note says cancel anytime from the profile, in about 30 seconds. Another note says a regular Pro plan may not be used for commercial purposes, and points at Enhancv business plans.

### Autofill

URL: /autofill. This is the store of answers for filling job applications. It is not the resume.

| Group | Questions and choices seen |
| --- | --- |
| US application questions | Authorized to work in the US: Yes, No. Need visa sponsorship: Yes, No. |
| Job preferences | Willing to relocate: Yes, No. Expected salary: a free field. Notice period: Immediately, 1 week, 2 weeks, 1 month, 2 months, 3+ months. Travel: none, up to 25%, 50%, 75%, 100%. |
| Equal employment, optional | Gender: Man, Woman, Non-binary, Prefer not to say. Race or ethnicity: Hispanic or Latino, White, Black or African American, Asian, Prefer not to say. Veteran: Yes, No, Prefer not to say. Disability: Yes, No, Prefer not to say. The intro says refusing a question is allowed. |
| Background | Criminal record: Yes, No. Worked at this company before: Yes, No. |
| Personal overrides | Email, phone, LinkedIn URL. The page says these values replace the resume when a form is filled. |
| Custom questions | “Add a question.” |

No answers were saved.

## 5. Editor

### Signed-in chrome

The empty resume was “Nouveau CV (2)” at /resume/6af4c56ea0e63163c046f001. After import, the new resume is “Nouveau CV (3)” at /resume/6af4c6bea0e63163c04852df.

Title row: a home menu, the document name, and (Enregistré), which is (Saved). Upgrade and the account avatar stay at the right.

Toolbar: Assistant IA (AI Assistant), Corriger les fautes (Fix Mistakes), Vérifier et Adapter (Check & Tailor), Réorganiser (Rearrange), Modèles (Templates), Design & Police (Design & Font), then undo (Annuler), redo (Rétablir), and Historique (History).

Opening a tool replaces the left AI column. The address records it:

| Tool | Query |
| --- | --- |
| Fix Mistakes, and the tailor entry | activeToolboxPanel=RESUME_CHECKER |
| Templates | activeToolboxPanel=TEMPLATES |
| Design & Font | activeToolboxPanel=DESIGN |
| History | A version-history view that covers the editor, not a query-only panel |

Right rail: eye, download, and a link icon once the page has content. A further small icon under the link was visible on the imported resume and was not opened. The guest rail’s gold crown was not repeated as a crown on the signed-in page.

### AI column

When no tool is open, the left column is the assistant.

On the empty signed-in resume the line is “The hardest part is the blank page.” Chips: “Import my old resume,” “Import from LinkedIn,” “Ask me questions and write it for me.” The box says “Edit, touch up, or ask for anything you want on your resume.”

On the guest preloaded resume the line is “Whatever you are in, the page as a whole is still too thin to send,” and the chips are expand, ask-and-write, and “Would this get me an interview?”

On the imported resume the progress label is Commencé (Started), the line is “No matter the section, the whole thing is still too light to send,” and the chips are “What’s missing?”, “Ask me questions and write it for me,” and “Would this get me an interview?”

The chips change with how full the page is. No message was sent, so a live model reply was not watched. No credit counter was on the editor, the dashboard, or billing.

### Fix Mistakes

On the empty resume the left panel is titled Fix Mistakes and carries a badge of 5.

- A meter from F to A. The line above it says to complete the resume to get a grade.
- Spelling and grammar: “No problem detected.”
- Wording and readability: a lock, “Upgrade to Pro to unlock the full report.”
- Recommendations: “No problem detected.”
- Recruiter checks, each waiting for content: Credibility, Interview risks, Age bias, Gaps in the career, Scope and responsibilities, Skill gaps.

### Check & Tailor

The first screen is a modal: “Check and adapt your resume for ATS filtering.” Three steps: paste the job description, Enhancv analyzes the offer and assigns an ATS score, then you get suggestions to improve the match before applying. Continue goes to “Applying for a new job?”

That second screen has one field: “Paste a job URL (https://) or the full job description.” Instructions mention the right-click menu and Ctrl+V. Continue stays disabled until the field has text. Close is the other button. Nothing was pasted, so no score and no rewritten bullets were produced.

### Rearrange

With no sections, a dialog says “You have no sections in your resume.” and “Add your first section!” Buttons: “Continue editing” and “Add a section.” Drag handles and page numbering were not exercised. The product copy for Rearrange includes “Page X of Y.” That page counter was not on screen in this empty state.

### History

“Version history.” A group “Today” with “1 version.” The row is an eye and the timestamp 11 Nov 2026 19:43. A banner across the top says restoring older versions of the resume requires Enhancv Pro, with “See the prices.”

### Add a section

“Add a new section.” Subline: “Click a section to add it to your resume.” Each card is a miniature of sample content, with the section name under it and an add action.

Names seen, in French, with the English equivalent:

| On the card | English |
| --- | --- |
| Éducation | Education |
| Expérience | Experience |
| Résumé | Summary |
| Compétences | Skills |
| Personnalisé | Custom |
| Langues | Languages |
| Formation / Cours | Training / Courses |
| Projets | Projects |
| Réalisations | Key achievements |
| Points forts | Strengths |
| Bénévolat | Volunteering |
| Expertise sectorielle | Industry expertise |
| Passions | Passions |
| Mon quotidien | My day |
| Retrouvez-moi en ligne | Find me online |
| Prix | Awards |
| Références | References |
| Ma philosophie de vie | Life philosophy |
| Publications | Publications |
| Livres | Books |
| Expérience supplémentaire | Additional experience |
| Compétences supplémentaires | Additional skills |
| Publications supplémentaires | Additional publications |
| Signature | Signature |

Custom appears more than once, as several sample cards that share the Personnalisé label. No card was added, so the in-place fields of a newly added section were not watched on this account. The guest preloaded page already shows the field pattern for experience, education, skills, and languages.

### Design & Font

Values read off the open panel for this resume:

| Control | Value on screen | Ends of the slider |
| --- | --- | --- |
| Page margins | 5 | Narrow to wide |
| Section spacing | 3 | Compact to more space |
| Colors | Two rows of round swatches, 12 visible, plus “Use custom colors” | Primary and secondary exist in the product copy. The custom picker was not opened. |
| Font style | Rubik | The menu was not expanded. Other family names were not read here. |
| Font size | Medium | A small A to a large A |
| Line height | 1 | Condensed to spacious |
| Column layout | 2 selected, of 4 thumbnails | 1, 2, 3, 4 |
| Backgrounds | A grid of pattern thumbnails, two rows | A custom background studio exists in the product copy and was not opened. |
| Signature | “Add new” | Show on all pages, last page, or one page exists in the product copy and was not opened. |

### Templates inside the editor

“Choose a template.” The current template has a green check. Under the list: a green “Continue editing,” then “Document size” with A4 selected and US Letter beside it, then “Resume language” set to Français.

All 17 were on screen. Order seen:

| French label | English string | What the thumbnail shows |
| --- | --- | --- |
| Deux colonnes | Double column | Selected. Two columns. This is the layout already on the page. |
| Harvard | Ivy League | French name for the ivyLeague template. Serif, single column. |
| Élégant | Elegant | Dark sidebar and a photo. |
| Crête | Crest | Badged New. |
| Empreinte | Imprint | Badged New. |
| Moderne | Modern | Photo, airy single column. |
| Raffiné | Polished | Teal sidebar. |
| Contemporain | Contemporary | Single column, small photo. |
| Créatif | Creative | Dark header band. |
| Chronologique | Timeline | Dates in a left rail. |
| Stylé | Stylish | Two columns with a photo. |
| Une colonne | Single column | Plain single column. |
| Compact | Compact | Denser single column. |
| Multicolonne | Multicolumn | A narrow skills rail. |
| Classique | Classic | Traditional single column. |
| Performance | High Performer | Single column with accent rules. |
| Minimal | Minimal | Wide margins and a small graphic. |

A second template was not applied. Content surviving a switch is what the template screen itself says (“you can always change it later”) and what the product copy says. It was not re-tested by clicking another thumbnail in this session.

### Download

On the trial, from the rail:

1. A warning band: “Empty fields detected!” and “Consider removing the empty sections or filling them in,” with “Back to editing.”
2. “Download your resume.”
3. “Please select the file format.”
4. File name, filled with “Nouveau CV (2)”, suffix .pdf. Hint: letters, numbers, and spaces are allowed. Special characters are removed automatically.
5. A green “Download as PDF.”
6. “Send the PDF by email.”
7. A text link, “Download as TXT.”

A Word or DOCX button was not on this dialog. The app still contains a “Download as Word (.docx)” string, and the public pricing FAQ has said resumes download as PDF because Word reflows. Those two statements were not resolved by a paid account. On this trial, the dialog is PDF, email PDF, and TXT.

### Autosave and undo

(Saved) stays next to the title across navigation and after import. There is no separate Save button. Undo and redo are toolbar icons. Ctrl+Z was not pressed. History is the long undo, and restoring an older version is behind Pro on this account.

## 6. Import, watched with a known PDF

Entry: the AI chip “Import my old resume” on the signed-in editor. It opens the system file chooser. There is no drop zone and no review table on this path.

The file was a one-page text PDF for a fictional person:

- Alex Test, Product Analyst
- alex.test@example.com, San Francisco, CA
- A one-sentence summary
- Product Analyst at Northwind Labs, January 2022 to March 2024, San Francisco, two bullets
- B.A. Economics, State University, 2018
- Skills: SQL, Experiment design, Stakeholder reporting
- English, Native

Enhancv created a new document, Nouveau CV (3), and left Nouveau CV (2) in place. The title switched to (Saved) with no extra click. The layout is the two-column template. A photo placeholder sits at the top right. Section headings on the imported page stayed in English, matching the file, while the application chrome stayed in French.

| Source field | Where it landed |
| --- | --- |
| Alex Test | Header, as ALEX TEST |
| Product Analyst | Blue headline under the name, and the job title |
| Email | Header, with an @ icon |
| San Francisco, CA | Header, with a pin |
| Northwind Labs, Jan 2022 – Mar 2024, San Francisco | One experience entry |
| Both bullets | The same two sentences, not rewritten |
| B.A. Economics, State University, 2018 | Education, under the job, on the left |
| Summary sentence | A Summary section in the right column |
| Three skills | Separate underlined tags |
| English, Native | A language row with five filled dots |

Immediately after the page appeared, a dialog titled “Content problems detected” said high-impact content was missing and explained that the top of the resume needs a strong summary and the main achievements. Buttons: “Work with the original text” and “Improve with AI.” Improve with AI was not clicked. On a later open the dialog was gone and the parsed text was still on the page.

What this one file does not prove: scanned PDFs, DOCX, multi-column source files, missing headings, or a phone number. Phone and LinkedIn were not in the file and did not appear. The 2 MB limit is verified for the public checker and the cover-letter upload. It was not printed on this editor import.

### LinkedIn

The onboarding step asks for a public profile URL and can be skipped.

The signed-in route /linkedin-resume-import showed four checked steps: analyze the resume, analyze experience, extract skills, generate sections. It then stopped on a checkbox reCAPTCHA, “Please verify that you are not a robot to continue.” The import was not finished. A file export from LinkedIn was not offered on that screen.

## 7. AI, as far as it was opened

| Feature | Where it sits | What was seen | What was not done |
| --- | --- | --- | --- |
| Assistant | Left column, and the AI Assistant toolbar item | Chips that change with an empty page, a thin page, and an imported page. A free-text box and a send button. | No prompt was sent. No diff, accept, or undo of a model edit. |
| Fix Mistakes | Toolbar | Grade meter, spelling, a Pro lock on wording and readability, recommendations, and six recruiter checks that wait for content. | No accepted rewrite. |
| Check & Tailor | Toolbar, then two modals | Paste a URL or a full description. Continue stays disabled until there is text. | No score, no keyword list, no applied edits. |
| Import follow-up | Modal on the new resume | Keep original text, or improve with AI. | Improve with AI was not clicked. |
| Interview | /interview-help | The promise of a company brief, STAR, talking points, and practice questions, blocked on selecting an application. | No report and no mock. |
| Cover letter | Documents tab, and strings for a generator | The tab exists. | The generator was not opened. |
| Credits | Not on the screens that were open | The product copy describes a weekly pool that does not roll over, spent on tailoring, cover letters, ATS checks, assistant edits, and interview reports. | No number was visible, and none was spent on purpose. |

The homepage names several model providers and says suggestions must stay inside the user’s real history. That is Enhancv’s description. This session did not see a model name in the product UI.

## 8. Application chrome versus the resume

These are the app’s own interface tokens, read from the stylesheet served by app.enhancv.com. They are not the colors printed on a resume. Resume color is whatever the user picks in Design & Font.

| Token | Value | Where it shows up |
| --- | --- | --- |
| Brand green | #2dc08d | Primary buttons, logo, the Upgrade button, Import and Continue |
| Brand green, darker | #08936a / #067658 | Hover and brand text |
| Brand tint | #ecfdf5 | Quiet green panels, such as the dashboard job promo |
| Text | #161b1d | Primary text |
| Page | #fafafa / #f3f5f6, shell #fafbfd | Page background |
| Purple | #8271e3 | The Pass ATS choice, Add a section, Create, and several text links |
| Danger | #e71744 | The guest “Sign up to save your work” line |
| Warning | #feb251 | Warning badges |
| Success | #049138 | Success states |

UI headings use Rubik. UI body uses Inter. The resume on the test document also defaults to Rubik, which is a resume setting, not the app font leaking by accident. Spacing steps in the stylesheet run from 2 and 4 through a large scale. Radii include 4, 8, 12, 16, 24, 32, and a full pill.

Resume page, seen: a white sheet on a light canvas, two columns when Double column is selected, blue used for the role line, company, school, and contact icons, black rules under section titles, and a round photo placeholder. Skills are underlined tags. Language level is a row of dots. The trial page text includes a “Powered by” mark.

## 9. Journeys

### First visit, no account

1. Marketing page, or a direct app URL.
2. Onboarding asks about an existing resume, a target role, and recruiters versus ATS.
3. A template carousel, then an optional LinkedIn URL.
4. A preloaded editor opens. The page is already full of placeholders.
5. Fix Mistakes, download, and Sign Up each open an account card. The editor itself stays visible behind the card.

### Return, signed in

1. Login lands on the dashboard.
2. Documents lists every resume and cover letter, with search, pin, tag, duplicate, tailor, and delete.
3. Opening a row goes to /resume/:id. The title already says Saved.
4. Upgrade and the plans page are one click away. Payment is a second step and was not taken.

### Upload

1. From the editor AI column, Import my old resume.
2. The system file chooser. PDF was accepted. DOCX was not tried on this path.
3. A new document appears, already in the two-column template, with (Saved).
4. A content dialog offers the original wording or an AI improvement.
5. The previous document is still in the list.

### Tailor

1. Check & Tailor.
2. A three-step explanation, then one field for a URL or the full posting.
3. Continue stays off until the field has text.
4. The score, the keyword gaps, and the accept-or-reject edits are in the product copy. They were not produced in this session.

### Look, then export

1. Templates: 17 thumbnails, A4 or US Letter, a resume language.
2. Design & Font: margins, section spacing, colors, Rubik, size, line height, four column layouts, backgrounds, signature.
3. Download warns about empty fields, then PDF, email PDF, or TXT on this trial.

## 10. Functional inventory

Priority is for a future lookalike. Essential is required for a credible builder. Advanced is what makes the product feel like Enhancv. Optional is the job-search suite around the document.

| Feature | Where | Behavior | Priority |
| --- | --- | --- | --- |
| Guest onboarding | /onboarding | Four steps: existing file, role, recruiter versus ATS, template, optional LinkedIn. | Essential |
| Guest editor | /resume/new | Preloaded page, tools visible, save and download walled. | Essential |
| Email login | /login | Email, password, Google, Facebook, LinkedIn. | Essential |
| Signup card | Editor and /signup | Google, LinkedIn, email. Facebook is on login. | Essential |
| Dashboard | / | Jobs promo, empty applications, document table, getting-started checklist, extension promo. | Essential |
| Document list | /documents | Tabs, search, list and grid, pin, tag, duplicate, tailor, delete, download. | Essential |
| In-place editor | /resume/:id | The page is the form. (Saved) with no Save button. | Essential |
| Add entry | On a section | Green plus at the end of an entry, seen on the guest page. | Essential |
| Add section | Empty column and a gallery | Purple button, then a card gallery of section types. | Essential |
| Core sections | Editor | Header, summary, experience, education, skills, languages, and the longer catalog. | Essential |
| Templates | Editor drawer | 17 layouts, A4 and US Letter, resume language. | Essential |
| Design | Editor drawer | Margins, spacing, line height, columns, type, colors, backgrounds, signature. | Essential |
| PDF and TXT | Download | Named file, empty-field warning, email the PDF. | Essential |
| File import | AI column | File chooser to a new document. No review grid. | Essential |
| Trial | Billing | 7 days, then editing stops and download remains, per the billing sentence. | Essential |
| Fix Mistakes | Toolbar | Grade, spelling, a Pro-locked wording report, recruiter checks. | Advanced |
| Check & Tailor | Toolbar | One job URL or description, then a score and edits. The score was not produced here. | Advanced |
| Assistant | Left column | Chips plus a free prompt. Structural edits are described in the product copy. | Advanced |
| History | Toolbar | A version list. Restore is Pro on this account. | Advanced |
| Rearrange | Toolbar | Sections across pages. Empty state blocks it until a section exists. | Advanced |
| Cover letter | Documents | A tab and a generator in the product copy. The editor was not opened. | Advanced |
| Share | Right rail | A link icon. The comment flow was not opened. | Advanced |
| Tracker | /job-applications | Spreadsheet, column picker, New column, new application. | Advanced |
| Job feed | /job-feed | One search box and example chips. Results were not loaded. | Optional |
| Interview | /interview-help | Starts from a saved application. | Optional |
| Autofill | /autofill | Stored answers for an extension, including optional EEO questions. | Optional |
| Extension promo | Dashboard | Save a job and fill an application. The extension itself was not installed. | Optional |
| Business plans | Plans page link | A separate product. Not opened. | Optional |

## 11. Sitemap

Marketing: `/`, `/pricing/`, `/resume-templates/`, `/features/`, `/resume-examples/`, `/cover-letter-examples/`, `/resources/resume-checker/`, `/blog/`. The path `/ats-resume-checker/` is a 404.

Application, guest: `/onboarding`, `/onboarding#6`, `/onboarding#7`, `/resume/new?preloaded=true`, `/login`.

Application, signed in: `/`, `/documents`, `/job-feed`, `/job-applications`, `/interview-help`, `/profile`, `/billing`, `/autofill`, `/plans`, `/resume/:id`, `/linkedin-resume-import`.

`/jobs` returns to the dashboard. `/credits` returns to the profile.

## 12. Reproduction blueprint

Build the document first, then the assistant that edits that document, then the job search around it.

### MVP

- Onboarding of one question at a time: existing file or not, target role, a small template choice.
- A guest editor that shows a real page before an account exists, and that asks for an account on save and on download.
- Email login plus one social provider. Keep Facebook on login if the signup card is email-first.
- A dashboard list and a document library with duplicate and delete.
- An editor where the page is the form: header, summary, experience, education, skills, add section, add entry, reorder, autosave, A4 and letter, one accent color, PDF with a real text layer, and an empty-field warning.
- Import that creates a document and lands in the editor, with an explicit choice to keep the original sentences.
- A 7-day trial that watermarks the PDF and caps how many entries can be added. The public free card says 12 items.

### What makes it this product

- An assistant column whose suggestions change as the page fills, and whose edits can be accepted or undone.
- A rule that the assistant does not invent numbers.
- Check & Tailor as one field, a score, and a review of each change.
- The rest of the section catalog, including the personal blocks.
- Seventeen structures, not a thousand unique designs. Role examples are sample content.
- Version history.
- A cover letter that can share a template with the resume.

### Later

Job tracker and the column picker, the job feed, interview prep, translation into a new document, the browser extension and the autofill profile, custom page backgrounds, and a business workspace. Those surfaces are real. They are not required to reproduce the resume.

### Editor rules worth keeping

A section does not split across columns. Headings stay in a predictable vocabulary. Icons do not contain the only copy of a word. Header links are visible. Autosave is quiet and honest when it fails. AI output stays a suggestion until the user accepts it, except where the user has asked the assistant to apply a change. Those two modes should look different. Placeholder numbers must look like placeholders.

## 13. Unknowns

| Topic | Status |
| --- | --- |
| Switching templates after the page has real content | Not clicked. The UI says it can be changed later. |
| The font list beyond Rubik | The closed value is Rubik. The menu was not opened. |
| Ctrl+Z | Undo and redo buttons exist. The keyboard shortcut was not pressed. |
| An ATS score and an accepted AI rewrite | The forms were opened. They were not submitted. No credit number was visible. |
| DOCX download | Not on the trial dialog. The string exists in the app. A paid account was not used. |
| Public quarterly and semiannual prices | Tabs exist. Only the $39 monthly card was read. Structured data previously listed $69 and $99. The signed-in default is $23 a month, $69 billed quarterly. |
| Per-row tracker statuses | The filter showed All and Inactive over 30 days. The row’s status menu was not opened. |
| Cover letter editor | The documents tab exists. The editor was not opened. |
| Job-feed results | The search was not submitted. |
| Multi-page behavior | The imported resume stayed on one page. Rearrange’s page counter was not shown. |
| Drag-and-drop import | This entry point uses the file chooser. A drop zone exists in the product copy for the new-resume modal and was not the path used. |
| LinkedIn import result | Stopped on a reCAPTCHA. |
| 2 MB on the main resume upload | Verified for the public checker and the cover-letter upload. Not printed on the editor import. |
| Business and bootcamp admin | A different product. Out of scope. |

## 14. What this session changed on the account

- Language was left on French.
- Password, email, and plan were not changed.
- Payment was not started.
- A sample PDF created Nouveau CV (3), “Alex Test,” beside the original resume.
- Improve with AI was not run. On a later open, the content-problems dialog was no longer up and the parsed sentences were still the original ones.
