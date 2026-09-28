# CS239 · Fall 2026

Static course webpage for **CS239: Topics in Computer Science: Large Language
Models for Code Intelligence**. There is no build step or JavaScript dependency.

## Editing the course

- Edit `index.html` to replace the bracketed placeholders. The staff, logistics,
  content, coursework, schedule, and resources sections have matching HTML IDs.
- Update the short “Additional course details to be announced” message below the title when
  the content is ready.
- The sole instructor's portrait uses `../../assets/profile_full.jpg`. Replace
  `[Instructor name]` and update the image's `alt` text when adding the name.
- Lectures are Mondays and Wednesdays, 4:00–5:50 p.m., in GEOLOGY 6704. Office
  hours are Thursdays, 4:00–5:00 p.m., in Engineering VI, in front of Office 295.
- The schedule lists 19 lecture meetings from September 28 through December 2,
  2026, with a deadline-only row for October 9 and a “No class” row for November 11.
  Topics, subtopics, and the
  40 paper links follow `../../Reading_List_CS239_LLM4CodeIntell.xlsx`, including
  topic groups that span dates in the spreadsheet's merged cells. The schedule
  is static HTML; update `index.html` when the reading list changes.
- Each lecture uses a `tbody.lecture-group`. Each subtopic and its matching
  papers share a row, with a light border between subtopics and no bullets.
  The date and due cells use `rowspan` to cover the group's
  rows; update those spans if you add or remove a subtopic.
- September 28 is the overview; September 30 is Dr. Hengtao Guo's guest lecture
  with the MaxText repository link. October 14 is the project proposal session.
  Mid-term reports occupy November 4 and the first half of November 9; the
  SGLang reading is in the second half of November 9. Final project reports
  occupy November 30 and December 2. Unspecified deadlines are left blank.
- Edit `style.css` to adjust colors, spacing, or typography. UCLA colors are
  defined at the top of the file.
- The Sponsors and Resources section links to TRC, MaxText, Claude's program for
  scientists, and student offers from Kiro and Google. Check the linked program
  pages when updating availability, eligibility, or offer deadlines.

All links to local assets are relative, so the page works at the requested
subdirectory and can also be opened directly from disk. Navigation remains
available on small screens; the schedule scrolls horizontally when needed.

## Preview from this server

From the repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

If viewing from a Mac connected over SSH, run this in a **Mac terminal**, replacing
`YOUR_SERVER` with the same host or SSH alias you normally use:

```sh
ssh -N -L 8000:127.0.0.1:8000 yrbding@YOUR_SERVER
```

Then open <http://localhost:8000/teaching/cs239_fall2026/> in the Mac browser.

## Hosting and design sources

These files can be served directly by GitHub Pages. Once this repository is
published with Pages, the course path is `/teaching/cs239_fall2026/`.

The academic layout is inspired by [Stanford CS336](https://cs336.stanford.edu/).
The stylesheet and markup are independent. Course information not yet supplied
remains as placeholders.

- [UCLA brand colors](https://brand.ucla.edu/identity/colors).
- The official white UCLA logo is saved at `../../assets/ucla-logo-white.svg`
  from [UCLA's website](https://www.ucla.edu/img/logo_UCLA_white.svg).
- The COIN Lab logo uses the existing `../../assets/coin_logo_rectangle.png`.
