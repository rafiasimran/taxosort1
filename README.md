TaxoSort is a lightweight, privacy-focused Single-Page Application (SPA) that automatically categorizes learning content and course titles into structured taxonomies using modern Large Language Models (LLMs). The application operates on a BYOK (Bring Your Own Key) model, meaning all API requests are sent directly from your browser to the respective provider. There is no middle-tier server and no data retention.

Features:
Multi-Framework Support: Classify content according to three standard frameworks:
Standard L&D Framework (Domain → Category → Subcategory → Topic)
Bloom's Taxonomy (Level → Domain → Skill → Learning Outcome)
Skills & Competency Framework (Function → Competency → Skill → Proficiency)
Three Integrated AI Providers: Seamlessly switch between Anthropic (Claude), Google (Gemini), and OpenAI (GPT-4o) directly from the UI.
Real-Time Analytics & Metrics: Instantly calculates a Content Health Score, displays confidence distribution, and lists top domains.
LMS-Ready Export: Filter and export your results as a standardized CSV (optimized for SAP SuccessFactors, Cornerstone, Moodle, Workday Learning) or as JSON.
Demo Mode: Fully functional preview loaded with synthetic demo data for SAP, Technology, Business, Data Science, and HR content—no API key required to test the UI.
🛠️ Technical Architecture
This project is built with a minimalist, "zero-dependency" approach:
HTML5 & CSS3: Single-file layout featuring a responsive CSS Grid system and a modern dark theme (using Inter & JetBrains Mono fonts).
Vanilla JavaScript: Native asynchronous operations (async/await) for parallel API requests to the AI providers.
Direct Browser Integration: Utilizes direct browser-to-API communication (e.g., using anthropic-dangerous-direct-browser-access for Claude).


Installation & Usage:
Because TaxoSort runs entirely in the browser, no server-side installation or build step is required.
Clone the repository or download the taxosort1.html file.
Open taxosort1.html directly in any modern web browser (Chrome, Firefox, Safari, Edge).
Paste your respective API key (Anthropic, Google, or OpenAI) into the configuration panel.
Paste your course titles (one per line) and click "Classify Now".

Privacy & Security
Local Execution: The application runs entirely on the client side (in your browser).
No Tracking: There is no backend database caching your prompts, API keys, or classification results.
Secure Connections: All requests are made via encrypted HTTPS connections directly to the official provider APIs.

License
This project is licensed under the MIT License

