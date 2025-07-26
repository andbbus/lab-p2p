## lab-p2p
Repo for the peer-to-peer lab of Economics &amp; Development

# Peer-to-Peer Data Science \& AI Lab — Comprehensive Syllabus \& Resource Index

The following index lays out a full-semester laboratory programme (12 bi-weekly sessions plus two optional deep-dives).  Each topic includes (1) a concise syllabus with learning outcomes, (2) a recommended session structure, and (3) curated, English-language resources for self-study and hands-on exercises.  All materials are openly accessible and were selected for beginners and intermediate users in Economics \& Development.

## Programme Map \& Sequence

| Week | Theme | Core Skills | Capstone Output |
| :-- | :-- | :-- | :-- |
| 0 | On-boarding \& Toolchain Setup | R/RStudio, Git, Overleaf accounts | Working development environment |
| 1–2 | Data Visualisation with ggplot2 | Grammar of Graphics, plot types | Re-create a TidyTuesday chart |
| 3–4 | Reproducible Documents with RMarkdown \& Quarto | Dynamic reports, slides, blogs | Publish a brief data story |
| 5 | Technical Writing in LaTeX (Overleaf) | Academic layouts, citations | Conference-style paper template |
| 6 | Git \& GitHub Workflow | Version control, collaboration | Personal portfolio repository |
| 7–8 | Interactive Apps with Shiny | Reactive programming, UI design | Deploy a mini dashboard |
| 9 | Data Challenges (TidyTuesday \& Kaggle) | Wrangling, EDA, storytelling | TidyTuesday challenge submission |
| 10 | Replication Packages \& Open Science | Codebooks, data sharing | Reproduce a published figure |
| 11 | Large-Language Models for Research | Prompt engineering, code assist | AI-accelerated literature matrix |
| 12 | Showcase \& Peer Review | Presentation, feedback loops | Live demo \& portfolio critique |
| Optional A | Spatial Data \& Mapping | sf, tmap, leaflet | Choropleth for an SDG indicator |
| Optional B | Advanced Visual Design | Themes, brand palettes | House-style ggplot2 theme R pkg |

## Session 0 — Kick-Off \& Environment Boot-Strap

### Learning Goals

- Install R ≥ 4.3, RStudio, Git, and basic TeX distribution.
- Create free accounts on GitHub, Overleaf, Kaggle, Posit Cloud, and shinyapps.io.
- Fork the shared repository `lab-p2p` and clone locally.


### Pre-lab Checklist

1. Follow Posit’s official installation guide (R + RStudio) [^1].
2. Install `tidyverse`, `ggplot2`, `quarto`, `shiny`, `devtools` packages in one R script.
3. Generate an SSH key and connect RStudio to GitHub [^2].
4. Open Overleaf’s *Learn LaTeX in 30 Minutes* interactive tutorial [^3].

### Resources

| Type | Title \& Link | Notes |
| :-- | :-- | :-- |
| Guide | Shiny “Hello World” example (`runExample("01_hello")`) [^4] | Verify Shiny works locally. |
| Cheatsheet | `data-visualization-with-ggplot2.pdf` [^5] | Print for quick reference. |
| Video | *Learn Overleaf in 6 Minutes* [^6] | Fast orientation to the IDE. |

## Module 1 — Data Visualisation with ggplot2 (Weeks 1-2)

### Syllabus Overview

1. Grammar of Graphics theory and `ggplot(data) + aes() + geom_*()` pipeline [^7][^8].
2. Core geoms: scatter, line, bar, histogram, boxplot [^9].
3. Faceting, scales, themes, annotations [^10][^11].
4. Extension ecosystem (`gganimate`, `patchwork`, `ggthemes`).
5. TidyTuesday case study: reproduce Cedric Scherer’s energy chart [^10].

### Key Resources

| Category | Resource | Description |
| :-- | :-- | :-- |
| Textbook | *R for Data Science*, Ch.3 (Data Viz) [^12] | Authoritative introduction. |
| Tutorial | *Be Awesome in ggplot2* Practical Guide [^9] | Step-wise examples. |
| Practice | *Data Visualisation in R* DataQuest course [^13] | Browser-based exercises. |
| Cheat Sheet | Posit ggplot2 sheet [^5] | Compact geom reference. |
| Exercises | Bioinformatics ggplot2 tasks (incl. solutions) [^14] | Self-graded tasks. |

## Module 2 — Reproducible Documents with RMarkdown \& Quarto (Weeks 3-4)

### Syllabus Overview

- Markdown syntax, code chunks, YAML metadata.
- Export pipelines: HTML, PDF, Word, reveal.js slides.
- Parameterised reports and Quarto projects [^15].
- Embedding interactive `htmlwidgets` (plotly, leaflet).
- Continuous integration publishing via GitHub Pages.


### Assigned Readings \& Exercises

| Reading | Focus | Task |
| :-- | :-- | :-- |
| Quarto Docs *Getting Started* [^15] | Project scaffolding | Convert ggplot2 lab into a Quarto HTML report. |
| RMarkdown Website *Output Formats* [^15] | Format options | Render same doc to PDF \& Word. |
| Quarto Gallery *Blogdown Template* [^15] | Theming | Fork template, edit home page. |

## Module 3 — Technical Writing in LaTeX \& Overleaf (Week 5)

### Syllabus Overview

1. Document classes (`article`, `paper`, `beamer`).
2. Sections, figures, tables, equations (`align`, `tikz`).
3. BibTeX/BibLaTeX citation workflows.
4. Overleaf real-time collaboration \& Git integration [^16][^17].
5. Building a template for course term papers.


### Curated Resources

| Type | Link | Purpose |
| :-- | :-- | :-- |
| Wikibook | *LaTeX Wikibook* TOC [^18] | Free reference from basics to advanced maths. |
| Overleaf Tutorial | *Learn LaTeX in 30 Minutes* [^3] | Interactive. |
| Video | *Overleaf in Minutes!* 13-min walkthrough [^19] | Visual workflow. |
| PDF | Complete LaTeX manual (Wikibooks PDF) [^20] | Offline reading. |

## Module 4 — Git \& GitHub for Reproducible Research (Week 6)

### Syllabus Overview

- Git fundamentals: init, add, commit, branch, merge [^2].
- Linking RStudio projects to remote repositories [^2].
- Pull requests and code review etiquette.
- GitHub Pages \& Actions for automated Quarto builds.
- Personal academic portfolio site (skills, projects, CV).


### Resources

| Medium | Title | Utility |
| :-- | :-- | :-- |
| Interactive | GitHub Learning Lab: *Introduction to GitHub* [^2] | Guided quests with bot feedback. |
| Doc | GitHub Docs *Using Git with RStudio* [^2] | Step-by-step screenshots. |
| Cheat | Atlassian Git cheat-sheet (search “git-cheatsheet.pdf”) | Quick command lookup. |

## Module 5 — Interactive Apps with Shiny (Weeks 7-8)

### Syllabus Overview

1. Reactive programming model (inputs, outputs, observers) [^4].
2. UI layouts (`fluidPage`, `sidebarLayout`, `tabsetPanel`).
3. Server logic: `renderPlot`, `reactive`, `observeEvent` [^21].
4. Deployment options (shinyapps.io, Posit Connect, Docker).
5. Enhancements: `bslib`, `shinythemes`, loading screens [^22].

### Learning Materials

| Category | Link | Comment |
| :-- | :-- | :-- |
| Course | RStudio-education Shiny short course [^24] | Four modules with Cloud exercises. |
| Book | *Mastering Shiny* Ch.1-3 [^21] | De-facto reference. |
| Cheatsheet | Shiny R cheatsheet (Posit) [^25] | Two-page printable. |
| GitHub Repo | Dean Attali’s *advanced-shiny* patterns [^22] | Copy-paste solutions for loading screens, URL params. |
| Video | *R Shiny Full Tutorial* (Data Professor) [^26] | 20-minute conceptual intro. |

## Module 6 — Data Challenges: TidyTuesday \& Kaggle (Week 9)

### Syllabus Overview

- Discovering open datasets; reading API docs.
- EDA pipeline (`skimr`, `janitor`, `DataExplorer`).
- From raw → tidy → visual story.
- Writing Kaggle kernels and TidyTuesday social media posts.


### Exercise

Produce a 280-character tweet thread with GIF of your ggplot2 visualisation; push code and `README.md` to your portfolio repo.

### Resource Pack

| Link | Why It Matters |
| :-- | :-- |
| TidyTuesday GitHub (`github.com/rfordatascience/tidytuesday`) | Weekly datasets \& starter scripts. |
| Kaggle *Getting Started with R* notebook (search “Kaggle R Tutorial”) | Shows kernel workflow. |

## Module 7 — Replication Packages \& Open Science (Week 10)

### Syllabus Overview

- Anatomy of a replication package (README, data, code, outputs).
- Tools: `renv`, `packrat`, `here`, `targets`.
- Zenodo DOI minting; linking to GitHub releases.
- Re-producing a figure from a policy evaluation paper (provided).


### Readings

| Source | Key Take-away |
| :-- | :-- |
| Journals’ replication polices summary (AEA, JDE) — see Econ literature review. | Understand submission requirements. |
| Blog | ROpenSci guide to reproducible research (search) |

## Module 8 — Large-Language Models for Academic Workflow (Week 11)

### Syllabus Overview

1. Prompt engineering patterns: “chain-of-thought”, “expert persona”, “refine”.
2. AI-assisted R coding via GitHub Copilot \& ChatGPT API [^27].
3. Semantic search for literature (Elicit, ScholarAI).
4. Ethical considerations \& citation of AI output.

### Lab Activity

Use ChatGPT to generate boilerplate code for a Shiny module, then review and refactor manually; document gains \& pitfalls in Quarto notebook.

### Resource List

| Type | Link | Notes |
| :-- | :-- | :-- |
| Docs | OpenAI Platform documentation [^27] | API endpoints, rate limits. |
| Blog | Shiny blog post: new component gallery [^27] | Example of AI-augmented docs. |
| Webinar | Posit *AI in RStudio* series (search) | Best practice demos. |

## Module 9 — Showcase \& Peer Review (Week 12)

### Deliverables

- **Live demo:** 5-minute Shiny dashboard or Quarto blog.
- **Repository health:** README, licence, issue tracker.

Peers assess using rubrics hosted in GitHub Issues; maintainers merge feedback as discussions.

## Reading \& Resource Master Table

| Theme | Primary Resource | Type |
| :-- | :-- | :-- |
| ggplot2 Fundamentals | *Be Awesome in ggplot2* [^9] | Article |
| Advanced Plot Customisation | Cédric Scherer tutorial [^10] | Blog |
| Shiny Basics | Posit lesson \#1 [^4] | Online lesson |
| Shiny Patterns | Dean Attali repo [^22] | Code gallery |
| Quarto Projects | quarto.org docs [^15] | Manual |
| LaTeX Reference | LaTeX Wikibook [^18] | Book |
| Git-RStudio Integration | Posit support article [^2] | Guide |
| AI API Usage | OpenAI docs [^27] | API reference |

## Logistics \& Community Channels

- **Repo:** `https://github.com/your-org/lab-p2p`
- **Chat:** Discord “\#unifi-end-labp2p” server for Q\&A.
- **Issue tracker:** Use labels `help-wanted`, `resource-suggestion`, `session-idea`.


### Final Notes

This index is designed as a living document; contributors are encouraged to open pull requests with improved resources or new exercise ideas.  Continuous peer-led evolution is the core philosophy of the lab—learn, build, share, repeat.

<div style="text-align: center">⁂</div>

[^1]: https://ggplot2.tidyverse.org

[^2]: https://bookdown.org/hneth/ds4psy/2.7-visualize:ex.html

[^3]: https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes

[^4]: https://shiny.posit.co/r/getstarted/shiny-basics/lesson1/

[^5]: https://posit.co/wp-content/uploads/2022/10/data-visualization-1.pdf

[^6]: https://www.youtube.com/watch?v=xcTN4F3l9Ds

[^7]: https://www.sthda.com/english/wiki/ggplot2-essentials

[^8]: https://www.rdocumentation.org/packages/ggplot2/versions/3.5.2

[^9]: http://r-statistics.co/Complete-Ggplot2-Tutorial-Part1-With-R-Code.html

[^10]: https://www.cedricscherer.com/2019/08/05/a-ggplot2-tutorial-for-beautiful-plotting-in-r/

[^11]: https://rstudio.github.io/cheatsheets/html/data-visualization.html

[^12]: https://github.com/sefakilic/ggplot-cheatsheet

[^13]: https://www.dataquest.io/course/r-data-viz/

[^14]: https://www.bioinformatics.babraham.ac.uk/training/ggplot_course/ggplot_exercise_answers.html

[^15]: https://www.overleaf.com/learn/latex/Tutorials

[^16]: https://www.overleaf.com/for/edu

[^17]: https://www.overleaf.com/learn/how-to/Can_I_use_Overleaf_to_teach_LaTeX_to_my_students%3F

[^18]: https://en.wikibooks.org/wiki/Wikibooks:Collections/LaTeX

[^19]: https://www.youtube.com/watch?v=kPpUOte45WE

[^20]: https://ftpmirror.your.org/pub/wikimedia/images/wikipedia/commons/archive/2/2d/20120416201943!LaTeX.pdf

[^21]: https://mastering-shiny.org/basic-app.html

[^22]: https://github.com/daattali/advanced-shiny

[^23]: https://ourcodingclub.github.io/tutorials/shiny/

[^24]: https://rstudio-education.github.io/shiny-course/

[^25]: https://shiny.posit.co/r/articles/start/cheatsheet/

[^26]: https://www.youtube.com/watch?v=jxsKUxkiaLI

[^27]: https://shiny.posit.co/blog/posts/introducing-component-layouts/

[^28]: https://flowingdata.com/visualization-in-r/

[^29]: https://www.studocu.com/en-ca/document/simon-fraser-university/econ/final-cheatsheet-data-visualization-with-ggplot2-r/124554757

[^30]: https://cran.rstudio.com/web/packages/ggplot2/readme/README.html

[^31]: https://www.datacamp.com/tracks/data-visualization-with-r

[^32]: https://github.com/bioinformatics-core-shared-training/r-intermediate/blob/master/ggplot2-exercises-with-solutions.Rmd

[^33]: https://www.reddit.com/r/rstats/comments/dzmkdr/the_complete_ggplot2_tutorial_most_comprehensive/

[^34]: https://cran.r-project.org/web/packages/ggplot2/refman/ggplot2.html

[^35]: https://www.udemy.com/course/r-graphics-data-visualization/

[^36]: https://myslu.stlawu.edu/~iramler/stat234/coursenotes/examples-with-ggplot2.html

[^37]: https://www.youtube.com/watch?v=_PzDLFJHO3E

[^38]: https://www.overleaf.com/for/universities

[^39]: https://www.scribd.com/document/94991689/Latex-Wikibook

[^40]: https://www.egr.msu.edu/decs/software/overleaf

[^41]: https://www.overleaf.com/latex/examples/latex-tutorials/jgvvmxktcvdr

[^42]: https://en.wikipedia.org/wiki/LaTeX

[^43]: https://it.overleaf.com/for/edu

[^44]: https://en.wikibooks.org/wiki/LaTeX

[^45]: https://zh.wikibooks.org/zh-sg/LaTeX

[^46]: https://it.overleaf.com

[^47]: https://www.youtube.com/watch?v=g8Ejj0T0yG4

[^48]: http://www-hep.colorado.edu/~jcumalat/4610_spr_09/Wikibooks_LaTeX_Guide.pdf

[^49]: https://www.scribd.com/document/317825504/Shiny-Cheatsheet

[^50]: https://github.com/mrjoh3/gallerier

[^51]: https://bookdown.org/paulcbauer/applied-data-visualization/11-shiny.html

[^52]: https://www.youtube.com/watch?v=wkXxeqVdrCY

[^53]: http://www.htmldrive.net/items/show/235/ShineTime-A-New-jQuery-CSS3-gallery-With-Animated-Shine-Effects

[^54]: https://github.com/stefanieschneider/shinygallery

[^55]: https://shiny.posit.co/r/getstarted/

[^56]: https://www.scribd.com/document/356892080/shiny-cheatsheet-pdf

[^57]: https://bookdown.org/lyzhang10/lzhang_r_tips_book/how-to-learn-shiny.html

[^58]: https://github.com/jos4uke/shiny_tutorial

[^59]: https://shiny.posit.co/r/getstarted/shiny-basics/lesson2/

[^60]: https://shiny.posit.co/r/gallery/
