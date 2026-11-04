# Aaditya Chandola · Portfolio

My personal portfolio site: a single responsive page covering my experience, projects and skills.

**Live site:** https://aaditya-develop.github.io/portfolio-site/

## What's on the site

| Section | Contents |
| --- | --- |
| **Hero** | Intro with a typing tagline, resume download and social links |
| **About** | Background, Rutgers CS & Data Science, certifications and achievements |
| **Experience** | Software Engineering Intern (AI) at Ryan, LLC: AG2 retrieval pipelines for the Canadian tax team, with an illustration of Ryan Tower |
| **Projects** | SEC 10-K Research Assistant (agentic RAG with LangGraph) and the Board & Brush Timesheet App (Swift + Supabase) |
| **Toolkit** | Languages, AI and data tools, backend and deployment |
| **Contact** | Email and LinkedIn |

## Featured work

**SEC 10-K Research Assistant.** A multi-agent RAG system that answers questions about company annual reports. A LangGraph router sends each question to hybrid retrieval (ChromaDB + BM25), Tavily web search or the model's own knowledge. A GPT-4o writer then checks its answer against the sources and regenerates it if it isn't grounded. RAGAS checks gate quality (faithfulness ≥ 0.90, relevancy ≥ 0.85), and the system is served through FastAPI on Azure.

**Board & Brush Timesheet App.** A mobile app built for Board & Brush Creative Studio to replace paper timesheets. It has separate employee and admin logins, time logging, employee management and hour reports, all backed by Supabase and PostgreSQL. [View code →](https://github.com/Aaditya-develop/board-brush-timesheet-ios)

## Built with

- Hand-written **HTML, CSS and JavaScript**, with no framework and no build step
- [Typed.js](https://github.com/mattboldt/typed.js) for the typing effect
- [Font Awesome](https://fontawesome.com) icons and Google Fonts (Inter, Space Grotesk, JetBrains Mono)
- An `IntersectionObserver` for scroll-reveal animations and highlighting the active nav link
- Pure CSS and inline SVG for the RAG pipeline diagram, the phone mockup and the Ryan Tower illustration
- Responsive from phone to desktop, and respects `prefers-reduced-motion`

## Project structure

```
index.html       Main page (every section lives here)
styles.css       All styles, with design tokens at the top
script.js        Typing effect, mobile menu, scroll animations
aboutme.html     Redirects old links to index.html#about
assets/          Optimized photos used on the site
theResume.pdf    Downloadable resume
```

## Running locally

No build step is needed. Serve the folder and open it in a browser:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080.

## Deployment

The site is hosted on **GitHub Pages** from the `main` branch. Pushing to `main` updates the live site within a minute or two.

## Contact

- Email: aadityachandola@yahoo.com
- LinkedIn: [aaditya-chandola](https://www.linkedin.com/in/aaditya-chandola-141682345/)
- GitHub: [Aaditya-develop](https://github.com/Aaditya-develop)

## License

[MIT](LICENSE)
