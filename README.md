
---

# 📰 AI News Summarizer (PDF Export)

A local-first AI-powered RSS news aggregation and summarization tool that transforms curated feeds into structured, printable PDF briefings.

Designed for researchers, builders, and operators who want signal — not noise.

---

## 🚀 What This Project Does

* Aggregates RSS feeds by profile
* Filters and deduplicates articles
* Summarizes content using configurable AI models
* Structures summaries with sources and metadata
* Renders clean HTML reports
* Exports formatted PDF briefings

The goal is simple:
**Turn live feeds into usable intelligence.**

---

## 🧠 How It Works

```text
RSS Feeds
   ↓
Feed Parser
   ↓
Filtering + Deduplication
   ↓
AI Summarization
   ↓
Structured Report Builder
   ↓
HTML Render
   ↓
PDF Export
```

---

## Key Capabilities

### Profiles

* Organize feeds by topic (AI, Health, Research, etc.)
* Switch profiles without changing logic

### Model-Driven Summarization

* Works with local models (via Ollama)
* Cloud-ready (optional)
* Configurable routing and fallback support

### Structured Output

* Headline summaries
* Source tracking
* Clean formatting
* Token-aware generation

### PDF Export

Designed for:

* Daily briefings
* Research snapshots
* Executive summaries
* Archival documentation

---

## 🖨 Example Use Cases

* AI industry morning brief
* Health & biotech scan
* Academic research tracking
* Competitive intelligence digest
* Community newsletter draft

---

## ⚙️ Configuration

### RSS Profiles

Feeds are grouped into profiles:

```json
{
  "AI": [
    "https://example.com/rss",
    "https://anotherfeed.com/rss"
  ]
}
```

Profiles can be modified without changing the summarization engine.

---

### Model Configuration

Example:

```json
{
  "summarizer": "gemma3:12b",
  "fallback": "llama3:8b"
}
```

Supports:

* Local-first inference
* Configurable token limits
* Deterministic settings for reproducibility

---

## 🔒 Local First. Cloud Ready.

* Runs fully local
* No required external APIs
* Cloud models optional
* Designed for consumer hardware

This project is part of a larger modular AI architecture focused on:

* Reproducible pipelines
* Model provenance
* Metric-driven evaluation
* Specialist routing frameworks
* Real-world deployment from download → fine-tune → merge → convert → deploy

The broader engine also powers domain-specific assistants, including chronic health coordination tools built on the same evaluation-driven core.
