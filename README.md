<div align="center">

# Arth Patel

**Engineer by training, researcher by habit.**
M.Tech, IIT Bombay · Structural Engineering & Computational Mechanics

A hand-sketched, single-file portfolio with a day / night theme.

[**Live site**](https://arthpatel02.github.io/portfolio/) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/arthpatel02) &nbsp;·&nbsp; [GitHub](https://github.com/ArthPatel02) &nbsp;·&nbsp; [Email](mailto:iarthpatel1405@gmail.com)

![HTML5](https://img.shields.io/badge/HTML5-single%20file-f7dd8e?style=flat-square&logo=html5&logoColor=1d1c1a)
![CSS3](https://img.shields.io/badge/CSS3-custom%20properties-a9e5cf?style=flat-square&logo=css3&logoColor=1d1c1a)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-f7dd8e?style=flat-square&logo=javascript&logoColor=1d1c1a)
![Responsive](https://img.shields.io/badge/responsive-320%E2%80%931440px-a9e5cf?style=flat-square)
![No dependencies](https://img.shields.io/badge/dependencies-none-1d1c1a?style=flat-square)

<!-- Add a screenshot: save it as docs/preview.png and uncomment the next line -->
<!-- <img src="docs/preview.png" alt="Portfolio preview" width="860"> -->

</div>

---

## About this project

This is the source of my personal portfolio. It is one `index.html` file with no build step, no framework and no package manager. Open it in a browser and it works.

The design idea is simple: every page opens with a small hand-drawn sketch that tells a little story, and the content underneath stays clean and quiet.

## Highlights

- **Hand-drawn illustrations.** Inline SVG sketches that draw themselves on scroll, with a slightly rough, pencil-like edge.
- **Day and night themes.** Butter yellow in the day, mint at night. The day theme opens first, and the choice is remembered in the browser.
- **Fully responsive.** Checked from 320px phones up to 1440px desktops, with no sideways scrolling.
- **Fast.** No libraries, no images required for the sketches, and short draw-on animations.
- **Interactive touches.** A custom cursor on desktop, an animated grid on the home page, and a full-screen menu on phones.
- **Project pop-ups.** Each of the "Other projects" opens a card with the details, tools and dates.
- **Self-sorting list.** Projects are ordered newest first from their dates, so adding one is a single line.

## Pages

| Page | What is there |
|---|---|
| **Home** | Introduction, sketch, and a short strip of featured work |
| **About** | My story, written in my own words, with a portrait |
| **Research** | Four research themes and the tools and software I use |
| **Projects** | Research projects, plus other projects with detail pop-ups |
| **Journey** | Education and work experience |
| **Contact** | Email, location and links, with a copy-to-clipboard button |

## Project structure

```text
.
├── index.html        # the whole site: HTML, CSS and JavaScript
├── README.md
├── images/
│   ├── about.jpg     # portrait on the About page
│   └── photo.jpg     # fallback portrait
├── logos/
│   ├── iitb.png      # IIT Bombay (Journey)
│   └── iitt.png      # IIT Tirupati (Journey)
└── tools/            # software logos for the Research page
    ├── abaqus.avif
    ├── ansys.svg
    ├── matlab.svg
    ├── python.svg
    ├── staadpro.svg
    ├── etabs.svg
    ├── geostudio.svg
    ├── osgad.svg
    ├── autocad.svg
    ├── autocad_arch.svg
    ├── rivet.svg
    └── overleaf.svg
```

## Run it locally

```bash
git clone https://github.com/ArthPatel02/portfoilo.git
cd portfoilo

# Option 1: just open the file
open index.html            # macOS  (use "start index.html" on Windows)

# Option 2: serve it locally
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Make it yours

Everything is in `index.html`, so a text search finds what you need.

| To change | Search for |
|---|---|
| Accent colours | `--accent` (day colour in `:root`, night colour in `html[data-theme="dark"]`) |
| Email and links | `mailto:` and `linkedin.com` |
| Photos and logos | Replace the files in `images/`, `logos/` and `tools/` with the **same file name** |
| Add a project | Copy a row inside the `Other projects` block and change the title, `data-date`, `data-text` and `data-tools` |
| Project order | Nothing to do. Rows sort themselves, newest first |

A project row looks like this. Separate the bullet points in `data-text` with a `|`.

```html
<div class="project pg-other" data-type="" data-date="Jan 2025 – Apr 2025"
     data-title="Project name"
     data-text="First point.|Second point."
     data-tools="MATLAB · FEM">
  <div class="no">01</div>
  <div><h3>Project name</h3></div>
  <div class="pdate">Jan 2025 – Apr 2025</div>
</div>
```

## Deploy on GitHub Pages

1. Push the files to a repository on GitHub.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and the `/ (root)` folder.
4. Save. The site will be live at `https://<your-username>.github.io/<repository-name>/` in a minute or two.

## Built with

- HTML5, CSS3 (custom properties for the themes) and vanilla JavaScript
- Inline SVG with a turbulence filter for the sketch effect
- `IntersectionObserver` for the draw-on animations
- Google Fonts: Inter

## Contact

Interesting problems start with a question. For research discussions, collaborations or academic opportunities:

- Email: [iarthpatel1405@gmail.com](mailto:iarthpatel1405@gmail.com)
- LinkedIn: [linkedin.com/in/arthpatel02](https://www.linkedin.com/in/arthpatel02)
- GitHub: [github.com/ArthPatel02](https://github.com/ArthPatel02)

## License

© 2026 Arth Patel. All rights reserved.
The code and content are shared here to view. Please ask before reusing the design, text or illustrations.
