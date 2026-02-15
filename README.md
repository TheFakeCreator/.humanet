# Humanet Template

**Official `.humanet/` folder template for documenting ideas on the Humanet platform.**

[![Humanet](https://img.shields.io/badge/Humanet-Template-purple)](https://humanet.dev)

> **Humanet:** GitHub for Ideas + Notion for Structure + Obsidian's Knowledge Graph

This repository contains the standard structure for the `.humanet/` folder that you add to any project to make it a Humanet idea.

---

## 🚀 How to Use This Template

### Option 1: Clone and Copy to Your Project (Recommended)

```bash
# Clone this template repository
git clone https://github.com/humanet/template.git humanet-template

# Copy the entire contents to your project's .humanet folder
cp -r humanet-template/* your-project/.humanet/

# Clean up
rm -rf humanet-template

# Or on Windows PowerShell:
# Copy-Item -Path humanet-template\* -Destination your-project\.humanet\ -Recurse
```

### Option 2: Manual Download

1. Download this repository as ZIP
2. Extract the contents
3. Copy all files to a `.humanet/` folder in your project
4. Fill out the templates

### Option 3: Initialize New Project

```bash
# Create your project directory
mkdir my-idea && cd my-idea
git init

# Clone template directly as .humanet
git clone https://github.com/humanet/template.git .humanet
cd .humanet
rm -rf .git  # Remove template's git history
```

---

## 📂 What's Inside

```
.humanet/  (this repository structure)
├── config.yml                    # Core metadata & lifecycle tracking
├── README.md                     # This file - documentation guide
├── problem_statement.md          # Required: What problem does this solve?
├── idea.md                       # Required: The core concept & approach
├── scope.md                      # Required: Boundaries & success metrics
├── CHANGELOG.md                  # Evolution & version history
├── CONTRIBUTORS.md               # Attribution & roles
├── config.schema.json            # JSON Schema for validation
│
├── diagrams/                     # Visual documentation
│   └── README.md
│
├── research/                     # Supporting materials
│   ├── README.md
│   └── literature-review.md
│
├── discussions/                  # Decision logs & ADRs
│   ├── README.md
│   └── 001-tech-stack-selection.md
│
├── evaluations/                  # AI validation reports (auto-generated)
│   └── README.md
│
└── templates/                    # Reusable templates
    ├── README.md
    ├── decision-record.md
    ├── meeting-notes.md
    └── research-summary.md
```

---

## ✅ Required Files

Every Humanet idea must have these files:

1. **[`config.yml`](./config.yml)** — Metadata, lifecycle status, domains, contributors
2. **[`problem_statement.md`](./problem_statement.md)** — What problem does this solve?
3. **[`idea.md`](./idea.md)** — The core concept and approach
4. **[`scope.md`](./scope.md)** — Boundaries, expectations, success metrics

---

## 📝 Quick Start (15 Minutes)

### Step 1: Update `config.yml` (5 min)

Edit [`config.yml`](./config.yml) with your idea's information:

- Set your idea name and tagline
- Choose 2-5 relevant domains
- Add your GitHub username as maintainer
- Set the repository URL
- Choose a license (default: CC-BY-4.0)

### Step 2: Write Your Core Documentation (10 min)

Fill out the three required documents:

- **[`problem_statement.md`](./problem_statement.md)** — What pain point are you addressing?
- **[`idea.md`](./idea.md)** — What's your solution? How does it work?
- **[`scope.md`](./scope.md)** — What's in scope, out of scope, and how will you measure success?

### Step 3: Commit to Your Repository

```bash
# In your project directory
git add .humanet/
git commit -m "Add Humanet documentation"
git push
```

### Step 4: Register on Humanet

Visit [humanet.dev](https://humanet.dev) to register your idea.

---

## 📊 Lifecycle States

Your idea progresses through these stages:

```
📝 Provisional (30 days)
    ↓
🤖 AI Evaluation
    ↓
├─→ ❌ Needs Refinement
│       ↓
│   Re-evaluation
│       ↓
└─→ ✅ Validated
        ↓
    🚀 Active Development
        ↓
    ├─→ ⏸️ Dormant (paused)
    ├─→ 📦 Archived (completed)
    └─→ 🔄 Deprecated (superseded)
```

Your current status is tracked in [`config.yml`](./config.yml).

---

## 🎨 Optional Enhancements

### Add Visual Documentation

1. Create diagrams with [draw.io](https://draw.io)
2. Save `.drawio` file in `diagrams/`
3. Export as `.png` or `.svg`
4. Embed in your docs: `![Diagram](./diagrams/your-diagram.png)`

See [`diagrams/README.md`](./diagrams/README.md) for guidelines.

### Document Your Research

Add supporting materials to [`research/`](./research/):
- Literature reviews
- Academic papers
- Case studies
- Data and evidence

Use [`research/literature-review.md`](./research/literature-review.md) as a template.

### Record Decisions

Document important decisions in [`discussions/`](./discussions/):
- Architecture Decision Records (ADRs)
- Technical choices
- Design decisions

Copy [`templates/decision-record.md`](./templates/decision-record.md) to get started.

---

## 🤖 Platform Integration

When you push this `.humanet/` folder to GitHub, the Humanet platform can:

- **Auto-discover** your idea (with GitHub App installed)
- **Validate** structure and completeness
- **Evaluate** your idea during provisional phase
- **Update** `config.yml` with validation results
- **Track** contributors and karma
- **Monitor** activity and engagement

**Bot permissions:** Limited to `.humanet/` folder only for security.

---

## 🌟 Available Domains

Choose 2-5 domains in `config.yml`:

```
ai-ml                  blockchain              climate-tech
dev-tools              education               finance
healthcare             knowledge-management    productivity
research-tools         social-impact           web3
other
```

---

## 📖 Learn More

- **Platform:** [humanet.dev](https://humanet.dev)
- **Documentation:** [docs.humanet.dev](https://docs.humanet.dev)
- **GitHub:** [github.com/humanet](https://github.com/humanet)
- **Discord:** [discord.gg/humanet](https://discord.gg/humanet)

---

## ❓ FAQ

### Where does this folder go?

In a `.humanet/` folder at the root of your repository:

```
your-project/
├── .humanet/           ← This template goes here
│   ├── config.yml
│   ├── README.md
│   └── ...
├── src/
├── docs/
└── README.md
```

### Can I customize the structure?

Yes! The only required files are:
- `config.yml`
- `problem_statement.md`
- `idea.md`
- `scope.md`

Everything else is optional. Add or remove folders as needed.

### What about my project README?

Your main project `README.md` stays at the repository root. This `README.md` is specifically for the `.humanet/` folder documentation.

### How do I validate my setup?

The Humanet platform validates your structure automatically. You can also check:
- All required files present
- `config.yml` matches the schema
- No placeholder text remaining

### What license should I use?

Default is `CC-BY-4.0` (Creative Commons Attribution) for idea documentation. You can change this in `config.yml`. Common options:
- CC-BY-4.0 (attribution required)
- CC-BY-SA-4.0 (attribution + share-alike)
- MIT (permissive)
- Unlicense (public domain)

---

## 🎯 Best Practices

**Be Specific**
- ❌ "Makes things easier"
- ✅ "Reduces setup time from 2 hours to 5 minutes"

**Use Evidence**
- Back claims with research
- Cite sources
- Show similar projects

**Add Visuals**
- One diagram beats 1000 words
- Use draw.io for consistency
- Keep diagrams simple and focused

**Document Decisions**
- Why did you choose this approach?
- What alternatives did you consider?
- What are the trade-offs?

**Update Regularly**
- Keep `CHANGELOG.md` current
- Update status in `config.yml` as you progress
- Revise docs as your idea evolves

---

## 🤝 Contributing to Ideas

Found an interesting idea and want to contribute?

1. Read the `.humanet/` documentation
2. Check if they're accepting contributions in `config.yml`
3. Look for contribution guidelines
4. Make your contribution (code, docs, research, design, etc.)
5. Earn karma on the Humanet platform!

---

## 📜 Template License

This template structure is provided as-is for use with the Humanet platform. Your idea documentation uses whatever license you specify in `config.yml`.

---

**Ready to document your idea?** Clone this template and start filling it out!

---

<p align="center">
  <strong>Humanet:</strong> GitHub for Ideas + Notion for Structure + Obsidian's Knowledge Graph<br>
  <em>The missing layer between "I have an idea" and "Let's build it."</em>
</p>
