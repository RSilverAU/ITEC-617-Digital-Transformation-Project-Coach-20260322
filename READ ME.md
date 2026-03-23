# ITEC-617 Digital Transformation Project Coach

An AI-powered simulation that helps you prepare your Digital Transformation (DT) team project presentation by challenging you from multiple executive perspectives.

Built for **ITEC-617: Information and Technology** at American University's Kogod School of Business.

> **Updated: March 21, 2026** — A third access path has been added: **Claude Cowork** (Path C). This is the recommended path for students who want the simplest setup with no command-line tools, no Git installation, and no coding required. See [Step 3](#step-3-choose-your-ai-assistant-path) and the companion [Student Guide Word document](Student%20Guide%20-%20Using%20Claude%20Cowork%20with%20Project%20Coach%20(v1.3).docx) for full instructions.

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

| Persona | Name | Focus Areas |
|---------|------|-------------|
| **CIO** | Jordan Chen | IT strategy, governance, enterprise architecture |
| **CISO** | Anika Patel | Cybersecurity, risk, privacy, compliance |
| **CFO** | Robert Okafor | Financial analysis, ROI, TCO, budget impact |
| **COO** | Maria Santos | Operations, implementation, pilot design |
| **CHRO** | David Washington | Change management, people, culture |
| **CTO** | Priya Ramanathan | Technology, innovation, architecture |
| **CDO** | Sarah Kim | Data strategy, governance, AI ethics |
| **General Counsel** | Jonathan Shapiro | Legal, regulatory, IP, compliance |
| **VP Procurement** | Lisa Fernandez | Vendor strategy, contracts, negotiation |

Start with **CFO, CIO, and CISO** in every session — these three are mandatory. Add others based on your project's specific needs.

---

## What You Need

Choose your path below. **Path C (Claude Cowork)** requires the least setup — no Git, no VS Code, no command line.

| Tool | Path A | Path B | Path C |
|------|--------|--------|--------|
| Git | Required | Required | Not needed |
| VS Code | Required | Required | Not needed |
| GitHub Copilot | Required | — | Not needed |
| Claude Code (CLI) | — | Required | Not needed |
| **Claude Cowork (desktop app)** | — | — | **Required** |
| Claude Pro subscription ($20/mo) | — | Required | Required |
| GitHub Education account (free) | Recommended | — | Optional |

You do **not** need to know how to code on any path. The AI assistants handle all the technical work — you focus on your business case.

---

## Getting Started

### Step 1: Download the repository

Go to [github.com/leifulstrup/ITEC-617-Digital-Transformation-Project-Coach](https://github.com/leifulstrup/ITEC-617-Digital-Transformation-Project-Coach).

- **Path A or B users**: Click the green **"Use this template"** button and create a private repo for your team (see full instructions below).
- **Path C (Cowork) users**: Click the green **"Code"** button and select **"Download ZIP"**. Save it to your Desktop or Downloads folder. You will extract it using Claude Cowork in Step 3.

### Step 2: (Path A & B only) Create your team's copy of this repo

Each team creates their own private copy using GitHub's template feature.

1. Go to the repo URL above
2. Click the green **"Use this template"** button → **"Create a new repository"**
3. Name your repo (e.g., `Team-Name-DT-Project`) and set visibility to **Private**
4. Click **"Create repository"**

Then open a terminal and clone your new repo:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
code .
```

This downloads your team's project files and opens them in VS Code.

> **Path C users skip this step entirely.** Claude Cowork will extract the ZIP file for you.

### Step 3: Choose your AI assistant path

Pick **one** of these three paths:

---

#### Path A: VS Code + GitHub Copilot (Recommended for Copilot users)

Best for students with a [GitHub Education](https://education.github.com/) account (free Copilot Pro).

1. Install the GitHub Copilot extension in VS Code
2. Open Copilot Chat and use `@cio`, `@cfo`, `@ciso`, etc. to consult personas
3. Use prompt templates (`/setup-project`, `/start-simulation`, `/evaluate-proposal`, `/presentation-prep`)

See **[QUICKSTART-COPILOT.md](QUICKSTART-COPILOT.md)** for full setup instructions.

---

#### Path B: Claude Code CLI

Best for students with a [Claude Pro](https://claude.ai/) subscription who are comfortable with a terminal.

1. Install Claude Code and open this repo
2. Use slash commands: `/cio`, `/cfo`, `/ciso`, etc. to consult personas
3. Use `/setup-project` to fill in your brief, `/evaluate` for scoring, `/presentation-prep` for mock Q&A

See **[QUICKSTART-CLAUDE-CODE.md](QUICKSTART-CLAUDE-CODE.md)** for full setup instructions.

---

#### Path C: Claude Cowork *(New — No Setup Required)*

Best for students with a [Claude Pro](https://claude.ai/) subscription who want the simplest possible experience — no Git, no terminal, no extensions.

**What it is**: Claude Cowork is a desktop AI tool that gives Claude direct access to a folder on your computer. You interact entirely through a chat interface. Claude reads the skill files in this repository and replicates the full simulation behavior conversationally.

**Quick setup**:

1. Download the ZIP file from GitHub (green "Code" button → "Download ZIP")
2. Launch the Claude desktop app and enable Cowork mode
3. Select or create a local working folder — **important: choose a location not synced to OneDrive or iCloud** (these services require additional login steps that interfere with file access; back up finished outputs to cloud storage separately)
4. Tell Claude: *"Extract this zip file into a new folder called [YourTeamName]-Project-Coach inside my selected folder"* and drag the ZIP into the chat
5. Drop your prior assignment files (PDFs, Word docs) into the chat and say: *"Please copy these into student-workspace/source-docs/"*
6. Tell Claude: *"Please run setup-project"* — Claude reads the skill file and walks you through building your project brief
7. Say *"Please act as the CFO"*, *"Please act as the CIO"*, etc. to consult personas
8. Say *"Please evaluate my proposal"* after 3–4 consultations

**Pro tip**: At the start of any session, say: *"Please create a markdown file to document what we do in this chat and continue to update it as we proceed."* Claude will maintain a running log you can share with teammates.

See the **[Student Guide Word document](Student%20Guide%20-%20Using%20Claude%20Cowork%20with%20Project%20Coach%20(v1.3).docx)** for complete step-by-step instructions, including team collaboration options and presentation feedback.

---

### Step 4: Fill in your project brief

If you have completed earlier assignments (Team Charter, Industry/Company write-up, etc.), drop copies of your deliverables into `student-workspace/source-docs/` first.

Then use the interactive setup:
- **Path A**: Select the **setup-project** prompt in Copilot Chat
- **Path B**: Run `/setup-project` in Claude Code
- **Path C**: Say *"Please run setup-project"* in the Cowork chat

The AI detects your current assignment milestone, extracts context from any source documents you provided, and adapts its questions to your stage. It writes the brief for you and reviews it for quality.

Companion templates: `student-workspace/roi-summary.md` (Assignment 5) and `student-workspace/ocm-assessment.md` (Assignment 6).

Alternatively, open `student-workspace/project-brief.md` and complete every section manually. The more detail you provide, the better the executive feedback.

### Presentation Feedback

Once you have draft slides, the simulation provides **slide-by-slide feedback**:

1. Place a **copy** of your `.pptx` or `.pdf` in `student-workspace/slides/`
2. For Path A/B users, extract text content for AI analysis:
   ```bash
   uv run extract_presentation.py
   ```
3. **Path B (Claude Code)** and **Path C (Cowork)** users: Claude can read `.pptx` and `.pdf` files directly — skip the extraction step and ask Claude to review your slides directly.

> **Protect your work.** Always keep your original PowerPoint in a separate folder outside this repository (e.g., your Desktop or OneDrive). Save backup copies or use `git commit` to snapshot your work before each AI feedback session.

### Optional: Install Python and uv (Path A/B only)

The `extract_presentation.py` script requires Python and the `uv` package manager.

1. **Install Python 3.12+** from [python.org/downloads](https://www.python.org/downloads/)
2. **Install uv** from [docs.astral.sh/uv/getting-started/installation](https://docs.astral.sh/uv/getting-started/installation/)
3. Verify: `python3 --version` and `uv --version`

---

## Working as a Team

All three paths are designed for one person to run the AI session at a time. Choose a collaboration model that fits your team:

### Option 1: Simulation Lead + Shared Cloud Folder (Recommended for most teams)

Designate one team member as the **Simulation Lead** who runs Claude sessions on their local machine. After each session, they copy updated workspace files (`project-brief.md`, `roi-summary.md`, `ocm-assessment.md`, and generated Word documents) to a shared team folder on OneDrive, Google Drive, or SharePoint. Other team members review outputs and feed corrections back to the Lead.

To hand off to a new Lead: copy the entire Project Coach folder to the new Lead's computer and have them open Cowork (or VS Code) and select that folder. The workspace files carry all prior session context.

**Note for Path C users**: Keep the working folder local (not synced to OneDrive/iCloud). Only copy finished outputs to the shared folder.

### Option 2: GitHub Desktop Sync (For teams who want version history)

Any team member can sync the working folder with a shared private GitHub repository using **GitHub Desktop** — a free GUI tool that requires no command-line knowledge.

1. One member creates a private GitHub repo and invites teammates as collaborators
2. Each member installs [GitHub Desktop](https://desktop.github.com/) and clones the repo locally
3. Point Claude Cowork (or VS Code) at the cloned local folder
4. After each session: open GitHub Desktop → commit changes → click "Push origin"
5. Before each session: open GitHub Desktop → "Fetch origin" → "Pull"

This gives your team full version history and lets any member take over as Simulation Lead without manual file transfers. Setup takes 30–45 minutes one time.

| Approach | Setup | Ongoing effort | Version history |
|---|---|---|---|
| Simulation Lead + shared cloud folder | Near zero | Copy outputs after sessions | None |
| GitHub Desktop sync | 30–45 min, one-time | 2 clicks before/after sessions | Full |

---

## Evaluation Rubric

Proposals are scored across 9 weighted dimensions:

| Dimension | Weight | Key Questions |
|-----------|--------|---------------|
| Business Case Strength | 20% | Is the problem clear? Is there a compelling value proposition? |
| Financial Analysis | 15% | Is the ROI credible? Is TCO fully accounted for? |
| Implementation Strategy | 15% | Is the pilot well-scoped? Is the timeline realistic? |
| Technology Selection | 10% | Is the tech mature enough? Were alternatives considered? |
| Risk & Security | 10% | Are threats identified? Is privacy addressed? |
| Change Management | 10% | Are stakeholders mapped? Is there a training plan? |
| Presentation Readiness | 10% | Is the narrative compelling? Can the team handle Q&A? |
| Data & Analytics | 5% | Are data requirements clear? Are ethics considered? |
| Vendor Strategy | 5% | Is vendor lock-in mitigated? Are SLAs defined? |

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
├── STUDENT-GUIDE.md           # Comprehensive student guide
├── QUICKSTART-COPILOT.md      # Path A: VS Code + Copilot setup
├── QUICKSTART-CLAUDE-CODE.md  # Path B: Claude Code setup
├── CLAUDE.md                  # Claude Code context configuration
├── UPDATED README (2026-03-21).md  # This file — adds Path C (Cowork)
└── Student Guide - Using Claude Cowork with Project Coach (v1.3).docx
                               # Path C: Full step-by-step Cowork guide
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

| Problem | Solution |
|---------|----------|
| `git: command not found` | Install Git from [git-scm.com/downloads](https://git-scm.com/downloads), then restart your terminal |
| `uv: command not found` | Install uv from [docs.astral.sh/uv](https://docs.astral.sh/uv/getting-started/installation/), then restart your terminal |
| `python: command not found` | Install Python from [python.org/downloads](https://www.python.org/downloads/). On Mac, try `python3` instead of `python` |
| `code: command not found` | In VS Code: press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows), type "shell command", select "Install 'code' command in PATH" |
| Copilot not responding to `@cio` | Make sure GitHub Copilot Chat extension is installed and you're signed in with a GitHub Education account |
| Claude Code not recognizing `/cio` | Make sure you opened the project folder (not a parent folder) in VS Code or navigated to it in the CLI |
| `extract_presentation.py` fails | Run as `uv run extract_presentation.py` (not `python extract_presentation.py`). Check Python 3.12+ and uv are installed |
| Cowork can't access files | Make sure the working folder is **not** synced to OneDrive or iCloud. Move it to a local path (e.g., Desktop or a non-synced Documents subfolder) and re-select it in Cowork |
| Cowork session lost context | Prior workspace files persist between sessions — Claude reads them at the start of each new chat. If context seems missing, tell Claude: *"Please read student-workspace/project-brief.md to catch up"* |
| Two team members edited the same file | If using GitHub Desktop, you may see a merge conflict. Open the conflicted file, keep the correct version of each section, delete the conflict markers (`<<<`, `===`, `>>>`), save, and commit |

Still stuck? Ask your instructor or TA for help.

---

## License

This project is licensed under the [MIT License](LICENSE). It is for educational use within ITEC-617 at American University's Kogod School of Business.
