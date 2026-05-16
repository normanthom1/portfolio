JOHANNA ESCUDERO PORTFOLIO SITE — README
=========================================

WHAT'S IN HERE
--------------
A complete, self-contained static website plus a redrafted CV (both .docx and .pdf).
No build tools needed. No server required for local viewing. Just plain HTML, CSS,
and your files.


HOW TO USE LOCALLY
------------------
1. Extract this zip to:    C:\Users\tomrn\Documents\Johanna
   (The folder structure inside the zip will land there directly.)

2. Open the folder and DOUBLE-CLICK on `index.html` to view the site in your
   default browser. That's it. Every page links to the others. The CV download
   button works. The fonts load from Google Fonts so an internet connection
   gives the best result, but everything is still readable offline.

3. To edit any page, open the .html file in any text editor (Notepad++, VS Code,
   even Notepad) and change the text between the tags. Save the file. Refresh
   the browser. Done.


FOLDER STRUCTURE
----------------
Johanna/
├── index.html                  Home page
├── about.html                  About page
├── work.html                   Portfolio index (4 project cards)
├── writing.html                Blog index (3 starter essays)
├── cv.html                     Web-readable CV with PDF download
├── contact.html                Contact info
├── style.css                   All styling (one shared file)
├── build_cv.js                 The Node.js script that built the CV docx
│                               (you don't need to run this — kept for reference)
│
├── work/
│   ├── fluoridation-hia.html
│   ├── smokefree-submission.html
│   ├── regression-analysis.html
│   └── housing-essay.html
│
├── writing/
│   ├── ten-years-dental-assistant.html       (~1,200 word starter essay)
│   ├── wellington-fluoridation-explained.html (~900 word starter essay)
│   └── smokefree-repeal-one-year-on.html      (~1,100 word starter essay)
│
└── assets/
    ├── Johanna_Escudero_CV.docx               <-- The redrafted CV (editable)
    ├── Johanna_Escudero_CV.pdf                <-- The redrafted CV (sharable)
    ├── Fluoridation_HIA_original.pdf/.docx    <-- Original assignment files
    ├── Housing_Essay_original.pdf/.docx
    ├── Regression_Analysis_original.pdf/.docx
    └── Smokefree_Submission_original.pdf/.docx


THINGS TO FIX BEFORE PUBLISHING
-------------------------------
Open the relevant HTML file in a text editor, use Ctrl+F to find the text below,
and replace it.

1. LINKEDIN URL (contact.html, line ~36)
   Currently:  <a href="#" target="_blank" ...>linkedin.com/in/johannaescudero</a>
   Replace the "#" with your actual LinkedIn profile URL.

2. ORIGINAL ASSIGNMENT PDFs HAVE TYPOS
   The original assignment files in /assets/ are unedited from what you
   submitted. Before publishing this site publicly, you'll want to fix:

   - In the Fluoridation HIA: multiple instances of "Pacifika" should be
     "Pasifika" (with an 's'); several Māori words are missing macrons or are
     misspelled ("Witangi"/"Waintanga" should be "Waitangi"; "Maori" should be
     "Māori"; "Aotearoa Tobacco Control Research Network" is a fictional body
     used in the assignment).

   - In the Smokefree submission: "Aotearoa Tobacco Control Research Network"
     is a fictional research network framing used to satisfy the assignment
     brief. The site's project page honestly discloses this in the academic-
     context notice box. You may want to either (a) keep that disclosure or
     (b) rewrite the submission's framing to remove the fictional body before
     making it downloadable.

   These typos and framings do not appear anywhere in the HTML pages I wrote —
   I made sure all references in the website use correct spellings. The issue
   is only in the original PDFs you're linking to as downloads.

3. BLOG POSTS ARE STARTER DRAFTS
   The three blog posts in /writing/ are first drafts I wrote in your
   analytical voice based on your existing assignments and our earlier
   conversation. Before publishing them under your name, read them carefully,
   edit anything that doesn't sound like you, and verify any specific
   statistics against current sources. They're written to be a useful
   starting point, not a finished product.

4. "COMING NEXT" / "COMING SOON" SECTIONS
   The work page mentions an "Oral health affordability piece coming next" and
   the writing page mentions several "Coming soon" topics. These are
   aspirational and you should remove or update them if they don't match what
   you actually plan to publish.

5. THE YEAR
   Pages say "© Johanna Escudero Pino, 2026". Update if needed.


HOW TO PUT IT ONLINE LATER
--------------------------
When you're ready to publish, three easy options (in order of simplicity):

  OPTION A — CLOUDFLARE PAGES (free, easiest, custom domain supported)
    1. Sign up at pages.cloudflare.com (free).
    2. Create a new project, choose "Direct Upload".
    3. Drag the entire Johanna folder onto the page. Done.
    4. You'll get a URL like johanna-portfolio.pages.dev within seconds.
    5. Buy a domain (~$15/year) and point it at the Cloudflare project.

  OPTION B — NETLIFY DROP (free, also very easy)
    1. Go to app.netlify.com/drop
    2. Drag the entire Johanna folder onto the page. Done.
    3. You'll get a URL like cosmic-llama-12345.netlify.app immediately.
    4. You can buy a domain through Netlify or point your own at it.

  OPTION C — SQUARESPACE (paid, no-code, easier to update via web interface)
    Not really an option for THIS site (which is hand-coded HTML) — but if
    you'd rather not touch HTML at all going forward, you could rebuild the
    same structure inside Squarespace (~NZ$25/month). The pages, content, and
    project descriptions in this build give you a complete spec to work from.


DESIGN NOTES
------------
Fonts: Fraunces (serif headings) + Public Sans (body text). Both free, both
loaded from Google Fonts. If you ever want to change them, edit the @import
line at the top of style.css.

Colours: deep teal, warm cream, and terracotta. All defined as CSS variables
at the top of style.css (--ink, --bg, --accent, etc.) so you can change them
in one place and the whole site updates.

The design is intentionally restrained — closer to a Helen Clark Foundation
brief or an Allen + Clarke deliverable than a creative portfolio. That choice
is in service of analyst credibility, not a personal style preference. You
can push it warmer or more personal if you'd like; the bones are good either way.


QUESTIONS
---------
If anything breaks or you want to make a change you can't figure out, ask
Tom for help — he knows where this came from and can help you edit safely.

Welcome to having a portfolio.
