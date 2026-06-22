# ResearchAI — Agentic Document & Research Assistant

> An AI-powered research assistant with agentic workflow integration, PDF parsing, multi-model support (Groq + Claude), and 6 specialized research modes. Built for the **Build with AI UAE** hackathon.


## 🔗 Links

- 🌐 **Live Demo:** [your-app.vercel.app](https://your-app.vercel.app)



## ✨ What Is ResearchAI?

ResearchAI is a fully functional AI-powered research and document assistant that runs entirely in the browser. No installation required. It combines:

- **Agentic AI workflow** — every query runs through a 4-step reasoning pipeline (Query Analysis → Retrieval → Synthesis → Formatting)
- **Multiple AI models** — Llama 3.3 70B, Mixtral 8x7B, Gemma 2 9B via Groq (free), and Claude Sonnet 4.6 via Anthropic
- **6 specialized research modes** — each with its own system prompt and behavior
- **4 output formats** — Full response, Key points, Structured report, Academic style
- **PDF parsing** — upload and query any PDF directly in the browser using PDF.js
- **Session stats** — live tracking of queries, tokens, agent steps, and latency

### 1. Key Points Mode — Agentic AI Overview
> **Query:** "What is agentic AI and why does it matter in 2025?"
> **Mode:** Deep Research · **Output:** Key points

The assistant returns a clean bulleted breakdown. Notice the session stats on the right — 4 queries, 16 agent steps, 0.7s average latency — showing the agentic pipeline running efficiently.

<img width="1277" height="689" alt="Screenshot 2026-06-23 at 03 32 36" src="https://github.com/user-attachments/assets/0f09c46a-a93b-4d0f-97f6-1386354abd9b" />


### 2. Key Points Mode — Large Language Models
> **Query:** "Explain how large language models work"
> **Mode:** Deep Research · **Output:** Key points

Demonstrates how the Key Points output format forces the model to return structured bullets only — no prose paragraphs. The response breaks down LLMs into Overview, Key Components (Tokenizer, Embeddings, Encoder, Decoder), all cleanly structured.

<img width="1276" height="711" alt="Screenshot 2026-06-23 at 03 36 41" src="https://github.com/user-attachments/assets/fddd7fb3-196c-439d-a1a0-7333fe6b9ca3" />


### 3. Compare & Contrast — Side-by-Side Table
> **Query:** "Compare Python vs JavaScript for AI development"
> **Mode:** Compare & contrast · **Output:** Full response

The Compare mode generates a fully rendered markdown table with dimensions like Syntax, Libraries, Performance, Data Science, Machine Learning, Community, and Use Cases — exactly what a researcher or developer needs for a quick decision.

<img width="1280" height="712" alt="Screenshot 2026-06-23 at 03 37 33" src="https://github.com/user-attachments/assets/0eec8c33-1161-4275-b183-8577cde4be22" />


### 4. Compare Mode — PDF Document Analysis
> **Source:** Uploaded PDF — "The Agentic AI Attack Surface" whitepaper
> **Mode:** Compare & contrast

Shows the assistant analysing an uploaded research paper and producing a structured summary with key concepts: the Agentic Kill Chain, Agent Identity Graph, and Zero Trust Agent Architecture. Demonstrates the Document Q&A + Compare mode working together on a real academic PDF.
<img width="1280" height="714" alt="Screenshot 2026-06-23 at 03 38 18" src="https://github.com/user-attachments/assets/a089d80e-1656-47d6-9dea-5c91da9f82e0" />


### 5. Summarize Mode — Research Paper TL;DR
> **Source:** Uploaded PDF — "The Agentic AI Attack Surface" whitepaper
> **Mode:** Summarize · **Output:** Full response

The Summarize mode produces a TL;DR followed by structured Key Points. In this example it compressed a full whitepaper into a concise summary covering autonomous AI agents, the Agentic Kill Chain model, and Zero Trust Architecture — all in seconds. Session shows 8 queries and 5.9k estimated tokens.
<img width="1280" height="714" alt="Screenshot 2026-06-23 at 03 38 18" src="https://github.com/user-attachments/assets/a089d80e-1656-47d6-9dea-5c91da9f82e0" />


### 6. Extract Data Mode — Entity & Fact Extraction
> **Query:** "Extract all entities and facts: OpenAI raised $6.6B in October 2024 at a $157B valuation. Sam Altman is CEO. They have 1,800 employees and 200 million weekly active users of ChatGPT."
> **Mode:** Extract data

The Extract mode pulls every named entity (OpenAI, Sam Altman, ChatGPT, Kieran Upadrasta, Cyber AI Systems Inc., Entro Security) with their associated facts — precisely structured, nothing missed. Session: 10 queries, 40 agent steps, 6.9k tokens processed.

<img width="809" height="660" alt="Screenshot 2026-06-23 at 03 52 31" src="https://github.com/user-attachments/assets/e5bc1183-e27c-49e3-832b-ba3b3b31f38a" />


### 7. Structured Report Mode — AI Assistant Market Analysis
> **Query:** "Analyze the competitive landscape of AI assistants in 2025"
> **Mode:** Deep Research · **Output:** Structured report

The Structured Report format enforces a specific output structure: **Executive Summary** → **Key Findings** → **Analysis** → **Gaps & Caveats** → **Takeaway**. This screenshot shows the Executive Summary and Key Findings sections covering Amazon Alexa, Google Assistant, Apple Siri, Microsoft Cortana, and Samsung Bixby — exactly formatted for a professional deliverable.

<img width="1280" height="714" alt="Screenshot 2026-06-23 at 03 36 17" src="https://github.com/user-attachments/assets/57e25a74-7b98-4875-9e44-cb7496ab4079" />


## 🚀 Features

### 6 Research Modes
| Mode | What It Does |
|------|-------------|
| 🔍 **Deep Research** | Multi-step reasoning with source tracing and citations |
| 📄 **Document Q&A** | Ask questions about uploaded PDFs and text files |
| ✂️ **Summarize** | TL;DR + key points + gaps in seconds |
| ⚖️ **Compare & Contrast** | Side-by-side markdown tables with key differences and verdict |
| 🗂 **Extract Data** | Pull entities, statistics, dates, and claims from any text |
| ✍️ **Draft & Write** | Professional drafts with alternative approaches |

### 4 Output Formats
| Format | Output Style |
|--------|-------------|
| **Full response** | Comprehensive prose with markdown headers |
| **Key points** | Bullets only — no prose, no filler |
| **Structured report** | Executive Summary → Key Findings → Analysis → Gaps → Takeaway |
| **Academic style** | Formal register with Abstract, Background, Findings, Discussion, Conclusion |

### AI Models
| Model | Provider | Cost |
|-------|----------|------|
| Llama 3.3 70B | Groq | Free |
| Mixtral 8x7B | Groq | Free |
| Gemma 2 9B | Groq | Free |
| Claude Sonnet 4.6 | Anthropic | Requires Vercel deploy |

### Other Capabilities
- 📕 **PDF upload & parsing** — PDF.js runs entirely in the browser, no server needed
- 🔁 **Agentic workflow trace** — collapsible step-by-step reasoning trace on every response
- 📊 **Live session stats** — queries, estimated tokens, agent steps, avg latency
- 🕒 **Query history** — click any past query to reuse it
- 📋 **Session export** — download the full conversation as `.txt`
- ⚙️ **Toggleable output options** — workflow trace, source tags, markdown rendering

## 🏁 Getting Started

### Option A — Run locally (no installation, free)

1. Download `research-assistant-v3.html`
2. Double-click to open in any browser
3. Get a free Groq API key at [console.groq.com](https://console.groq.com) → **API Keys** → **Create API Key**
4. In the app: click **Stats** tab (right panel) → paste your `gsk_...` key → **Save**
5. Start researching

**No terminal. No npm. No server. Just open and use.**

### Option B — Deploy to Vercel (enables Claude)

See the [Deploy to Vercel](#-deploy-to-vercel) section below.

## 📖 How to Use

### Basic Research
1. Select a mode from the left sidebar (e.g. **Deep Research**)
2. Select an output format from the top tabs (e.g. **Structured report**)
3. Type your question and press **Enter**

### PDF Document Q&A
1. Click **Document Q&A** in the left sidebar
2. Click **Attach** in the top bar → select a PDF
3. Wait for the Docs panel to show the file with page count
4. Ask questions: `Summarize this document` / `What are the key findings?` / `Extract all statistics`

### Switching Models
Click the model name in the top-left (e.g. **Llama 3.3 70B**) to open the model picker and switch between Groq models.


## 🔧 Agentic Workflow

Every response runs through a 4-step agentic pipeline that is visible as a collapsible **Workflow Trace** below each AI response:

Step 1 → Query Analysis      Decompose task, identify mode and output format
Step 2 → Retrieval           Search context, load document content if attached  
Step 3 → Synthesis           Cross-reference, structure the response
Step 4 → Formatting          Apply output format (bullets / structured / academic)

The workflow trace shows each step with a ✓ checkmark and timing — making the agentic reasoning transparent and auditable.

## 🔑 API Keys

| Service | Where to Get | Cost | Usage |
|---------|-------------|------|-------|
| **Groq** | [console.groq.com](https://console.groq.com) → API Keys | Free | 14,400 requests/day |
| **Anthropic** | [console.anthropic.com](https://console.anthropic.com) | Paid | For Claude Sonnet 4.6 |

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML, CSS, JavaScript (zero dependencies) |
| AI — Free | Groq API (Llama 3.3 70B, Mixtral 8x7B, Gemma 2 9B) |
| AI — Paid | Anthropic API (Claude Sonnet 4.6) |
| PDF Parsing | PDF.js v3.11 (runs in browser, no server) |
| Fonts | Inter + JetBrains Mono (Google Fonts) |
| Deployment | Vercel |

---

## 🏆 Hackathon

Built for the **Build with AI UAE** hackathon.

`#Googleantigravity` `#BuildwithAI` `#BwAIUAE`

## 📄 License

MIT — free to use, modify, and deploy.
