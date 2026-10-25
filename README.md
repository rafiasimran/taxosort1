# TaxoSort: AI Learning Content Classifier

Companies have thousands of courses in their learning platforms, and most of them are tagged badly or not at all. TaxoSort is my attempt at fixing that. You paste in a list of course titles, pick a framework, and an LLM sorts every title into a clean, structured taxonomy you can export straight into an LMS.

**[Live demo](https://rafiasimran.github.io/taxosort1/taxosort1.html)** (demo mode works without an API key)

## What it does

- **Three classification frameworks**
  - Standard L&D: Domain → Category → Subcategory → Topic
  - Bloom's Taxonomy: Level → Domain → Skill → Learning Outcome
  - Skills & Competency: Function → Competency → Skill → Proficiency
- **Three AI providers in one UI:** Anthropic Claude, Google Gemini and OpenAI, switchable from the settings panel
- **Analytics as you go:** a content health score, the confidence distribution and the top domains
- **LMS-ready export:** filtered results as CSV (shaped for SAP SuccessFactors, Cornerstone, Moodle and Workday Learning) or as JSON
- **Demo mode** with synthetic SAP, technology, business, data science and HR content, so anyone can try it

## How it's built

I kept it deliberately small: **one HTML file, no build step, no backend.**

- HTML5 and CSS3 with a responsive grid and a dark theme
- Vanilla JavaScript with `async`/`await` to run classification requests in parallel
- Requests go straight from the browser to the AI provider over HTTPS

## Privacy

TaxoSort uses a "bring your own key" model. Your API key and your course data go directly from your browser to the provider you chose. There's no server in between, no database and no tracking.

## Run it yourself

1. Download `taxosort1.html` (or clone the repo).
2. Open it in any modern browser.
3. Paste an API key for Claude, Gemini or OpenAI into the settings panel, or just use demo mode.
4. Paste your course titles, one per line, and click **Classify Now**.

## Tech

HTML · CSS · JavaScript · Claude API · Gemini API · OpenAI API · GitHub Pages

## License

MIT

---

Built by **Rafia Imran** · [GitHub profile](https://github.com/rafiasimran) · [Live CV](https://rafiaimran.cloud)
