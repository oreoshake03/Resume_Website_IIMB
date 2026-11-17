# Aditya Prakash — Academic Portfolio

A personal academic website presenting my research experience, education, technical projects, skills, and interests in machine learning and computational science. The website is a single-page portfolio built with HTML, CSS, and JavaScript, with a downloadable PDF copy of my CV.

## Development

### Planning and page structure

I organised the content around the information a reader would most likely look for: a short introduction, current research, earlier work, education, technical skills, leadership, and contact details. Research experience appears near the top because it is the main focus of the portfolio. Each research entry includes its dates, institution or context, a description of the work, and relevant methods or tools.

The page uses semantic HTML elements such as `header`, `nav`, `main`, `section`, `article`, `aside`, and `footer`. Sections have individual IDs so the navigation links take readers directly to the relevant content. The site is kept on one page to make it easy to scan without switching between multiple pages.

### Visual design and typography

I chose a restrained colour palette of white, navy, slate grey, and muted blue. White space and fine borders separate sections without making the page feel crowded. Headings and body text use different typefaces: **Source Serif 4** for major headings and **DM Sans** for navigation, descriptions, and smaller labels. Both are loaded through Google Fonts, with system-font fallbacks defined in CSS.

The styling is contained in `assets/styles.css`. Reusable colour, font, and content-width values are defined as CSS custom properties in `:root`, making the overall appearance easier to maintain. Element, class, and state selectors control the typography, spacing, borders, links, and interactive states. A consistent heading hierarchy and spacing system help distinguish research titles, institutional details, dates, and supporting information.

### Layout with CSS

I used **Flexbox** for the header navigation, action links, and keyword labels, where items need to align within a row or wrap naturally. **CSS Grid** handles larger two-column arrangements, including the introduction and current-status panel, research entries, project feature, education entries, skills, and contact section.

The header uses `position: sticky` to keep the navigation accessible as the reader scrolls. Research entries use a date column beside the main description on larger screens. The project section gives space to both the software description and a numerical summary of its operational scale. Alternating white and pale-grey section backgrounds provide visual separation while keeping the page consistent.

### Responsive behaviour

Media queries adjust the layout at narrower viewport widths, including breakpoints at **1050px, 800px, 600px, and 400px**. On tablets and phones, multi-column sections progressively move into simpler layouts; text sizes and spacing are reduced where appropriate, and the navigation becomes a collapsible menu below 800px. The objective was to keep research descriptions readable without horizontal scrolling or cramped columns.

### JavaScript and navigation

The JavaScript in `assets/script.js` is intentionally small. It opens and closes the mobile navigation, updates the menu button's `aria-expanded` state and label, closes the menu after selecting a section or pressing **Escape**, and resets it when the viewport becomes wider. It also updates the copyright year automatically. The rest of the website works as a static HTML and CSS page without a framework.

### Accessibility and usability

I added a **Skip to main content** link for keyboard users and visible focus outlines for links and buttons. The navigation has accessible labels, the mobile menu communicates whether it is expanded, and the page respects the browser's **reduced-motion** preference. Section links, contact links, and the CV download provide direct routes to the most useful information.

## Technologies

- **HTML5** — semantic content and page structure
- **CSS3** — typography, colour, spacing, selectors, Flexbox, Grid, and media queries
- **JavaScript** — responsive navigation and automatic copyright year
- **Google Fonts** — Source Serif 4 and DM Sans
- **GitHub Pages** — static website hosting

No CSS framework, package manager, or build process is required.

## Project files

```text
index.html
README.md
.nojekyll
assets/
  styles.css
  script.js
  favicon.svg
  Aditya_Prakash_CV.pdf
```

`index.html` contains the content and section links. `styles.css` defines the appearance and responsive layouts, while `script.js` manages the mobile menu. The `assets` folder also contains the favicon and downloadable CV.

## Running locally

Download or clone the repository, then open `index.html` in a browser. The site does not need a development server. An internet connection is needed to load the Google Fonts; fallback fonts are available if they cannot be reached.

## Publishing with GitHub Pages

1. Add `index.html`, `README.md`, `.nojekyll`, and the complete `assets` directory to the root of a GitHub repository.
2. Commit and push the files to the `main` branch.
3. Go to **Settings → Pages** in the repository.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main`, and choose `/ (root)`.
5. Save. Once GitHub Pages finishes publishing, the live website address will appear in the Pages settings.

Subsequent updates can be published by committing and pushing changes to the same branch.

## Contact

[LinkedIn](https://www.linkedin.com/in/adityaprakash19/) · [Email](mailto:25f1001933@ds.study.iitm.ac.in)
