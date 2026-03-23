# Quick Start: Claude Cowork

This guide walks you through setting up and using the Enterprise IT Navigator Simulation with Claude Cowork — the simplest access path, requiring no Git installation, no terminal, no command line, and no extensions. Everything happens through a chat interface on your desktop.

This path requires a **Claude Pro** subscription ($20/month). No other software is required.

---

## Prerequisites

| Prerequisite                | Details                                                                                      |
| --------------------------- | -------------------------------------------------------------------------------------------- |
| **Claude Pro subscription** | Sign up at [claude.ai](https://claude.ai/) — $20/month; cancel anytime                       |
| **Claude desktop app**      | Download at [claude.ai/download](https://claude.ai/download) — available for Mac and Windows |
| **Cowork mode**             | Enabled within the Claude desktop app (see Step 2)                                           |
| **Project Coach ZIP file**  | Download from GitHub (see Step 3)                                                            |

You do **not** need Git, VS Code, Python, Node.js, or any command-line tools.

---

## Step 1: Get Claude Pro

1. Go to [https://claude.ai/](https://claude.ai/).
2. Create an account or sign in.
3. Subscribe to Claude Pro ($20/month). This gives you access to the Claude desktop app with Cowork mode.

---

## Step 2: Install the Claude Desktop App and Enable Cowork

1. Go to [https://claude.ai/download](https://claude.ai/download) and download the desktop app for your operating system (Mac or Windows).
2. Install and launch the app.
3. Sign in with your Claude Pro account.
4. Enable **Cowork mode** — you should see a folder icon or "Select a folder" option in the interface. Cowork gives Claude direct access to a folder on your computer so it can read and write files on your behalf.

> If you do not see the Cowork option, check that your Claude Pro subscription is active and that you have the latest version of the desktop app.

---

## Step 3: Download the Repo and Create Your Working Folder

### Download the ZIP

1. Go to https://github.com/RSilverAU/ITEC-617-Digital-Transformation-Project-Coach-20260322.
2. Click the green **"Code"** button near the top right.
3. Select **"Download ZIP"**.
4. Save the ZIP file somewhere you can find it (Desktop or Downloads folder).

> You do **not** need to create a GitHub account or repository for this step. You are simply downloading the files.

### Select a Working Folder in Cowork

In the Claude desktop app, select or create a local folder to use as your working directory. This is where Claude will extract the repo and where all your work will be saved.

**Important**: Choose a location that is **not** automatically synced to OneDrive or iCloud. These cloud sync services require additional login steps that can interfere with how Cowork accesses files. A local folder works best — for example:

- `**C:\Users\*<YourName>*\Desktop\ITEC-617\Project Coach**` (Windows, assuming your desktop is not synced with OneDrive)
- `**/Users/YourName/Documents/ITEC-617/Project Coach**` (Mac, outside iCloud Drive)

You can back up your finished outputs to OneDrive or Google Drive manually after each session.

### Extract the Repo

In the Cowork chat, type the following and drag your ZIP file into the chat:

> *"Extract this zip file into a new folder called [YourTeamName]-Project-Coach inside my selected folder."*

Claude will extract the files and confirm when complete. You should see folders named `primer/`, `rubrics/`, `student-workspace/`, and files like `README.md` and `CLAUDE.md`.

---

## Step 4: Drop In Your Prior Assignment Files

If you have completed earlier assignments (Team Charter, Industry/Company selection write-up, Technology Selection, Draft Presentation(s), ROI Analysis, OCM AssessmentTeam Charter, Industry/Company write-up, etc.), drop copies of your deliverables into `student-workspace/source-docs/` first. You can also drag your files into the Cowork chat and say:

> *"Please copy these files into student-workspace/source-docs/"*

Claude will move them into the right location inside your Project Coach folder. The setup assistant will then extract context from them in the next step.

Then use the interactive setup:

- Say *"Please run setup-project"* in the Cowork chat

Claude will move them into the right location inside your Project Coach folder. The setup assistant will then extract context from them in the next step. 

The AI detects your current assignment milestone, extracts context from any source documents you provided, and adapts its questions to your stage. 

Alternatively, open `student-workspace/project-brief.md` and complete every section manually. The more detail you provide, the better the executive feedback.*

---

## Step 5: Fill In Your Project Brief

The simulation uses your project brief to provide relevant, specific feedback. The more detail you provide, the more challenging and useful the executive consultations will be.

### Option A: Interactive Setup (Recommended)

In the Cowork chat, type:

> *"Please run setup-project."*

Claude will read the setup-project skill file and walk you through your project brief section by section. It will:

- Detect your current assignment milestone and adapt its questions to your stage
- Extract content from any source documents you dropped in during Step 4, asking you to confirm rather than re-enter what you already submitted
- Write your completed `student-workspace/project-brief.md` when done
- Review the brief for quality and flag vague or missing areas
- For Assignment 5 and 6 work, also fill in `student-workspace/roi-summary.md` and `student-workspace/ocm-assessment.md`

This takes about 10–15 minutes and sets up everything the executives need to challenge you effectively.

### Option B: Manual Editing

If you prefer to fill in the brief yourself, ask Claude to open `student-workspace/project-brief.md` and complete every section:

- **Team Information**: Team name, member names, date
- **Target Company**: Company name, industry, business unit, size
- **Business Problem**: The specific challenge or opportunity (use data)
- **Proposed Technology Solution**: What technology and how it addresses the problem
- **Primary Benefit Type**: Select one category
- **Proposed Timeline**: Pilot duration and key milestones
- **Initial Financial Estimate**: Pilot cost, expected ROI, funding source
- **Key Risks**: Top 3–5 identified risks
- **Stakeholders**: Affected groups and their concerns
- **Additional Notes**: Any other context relevant to your proposal

---

## Step 6: Consult Executive Personas

Start the simulation by telling Claude which executive you want to consult. Each persona will introduce themselves, read your project brief, and challenge you from their specific C-suite perspective.

| Say this in the chat          | Executive                         | Focus Areas                                      |
| ----------------------------- | --------------------------------- | ------------------------------------------------ |
| *"Please act as the CIO"*     | Jordan Chen, CIO                  | IT strategy, governance, enterprise architecture |
| *"Please act as the CFO"*     | Robert Okafor, CFO                | Financial analysis, ROI, TCO, budget impact      |
| *"Please act as the CISO"*    | Anika Patel, CISO                 | Cybersecurity, risk, privacy, compliance         |
| *"Please act as the COO"*     | Maria Santos, COO                 | Operations, implementation, pilot design         |
| *"Please act as the CHRO"*    | David Washington, CHRO            | Change management, people, culture               |
| *"Please act as the CTO"*     | Priya Ramanathan, CTO             | Technology, innovation, architecture             |
| *"Please act as the CDO"*     | Sarah Kim, CDO                    | Data strategy, governance, AI ethics             |
| *"Please act as Legal"*       | Jonathan Shapiro, General Counsel | Regulatory, IP, contract risk, privacy law       |
| *"Please act as Procurement"* | Lisa Fernandez, VP Procurement    | Vendor strategy, SLAs, contract negotiation      |

**Start with CFO, CIO, and CISO** — these three are mandatory in every session. Add others based on your project's specific vulnerabilities.

**During each consultation:**

- Respond to the executive's questions with specifics, numbers, and evidence
- Ask them to push harder on areas where you feel uncertain
- Take note of any frameworks they reference (e.g., Kraljic Matrix, NIST CSF, TCO lifecycle)
- After the conversation, update your project brief with new insights

> **Tip**: Claude reads the executive's skill file and follows their behavioral instructions. You don't need exact commands — plain English like *"Act as the CFO and challenge my financials"* works the same as a formal slash command.

---

## Step 7: Evaluate Your Proposal

After consulting 3–4 executive personas, ask Claude to score your proposal:

> *"Please evaluate my proposal."*

Claude will:

- Score your proposal across all 9 rubric dimensions (1–5 scale)
- Calculate your composite weighted readiness score
- Determine your readiness level (Ready to Present, Nearly Ready, Making Progress, Early Stage, or Needs Rethinking)
- Highlight your top 3 strengths and top 3 gaps
- Recommend which personas to consult next based on your lowest-scoring areas

Run `/evaluate` after every 2–3 persona consultations to track improvement and know where to focus next.

---

## Step 8: Get Slide-by-Slide Presentation Feedback

Once you have a draft PowerPoint, Claude can read your slides directly and provide executive-perspective feedback.

1. Drag your `.pptx` or `.pdf` file into the Cowork chat and say:
   
   > *"Please save a copy of this to student-workspace/slides/"*
   
   Keep your master file in a separate safe location (OneDrive, Google Drive) — never rely on the simulation copy as your only version.

2. Ask for feedback from a specific executive:
   
   > *"Please act as the CFO and give me slide-by-slide feedback on my presentation."*
   
   Claude will read the slides and provide specific, targeted comments on each one — which slides are strong, which need work, and what's missing from your argument.

3. For a full panel perspective:
   
   > *"Please give me slide-by-slide feedback from the CFO, CIO, and CISO."*

---

## Step 9: Practice Mock Q&A

This simulates the 2–3 minute Q&A session with industry judges after your real presentation.

1. Fill in `student-workspace/presentation-notes.md` with your slide-by-slide talking points (optional but helps Claude focus its questions).

2. In the chat, type:
   
   > *"Please run presentation-prep."*
   
   Claude will simulate a panel of industry judges and:
   
   - Ask 5–7 tough, realistic questions focused on your weakest areas
   - Challenge your financial numbers, technical decisions, security posture, and change management approach
   - Provide feedback after each of your responses
   - Deliver a debrief at the end covering what went well and what to improve

---

## Working as a Team

Claude Cowork runs on one person's computer at a time. Use one of these collaboration models:

### Option 1: Simulation Lead + Shared Cloud Folder (Recommended)

Designate one team member as the **Simulation Lead** who runs all Claude sessions locally. After each session, they copy updated workspace files (`project-brief.md`, `roi-summary.md`, `ocm-assessment.md`, and any generated Word documents) to a shared team folder on OneDrive, Google Drive, or SharePoint. Other teammates review outputs and send corrections back to the Lead.

**Keep the Project Coach working folder local** on the Simulation Lead's machine (not in OneDrive/iCloud). Only copy finished outputs to the shared team folder.

To hand off to a different Simulation Lead: copy the entire Project Coach folder to the new Lead's computer and have them open Cowork and select that folder. The workspace files carry all prior context — Claude picks up exactly where you left off.

### Option 2: GitHub Desktop Sync

For teams who want full version history and frictionless handoffs, use **GitHub Desktop** — a free GUI tool requiring no command-line experience.

1. One team member creates a **private GitHub repository** and invites all teammates as collaborators
2. Each team member installs [GitHub Desktop](https://desktop.github.com/) (free) and clones the repository locally
3. Point Claude Cowork at the cloned local folder
4. **After each session**: open GitHub Desktop → write a short commit note → click "Commit to main" → click "Push origin"
5. **Before each session**: open GitHub Desktop → click "Fetch origin" → click "Pull"

This gives your team full version history and lets any member take over as Simulation Lead without manual file transfers. Initial setup takes 30–45 minutes.

| Approach                              | Setup               | Ongoing effort                 | Version history |
| ------------------------------------- | ------------------- | ------------------------------ | --------------- |
| Simulation Lead + shared cloud folder | Near zero           | Copy outputs after sessions    | None            |
| GitHub Desktop sync                   | 30–45 min, one-time | 2 clicks before/after sessions | Full            |

---

## Tips

- **Start early and iterate.** The simulation is most valuable when you use it across multiple sessions as your project develops — not in one sitting the night before April 27.
- **Be specific.** Vague answers get vague feedback. If you say "we expect significant cost savings," the CFO will ask "how much, exactly?" Come with numbers.
- **Update your brief after every consultation.** Claude evaluates what you have written, not what you told it verbally. Keep `project-brief.md` current.
- **Document your sessions.** At the start of any session, say: *"Please create a markdown file to document what we do in this chat and continue to update it as we proceed."* Claude maintains a running log useful for catching up teammates or continuing across sessions.
- **Study the primer before consultations.** The `primer/` directory has 16 reference sections covering the frameworks executives will cite. Reading the relevant sections beforehand helps you engage at a higher level.
- **Consult all three mandatory executives.** CFO, CIO, and CISO must be consulted before your final evaluation run. Don't skip them.
- **Use plain English.** You don't need exact commands. "Run setup-project," "Act as the CFO," "Evaluate my proposal," and "Practice Q&A" all work — Claude reads the skill files and follows their instructions.

---

## Troubleshooting

| Problem                                      | Solution                                                                                                                                                                                                           |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Cowork can't access files                    | Make sure the working folder is **not** synced to OneDrive or iCloud. Move it to a local path and re-select it in Cowork                                                                                           |
| Claude doesn't recognize "run setup-project" | Make sure Claude has access to your Project Coach folder and can see the `.claude/skills/` directory inside it. Try: *"Please read the file at .claude/skills/setup-project/SKILL.md and follow its instructions"* |
| Claude says it can't find the project brief  | Say: *"Please read student-workspace/project-brief.md"* — this reorients Claude to your workspace                                                                                                                  |
| Session lost context between chats           | Workspace files persist between sessions. At the start of a new chat, say: *"Please read student-workspace/project-brief.md and student-workspace/roi-summary.md to catch up on our project"*                      |
| Two team members edited the same file        | If using GitHub Desktop, a merge conflict may appear. Open the file, keep the correct version of each section, delete the conflict markers (`<<<`, `===`, `>>>`), save, and commit                                 |
| Claude gives generic feedback                | Your project brief likely has placeholder or vague content. Run setup-project again or manually fill in every section with specific numbers, names, and evidence                                                   |
| Can't find Cowork mode in the app            | Check that you have the latest version of the Claude desktop app and an active Claude Pro subscription. Cowork is a desktop-only feature                                                                           |

Still stuck? Ask your instructor or TA for help.
