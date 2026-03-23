# ITEC-617 Digital Transformation Project Coach

An AI-powered simulation that helps you prepare your Digital Transformation (DT) team project presentation by challenging you from multiple executive perspectives.

Built for **ITEC-617: Information and Technology** at American University's Kogod School of Business.

> **<mark>Updated: March 21, 2026** — A third access path has been added: **Claude Cowork** (Path C). This is the recommended path for students who want the simplest setup with no command-line tools, no Git installation, and no coding required. See "Your Path and What You Need" for an explanation and "Getting Started" for where to find the QUICKSTART guide.</mark>

---

## What It Does

You propose a business case for a pilot application of emerging technology. This simulation lets you:

1. **Consult 9 executive personas** who challenge your proposal from their domain perspective
2. **Get scored on 9 rubric dimensions** (45 criteria) aligned to what industry judges evaluate
3. **Track progress** across multiple evaluations with improvement metrics
4. **Practice mock Q&A** with a simulated judge panel targeting your weakest areas
5. **Iterate and improve** with prioritized, actionable recommendations

All personas incorporate insights from **4 years of industry judge feedback** (2021-2024), coaching you on the 10 recurring themes that judges consistently evaluate.

All personas and evaluations are grounded in the [Enterprise IT Primer](https://leifulstrup.github.io/enterprise-it-primer/) course content.

---

## The Executive Personas

| Persona             | Name             | Focus Areas                                      |
| ------------------- | ---------------- | ------------------------------------------------ |
| **CIO**             | Jordan Chen      | IT strategy, governance, enterprise architecture |
| **CISO**            | Anika Patel      | Cybersecurity, risk, privacy, compliance         |
| **CFO**             | Robert Okafor    | Financial analysis, ROI, TCO, budget impact      |
| **COO**             | Maria Santos     | Operations, implementation, pilot design         |
| **CHRO**            | David Washington | Change management, people, culture               |
| **CTO**             | Priya Ramanathan | Technology, innovation, architecture             |
| **CDO**             | Sarah Kim        | Data strategy, governance, AI ethics             |
| **General Counsel** | Jonathan Shapiro | Legal, regulatory, IP, compliance                |
| **VP Procurement**  | Lisa Fernandez   | Vendor strategy, contracts, negotiation          |

Start with **CFO, CIO, and CISO** in every session — these three are mandatory. Add others based on your project's specific needs.

---

## Your Path and What You Need

Choose your path from one of the three below:

- **<u>Path A</u>: VS Code + GitHub Copilot**. This is recommended for students who are Copilot users, have a [GitHub Education](https://education.github.com/) account (free Copilot Pro) and may have technical comfort.

- **<u>Path B</u>: Claude Code CLI**. This is best for students with a [Claude Pro](https://claude.ai/) subscription <u>and </u>who are comfortable with a terminal.

- **<u>Path C:</u> Claude Cowork** requires the least setup — no Git, no VS Code, no command line. It also requires a [Claude Pro](https://claude.ai/) subscription. Claude Cowork is a desktop AI tool that gives Claude direct access to a folder on your computer. You interact entirely through a chat interface. Claude reads the skill files in this repository and replicates the full simulation behavior conversationally.

The following table presents what is required, depending on your path:

| Tool                             | Path A: <br/>VS Code + GitHub Copilot | Path B:<br/>Claude Code CLI | Path C:<br/>Claude Cowork |
| -------------------------------- | ------------------------------------- | --------------------------- | ------------------------- |
| Git                              | Required                              | Required                    | Not needed                |
| VS Code                          | Required                              | Required                    | Not needed                |
| GitHub Copilot                   | Required                              | —                           | Not needed                |
| Claude Code (CLI)                | —                                     | Required                    | Not needed                |
| **Claude Cowork (desktop app)**  | —                                     | —                           | **Required**              |
| Claude Pro subscription ($20/mo) | —                                     | Required                    | Required                  |
| GitHub Education account (free)  | Recommended                           | —                           | Optional                  |

You do **not** need to know how to code on any path. The AI assistants handle all the technical work — you focus on your business case.

---

## Getting Started

All setup instructions, including how to download the repository and collaborate as a team, are in the QUICKSTART documents for the path you have selected:

| Path       | Tool                     | Best for                                                                                  | Setup guide                                                |
| ---------- | ------------------------ | ----------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| **Path A** | VS Code + GitHub Copilot | Students with GitHub Education (free Copilot Pro)                                         | [QUICKSTART-COPILOT.md](QUICKSTART-COPILOT.md)             |
| **Path B** | Claude Code (CLI)        | Students with Claude Pro who are comfortable with a terminal                              | [QUICKSTART-CLAUDE-CODE.md](QUICKSTART-CLAUDE-CODE.md)     |
| **Path C** | Claude Cowork (desktop)  | Students with Claude Pro who want the simplest setup — no Git, no terminal, no extensions | [QUICKSTART-CLAUDE-COWORK.md](QUICKSTART-CLAUDE-COWORK.md) |

---

## Start Using the Coach

See the appropriate quickstart guide in the table above for your chosen path. All setup instructions — including how to download the repository, fill in your project brief, and collaborate as a team — are in those documents.

For a comprehensive overview of the simulation workflow, rubric dimensions, and tips for all three paths, see **[STUDENT-GUIDE.md](STUDENT-GUIDE.md)**.

---

## Working as a Team

All three paths are designed for one person to run the AI session at a time. Choose a collaboration model that fits your team:

### Option 1: Simulation Lead + Shared Cloud Folder (Recommended for most teams)

Designate one team member as the **Simulation Lead** who runs Claude sessions on their local machine. After each session, they copy updated workspace files (`project-brief.md`, `roi-summary.md`, `ocm-assessment.md`, and generated Word documents) to a shared team folder on OneDrive, Google Drive, or SharePoint. Other team members review outputs and feed corrections back to the Lead.

To hand off to a new Lead: copy the entire Project Coach folder to the new Lead's computer and have them open Cowork (or VS Code) and select that folder. The workspace files carry all prior session context.

**IMPORTANT NOTE for Path C users**: Keep the working folder local (not synced to OneDrive/iCloud). Only copy finished outputs to the shared folder.

### Option 2: GitHub Desktop Sync (For teams who want version history)

Any team member can sync the working folder with a shared private GitHub repository using **GitHub Desktop** — a free GUI tool that requires no command-line knowledge.

1. One member creates a private GitHub repo and invites teammates as collaborators
2. Each member installs [GitHub Desktop](https://desktop.github.com/) and clones the repo locally
3. Point Claude Cowork (or VS Code) at the cloned local folder
4. After each session: open GitHub Desktop → commit changes → click "Push origin"
5. Before each session: open GitHub Desktop → "Fetch origin" → "Pull"

This gives your team full version history and lets any member take over as Simulation Lead without manual file transfers. Setup takes 30–45 minutes one time.

| Approach                              | Setup               | Ongoing effort                 | Version history |
| ------------------------------------- | ------------------- | ------------------------------ | --------------- |
| Simulation Lead + shared cloud folder | Near zero           | Copy outputs after sessions    | None            |
| GitHub Desktop sync                   | 30–45 min, one-time | 2 clicks before/after sessions | Full            |

---

## Evaluation Rubric

Proposals are scored across 9 weighted dimensions:

| Dimension               | Weight | Key Questions                                                  |
| ----------------------- | ------ | -------------------------------------------------------------- |
| Business Case Strength  | 20%    | Is the problem clear? Is there a compelling value proposition? |
| Financial Analysis      | 15%    | Is the ROI credible? Is TCO fully accounted for?               |
| Implementation Strategy | 15%    | Is the pilot well-scoped? Is the timeline realistic?           |
| Technology Selection    | 10%    | Is the tech mature enough? Were alternatives considered?       |
| Risk & Security         | 10%    | Are threats identified? Is privacy addressed?                  |
| Change Management       | 10%    | Are stakeholders mapped? Is there a training plan?             |
| Presentation Readiness  | 10%    | Is the narrative compelling? Can the team handle Q&A?          |
| Data & Analytics        | 5%     | Are data requirements clear? Are ethics considered?            |
| Vendor Strategy         | 5%     | Is vendor lock-in mitigated? Are SLAs defined?                 |

**Readiness Levels**: Ready to Present (90–100%) | Nearly Ready (75–89%) | Making Progress (60–74%) | Early Stage (40–59%) | Needs Rethinking (0–39%)

---

## Repository Structure

```
ITEC-617-Digital-Transformation-Project-Coach/
├── primer/                    # 16 reference sections (15 primer + judge advice)
├── rubrics/                   # 9 evaluation dimensions (45 criteria)
├── student-workspace/         # Your working directory
│   ├── project-brief.md       #   ← Fill this in first
│   ├── presentation-notes.md  #   Slide-by-slide notes template
│   ├── roi-summary.md         #   ROI analysis template (Assignment 5)
│   ├── ocm-assessment.md      #   OCM assessment template (Assignment 6)
│   ├── source-docs/           #   Drop prior assignment deliverables here
│   │   └── presentation-support/  #   AI-generated defense materials
│   ├── slides/                #   Place your .pptx and .pdf here
│   └── extracted/             #   Auto-generated by extract_presentation.py
├── scripts/
│   └── validate_markdown_links.py
├── extract_presentation.py    # Extracts .pptx content for AI analysis
├── .github/
│   ├── agents/                # 9 Copilot persona agents (@cio, @cfo, etc.)
│   ├── prompts/               # 5 Copilot prompt templates
│   └── copilot-instructions.md
├── .claude/
│   └── skills/                # 12 Claude Code skills (/cio, /evaluate, /setup-project, etc.)
├── STUDENT-GUIDE.md              # Comprehensive student guide (all paths)
├── QUICKSTART-COPILOT.md         # Path A: VS Code + Copilot setup
├── QUICKSTART-CLAUDE-CODE.md     # Path B: Claude Code setup
├── QUICKSTART-CLAUDE-COWORK.md   # Path C: Claude Cowork setup
├── README.md                     # This file
└── CLAUDE.md                     # Claude Code context configuration
```

---

## Grounding Content

All simulation content is grounded in the **[Enterprise IT Primer](https://leifulstrup.github.io/enterprise-it-primer/)**, covering:

- **Governance**: IT governance frameworks, C-suite roles, IT budgeting
- **Technology**: Build vs. buy, cloud computing, enterprise applications, open source
- **Risk & Security**: Cybersecurity, data governance, shadow IT
- **Transformation**: Digital transformation, AI & emerging tech, innovation management
- **Management**: Vendor management, project management

---

## Course Context

- **Course**: ITEC-617 Information and Technology (MBA, 1.5 credits)
- **Project**: Teams present a business case for a pilot application of emerging technology
- **Format**: 10-minute presentation + 2-3 minutes Q&A to industry judges
- **Date**: April 27, 2026
- **Weight**: 50% of final grade

---

## Markdown Link Check

This repo includes a link validation tool that checks all internal markdown links are valid.

**VS Code**: Open the Command Palette → **Tasks: Run Task** → **"Validate Markdown Links"**

**CLI**:

```bash
uv run scripts/validate_markdown_links.py --root .
```

**CI**: Link validation runs automatically on every push to `main` and on all pull requests.

---

## Troubleshooting

| Problem                               | Solution                                                                                                                                                                                                |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git: command not found`              | Install Git from [git-scm.com/downloads](https://git-scm.com/downloads), then restart your terminal                                                                                                     |
| `uv: command not found`               | Install uv from [docs.astral.sh/uv](https://docs.astral.sh/uv/getting-started/installation/), then restart your terminal                                                                                |
| `python: command not found`           | Install Python from [python.org/downloads](https://www.python.org/downloads/). On Mac, try `python3` instead of `python`                                                                                |
| `code: command not found`             | In VS Code: press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows), type "shell command", select "Install 'code' command in PATH"                                                                        |
| Copilot not responding to `@cio`      | Make sure GitHub Copilot Chat extension is installed and you're signed in with a GitHub Education account                                                                                               |
| Claude Code not recognizing `/cio`    | Make sure you opened the project folder (not a parent folder) in VS Code or navigated to it in the CLI                                                                                                  |
| `extract_presentation.py` fails       | Run as `uv run extract_presentation.py` (not `python extract_presentation.py`). Check Python 3.12+ and uv are installed                                                                                 |
| Cowork can't access files             | Make sure the working folder is **not** synced to OneDrive or iCloud. Move it to a local path (e.g., Desktop or a non-synced Documents subfolder) and re-select it in Cowork                            |
| Cowork session lost context           | Prior workspace files persist between sessions — Claude reads them at the start of each new chat. If context seems missing, tell Claude: *"Please read student-workspace/project-brief.md to catch up"* |
| Two team members edited the same file | If using GitHub Desktop, you may see a merge conflict. Open the conflicted file, keep the correct version of each section, delete the conflict markers (`<<<`, `===`, `>>>`), save, and commit          |

Still stuck? Ask your instructor or TA for help.

---

## License

This project is licensed under the [MIT License](LICENSE). It is for educational use within ITEC-617 at American University's Kogod School of Business.
