# Aditya Prakash — Professional Academic Résumé Website

A clean, fully responsive academic portfolio built with **HTML, CSS and a small JavaScript file**, designed for the web development assignment. The website requires no framework, server, build step or installation to display.

## What's different in this revision?

This version is deliberately more conservative and professional than the previous design:

- **Academic visual identity:** White and soft-grey backgrounds, dark navy text, muted blue accents, fine dividing rules and restrained borders instead of illustrations, decorative effects or large coloured panels.
- **Typography:** Source Serif 4 for titles and DM Sans for body/navigation, with readable fallback fonts; controlled heading scale and comfortable paragraph line spacing.
- **Clear information hierarchy:** Concise homepage with a summary and factual current appointments, followed by structured research, projects, education, skills, coursework, leadership, distinctions and contact sections.
- **Subtle CSS:** Grid-based section and card layout, flexbox navigation, consistent spacing, minimal hover styling, sticky header and responsive navigation.
- **Accessibility:** Semantic HTML, clear anchor navigation, keyboard-visible focus, skip link, labelled mobile-menu button, and reduced-motion support.

## Files

```text
index.html
.nojekyll
README.md
assets/
  styles.css
  script.js
  favicon.svg
  Aditya_Prakash_CV.pdf
```

All links and assets use **relative paths**, which makes the site compatible with a GitHub Pages *project* URL such as `https://USERNAME.github.io/REPOSITORY/`.

## CSS concepts demonstrated for the assignment

| Course concept | Implementation |
|---|---|
| Colour and fonts | Accessible navy/white/slate palette; serif headings and sans-serif reading text |
| Class and element selectors | `.research-entry`, `.section-top`, `.btn-primary`, `body`, `h1`, `a` |
| ID selectors | Page anchors `#research`, `#education`, `#contact` |
| Pseudo-selectors | `:hover`, `:focus-visible`, `:nth-child` |
| Box model | `margin`, `padding`, `border` and `box-sizing` for consistent spacing |
| Flexbox | Navigation links, action links, research keyword labels |
| CSS Grid | Hero, education rows, project highlight, skills and contact layouts |
| Positioning | `position: sticky` for navigation and `position: absolute` for mobile menu |
| Responsive design | Media queries at 1050px, 800px, 600px, and 400px |
| Navigation and usability | Anchor links, CV button, accessible collapsible mobile navigation |

## Preview locally

1. Extract the ZIP file.
2. Open `index.html` in Chrome, Edge or Firefox on your computer.
3. Click the menu links and verify each section.
4. Optional: start a local server with `python -m http.server 8000` and open `http://localhost:8000`.

## Publish through GitHub Pages (update the SAME repository)

1. On a **computer browser**, sign in at GitHub and open the repository used for your earlier HTML résumé assignment.
2. Upload the new `index.html`, `.nojekyll`, `README.md` and the `assets` folder contents to the **root** of that repository. Ensure the new `index.html` and `assets/styles.css` replace the old versions. Do **not** upload the ZIP itself as your website.
3. On the repository's **Settings → Pages** page, under **Build and deployment**, choose **Deploy from a branch**, select the website's branch (usually `main`) and `/ (root)`; save. If GitHub Pages was already enabled, just commit the new source files.
4. Visit the published URL in desktop and mobile browsers. Verify the navigation, research text, links and CV file.
5. Keep the final live URL and repository URL. Both must be inserted into the **same 1–2 page PDF** for your assignment.

**If updating with Git on your computer:**

```bash
git add index.html .nojekyll README.md assets/
git commit -m "Refine academic resume portfolio styling"
git push origin main
```

Use your actual default branch name if it is not `main`.

## Privacy and academic verification

- The included CV is the same user-provided PDF, not a newly generated CV. **It contains a phone number**. Hosting it makes the PDF publicly available, so remove its link and the PDF if you do not want that information public.
- An IIM Bangalore student ID card was used **only to verify the BBA DBE programme affiliation**. The ID card, photograph, roll number, blood group and date of birth were not included in the website.
- Read the source and confirm the accuracy of programme status, dates, research descriptions and links before publishing.

## Assignment submission

**Do not submit the ZIP as the final assignment PDF.** After the site is live, provide the live website URL and repository URL. The final single PDF should contain both links and a concise account of the website sections, design decisions and CSS improvements.

Expected final filename: `26120099_WD_MTProject.pdf`.
