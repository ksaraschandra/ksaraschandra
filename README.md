## Hi there 👋 
---

I explore the space at the intersection of **User Experience Research (UXR)** and **Artificial Intelligence**, leveraging advanced AI-assisted development (vibe coding with Claude Code, Cursor, Antigravity) to rapidly prototype and deploy robust, functional proof of concepts. My work focuses on creating human-in-the-loop AI prototypes that accelerate qualitative synthesis, ensure analytical rigor, and bridge the gap between complex research data and stakeholder decision-making.

## 🛠️ AI-Augmented UX Research Suite
These four projects form an end-to-end pipeline that transforms raw qualitative user research into validated, interactive, and secure stakeholder deliverables. All projects are grounded in a shared clinical research domain: **clinician trust calibration in AI-assisted Decision Support Systems (CDSS)**.

| Project & Repository | Core Objective | Key Differentiator | Tech Stack |
| :--- | :--- | :--- | :--- |
| **[Qualitative Coding Assistant](https://github.com/ksaraschandra/Qualitative-Coding-Assistant)** | AI-assisted transcript coding & tagging | **"AI proposes, human decides"** — preserves researcher agency with keyboard-driven validation instead of bulk auto-summarization. | Node.js, Ollama, Anthropic Claude, Dovetail API |
| **[Persona Similarity Engine](https://github.com/ksaraschandra/Persona-Similarity-Engine)** | Statistical validation of persona equivalence | **Bias-corrected similarity metrics** — uses a 7-stage NLP pipeline with three bias-correction layers to prevent merge errors. | Python, HTML5/Vanilla CSS |
| **[Interactive UX Research Report & Q&A](https://github.com/ksaraschandra/Interactive-UXResearch-Report-QA)** | Slide-integrated streaming Q&A deck | **Server-side hallucination guards** — intercepts and drops connections mid-stream if the LLM invents participant names. | Node.js, SSE, Anthropic Claude, Vanilla JS, CSS |
| **[One Customer Knowledge Hub](https://github.com/ksaraschandra/One-Customer-Knowledge-Hub)** | Federated multi-source feedback search & AI synthesis | **Federated MCP queries with zero cloud leakage** — queries NPS, CSAT, and support channels in parallel via stdio protocol and synthesizes trends locally. | Node.js, React, Model Context Protocol (MCP), Ollama (Mistral 7B) |

---
### 🔍 Deep Dive: The Projects

#### 1. [Qualitative Coding Assistant](https://github.com/ksaraschandra/Qualitative-Coding-Assistant)
A tool designed to speed up qualitative tagging without losing the researcher’s voice.
* **How it works:** Reads transcript files (`.vtt`) and taxonomy definitions, proposing structured highlights with quotes and rationales.
* **Differentiator:** Rejects passive delegation. The researcher must explicitly accept, edit, or reject each highlight. Includes few-shot style calibration and Dovetail API integration.

#### 2. [Persona Similarity Engine](https://github.com/ksaraschandra/Persona-Similarity-Engine)
An analytical tool to solve the common portfolio bloat problem: *"Do these two personas describe the same user?"*
* **How it works:** Extracts Jobs-to-be-Done (JTBDs), runs pairwise semantic comparisons, and calculates symmetric coverage ratios.
* **Differentiator:** Employs three independent bias-correction fixes (stratified tiers, raw-text tracks, and asymmetric penalties) to prevent false positives when comparing small and large personas.

#### 3. [Interactive UX Research Report & Q&A](https://github.com/ksaraschandra/Interactive-UXResearch-Report-QA)
A zero-dependency interactive presentation slide deck built directly for stakeholders.
* **How it works:** Allows stakeholders to read a research slide and instantly query the underlying corpus (transcripts, highlights) through an inline drawer.
* **Differentiator:** It runs server-side streaming regex guards (`detectInventedNames`) to instantly block responses if the LLM starts inventing participant names.

#### 4. [One Customer Knowledge Hub](https://github.com/ksaraschandra/One-Customer-Knowledge-Hub)
A unified workspace and search dashboard for querying fragmented user feedback databases.
* **How it works:** Connects to independent local database directories (NPS feedback, CSAT scores, support logs) and runs parallel search tool calls across these sources using the MCP standard.
* **Differentiator:** Operates entirely locally with zero cloud data leakage. Leverages a React frontend to monitor connections and stream synthesized research trends from local LLMs.

---
## 💻 Tech Stack & Skills
* **Languages:** JavaScript (ES6+), Python, HTML5, Vanilla CSS
* **AI & NLP:** Prompt Engineering, In-Context Learning / Full-Corpus Prompt Injection, Semantic Embeddings, System Prompt Constraints, Hallucination Guardrails, Model Context Protocol (MCP)
* **Backend & Orchestration:** Node.js, Express, Server-Sent Events (SSE), API Proxying & Integration (Dovetail, Anthropic, OpenAI), MCP Server Orchestration
* **Frontend Frameworks:** React (Vite)
* **Agentic Tooling & AI-Assisted Prototyping:** Cursor, Claude Code, Google Antigravity (leveraged for high-velocity prototyping, automated testing, and development orchestration)
* **Design Philosophy:** Human-in-the-Loop AI design, zero-dependency performance, minimalist/responsive frontend interfaces

---
*Feel free to reach out if you're interested in AI-UX research patterns, AI-assisted qualitative research systems, or human-AI collaboration!* 🚀
