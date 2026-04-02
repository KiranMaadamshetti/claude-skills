# Claude Skills Collection

### Powerful plugins for Claude AI that supercharge your workflow

[![Claude Compatible](https://img.shields.io/badge/Claude-Skills%20Compatible-blueviolet?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0wIDE4Yy00LjQxIDAtOC0zLjU5LTgtOHMzLjU5LTggOC04IDggMy41OSA4IDgtMy41OSA4LTggOHoiLz48L3N2Zz4=)](https://claude.ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Skills](https://img.shields.io/badge/Skills-2%20Available-orange?style=for-the-badge)](#available-skills)

---

## What Are Claude Skills?

Claude Skills are custom plugins you can install in [Claude.ai](https://claude.ai) that give Claude specialized capabilities. Think of them as expert knowledge packs — when you install a skill, Claude gains deep expertise in that domain and follows proven workflows to deliver professional-grade output.

**No coding required.** Just download a `.skill` file, upload it to Claude, and start using it.

---

## Available Skills

| Skill | What It Does | Download |
|-------|-------------|----------|
| [**Resume Analyser**](#-resume-analyser) | Scores, critiques, and completely rewrites your resume with a professional HTML report | [📥 Download](resume-analyser/resume-analyser.skill) |
| [**Strategy Toolkit**](#-strategy-toolkit) | 10 proven strategic frameworks for business analysis, competitive positioning, and execution | [📥 Download](strategy-toolkit/strategy-toolkit.skill) |

---

## How to Install

### Step 1: Download the `.skill` file
Click the download link above, or go to the skill folder and download the `.skill` file.

### Step 2: Open Claude Settings
Go to [claude.ai](https://claude.ai) → Click your profile icon (bottom-left) → **Settings**

### Step 3: Add the Skill
Navigate to **Profile** → **Skills** → **Add Skill** → Upload the `.skill` file

### Step 4: Start Using
That's it! The skill activates automatically when you ask relevant questions. See each skill's documentation below for example prompts.

> **Note:** Skills require a Claude Pro, Team, or Enterprise subscription.

---

## 📄 Resume Analyser

**An intensive, multi-dimensional resume analyser that scores, critiques, AND rewrites your entire resume.**

### What You Get

Every time you upload a resume, the skill delivers **two outputs**:

1. **Analysis Report (HTML)** — Interactive report with:
   - Overall score out of 100 with letter grade (A+ through F)
   - Radar chart across 10 scoring dimensions
   - Section-by-section critique with severity tags (🔴 Critical, 🟡 Important, 🔵 Minor)
   - Before → After rewrite examples for weak bullets
   - ATS compatibility audit with keyword gap analysis
   - Top 5 priority action plan ranked by interview impact

2. **Revised Resume (Markdown + Copyable)** — A complete rewrite of your entire resume:
   - Every bullet rewritten using the CAR framework (Challenge → Action → Result)
   - Generic objectives replaced with specific professional summaries
   - Skills categorized properly (not a flat list)
   - Outdated sections removed (Declaration, Personal Details)
   - Placeholders marked with `[PLACEHOLDER: ...]` for numbers you need to fill in
   - Copy-to-clipboard button for easy use
   - Print-friendly layout

### The 10 Scoring Dimensions

| Dimension | Weight | What It Measures |
|-----------|--------|------------------|
| Impact & Achievements | 20% | Quantified results, action verbs, CAR framework |
| ATS Compatibility | 15% | Parsability, keywords, formatting |
| Content Relevance | 12% | Signal-to-noise ratio, filler detection |
| Structure & Flow | 10% | Section order, information hierarchy |
| Formatting & Readability | 10% | Consistency, length, whitespace |
| Language & Grammar | 8% | Tense, voice, tone, spelling |
| Skills Presentation | 8% | Categorization, specificity |
| Career Narrative | 7% | Progression, gap handling |
| Digital Presence | 5% | LinkedIn, GitHub, portfolio |
| Compliance & Red Flags | 5% | PII risks, discrimination signals |

### How to Use

Simply upload your resume (PDF, DOCX, or TXT) and say:

```
Review my resume
```

Or be more specific:

```
Analyse my resume and rewrite it for a Senior Product Manager role.
Here's the job description: [paste JD]
```

**More trigger phrases:** `score my resume`, `is my resume ATS-friendly`, `fix my resume`, `improve my CV`, `tailor my resume for [role]`

### Files Included

```
resume-analyser/
├── SKILL.md                         # Core skill instructions
├── references/
│   └── scoring-rubric.md            # Detailed 10-dimension grading criteria
└── scripts/
    └── generate_report.py           # HTML report template generator
```

---

## 🎯 Strategy Toolkit

**10 proven strategic frameworks for business analysis, competitive positioning, strategy execution, and organizational decision-making.**

### The 10 Frameworks

| # | Framework | Author(s) | Best For |
|---|-----------|-----------|----------|
| 1 | **What Is Strategy** | Michael Porter | Defining competitive position, trade-offs, activity fit |
| 2 | **Five Competitive Forces** | Michael Porter | Industry attractiveness analysis |
| 3 | **Blue Ocean Strategy** | Kim & Mauborgne | Finding uncontested market space |
| 4 | **Building Company Vision** | Collins & Porras | Core values, purpose, BHAG |
| 5 | **Business Model Reinvention** | Christensen et al. | Designing how you create and capture value |
| 6 | **Strategy Execution** | Neilson et al. | Fixing decision rights, information flow |
| 7 | **Balanced Scorecard** | Kaplan & Norton | Measuring strategy across 4 perspectives |
| 8 | **Strategic Principles** | Gadiesh & Gilbert | One-phrase strategy for frontline decisions |
| 9 | **Strategy-to-Performance Gap** | Mankins & Steele | 7 rules for closing the execution gap |
| 10 | **RAPID Decision Model** | Rogers & Blenko | Clarifying who Recommends, Agrees, Performs, Inputs, Decides |

### How to Use

**For any strategic question**, just describe your situation:

```
I run a lending company in Tier 2-5 cities in India. We're trying to
scale from 5 branches to 55. Help me build a growth strategy.
```

**Or name specific frameworks:**

```
Do a Five Forces analysis for the Indian micro-lending industry
```

```
Help me find blue ocean opportunities in the home loan market
for small-town borrowers
```

```
Our strategy is good but execution is failing. Diagnose using
the four building blocks framework.
```

```
Build me a Balanced Scorecard for our branch expansion initiative
```

```
Create a RAPID decision map for these 3 decisions that keep
getting stuck in our organization: [list decisions]
```

### Framework Selection Guide

Don't know which framework to use? Just describe your problem:

| Your Problem | Claude Picks |
|-------------|-------------|
| "How should we compete?" | Porter's Strategy + Five Forces |
| "Our market is too crowded" | Blue Ocean + Business Model |
| "What should our company stand for?" | Vision Framework + Strategic Principles |
| "Strategy is fine but results lag" | Execution + Seven Rules + RAPID |
| "How do I measure strategic progress?" | Balanced Scorecard |
| "Should we enter this new market?" | Five Forces + Blue Ocean + Business Model |

### Files Included

```
strategy-toolkit/
├── SKILL.md                              # Core skill instructions + workflow
└── references/
    ├── framework-selector.md             # Decision guide for picking frameworks
    ├── porter-strategy.md                # Porter's What Is Strategy
    ├── five-forces.md                    # Five Competitive Forces
    ├── blue-ocean.md                     # Blue Ocean Strategy
    ├── vision-framework.md               # Building Company Vision (Collins/Porras)
    ├── business-model.md                 # Business Model Reinvention
    ├── strategy-execution.md             # Strategy Execution (Neilson)
    ├── balanced-scorecard.md             # Balanced Scorecard (Kaplan/Norton)
    ├── strategic-principles.md           # Strategic Principles (Gadiesh/Gilbert)
    ├── strategy-performance.md           # Seven Rules (Mankins/Steele)
    └── rapid-decisions.md                # RAPID Decision Model
```

---

## Building Your Own Skills

Want to create your own Claude skill? Here's the basic structure:

```
your-skill/
├── SKILL.md          # Required — YAML frontmatter + instructions
└── references/       # Optional — additional docs Claude reads as needed
```

### SKILL.md Format

```yaml
---
name: your-skill-name
description: >-
  Description of what the skill does and when to trigger it.
  Keep under 1024 characters. No angle brackets.
---

# Your Skill Title

Instructions for Claude go here...
```

### Key Rules
- **name** must be kebab-case (lowercase, hyphens only), max 64 characters
- **description** must be under 1024 characters, no `<` or `>` characters
- Use YAML `>-` block scalar if description contains colons or special characters
- Package as a `.skill` file (ZIP format) with the skill folder inside

---

## Contributing

Found a bug? Have an improvement? Contributions are welcome!

1. Fork this repository
2. Create a branch (`git checkout -b improve-resume-skill`)
3. Make your changes
4. Test by installing the modified `.skill` file in Claude
5. Submit a Pull Request

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

The strategic frameworks referenced in the Strategy Toolkit are the intellectual property of their respective authors (Michael Porter, Clayton Christensen, W. Chan Kim, Robert Kaplan, etc.). The skill files contain original instructional content for applying these frameworks, not reproductions of the source material.



