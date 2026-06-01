# Contributing to /filesdot/ 🤝

> Thank you for considering contributing to this list! Your help makes the Linux ricing community stronger. 🎨✨

<br/>

## 📋 Table of Contents

- [🗣️ Code of Conduct](#%EF%B8%8F-code-of-conduct)
- [🚀 Quick Start](#-quick-start)
- [➕ Adding a New Resource](#-adding-a-new-resource)
- [✏️ Formatting Guidelines](#%EF%B8%8F-formatting-guidelines)
- [✅ Quality Standards](#-quality-standards)
- [🔄 Pull Request Process](#-pull-request-process)
- [🔍 Review Criteria](#-review-criteria)
- [❌ What We Don't Accept](#-what-we-dont-accept)
- [💡 Pro Tips](#-pro-tips)
- [🆘 Getting Help](#-getting-help)

<br/>

## 🗣️ Code of Conduct

This project adheres to a [Code of Conduct](code_of_conduct.md). By participating, you agree to uphold this code. Please report unacceptable behavior to the maintainers.

> 🌟 **Be kind. Be helpful. Be awesome.**

<br/>

## 🚀 Quick Start

### I want to...

| Goal | Steps |
|------|-------|
| **Add a new tool/theme** | 1. Read [Quality Standards](#-quality-standards) → 2. Format entry per [Guidelines](#%EF%B8%8F-formatting-guidelines) → 3. Submit PR |
| **Fix a broken link** | 1. Locate entry → 2. Update URL → 3. Submit PR with "fix: broken link" in title |
| **Improve documentation** | 1. Edit markdown → 2. Preview locally → 3. Submit PR describing changes |
| **Suggest a category** | 1. Open an Issue first → 2. Discuss with maintainers → 3. Implement if approved |
| **Report a problem** | 1. Search existing Issues → 2. Open new Issue with details → 3. Wait for response |

### Fork & Clone
```bash
# 1. Fork the repo on GitHub
# 2. Clone your fork
git clone https://github.com/filesdot/resources.git
cd resources

# 3. Create a branch
git checkout -b feature/add-my-awesome-tool

# 4. Make your changes
# 5. Test locally (see below)
# 6. Commit & push
git commit -m "feat: add MyAwesomeTool to Terminal Emulators"
git push origin feature/add-my-awesome-tool

# 7. Open a Pull Request on GitHub
```

### Preview Locally
```bash
# Install a markdown previewer (optional but recommended)
# VS Code: Install "Markdown All in One" extension
# Or use:
npm install -g markdownlint-cli
markdownlint README.md  # Check for formatting issues

# Preview in browser:
# - VS Code: Ctrl+Shift+V
# - Or: https://dillinger.io (paste markdown)
```

<br/>

## ➕ Adding a New Resource

### Step 1: Verify Eligibility
Before adding, ensure the resource:
- ✅ Is **actively maintained** (last commit ≤ 2 years ago, or clear "stable" status)
- ✅ Has a **public repository** or official website
- ✅ Is **relevant to Linux desktop customization** ("ricing")
- ✅ Works on **at least one major distro** (Arch, Debian, Fedora, etc.)
- ✅ Is **free and open-source** (or has a free tier for theming/customization)

### Step 2: Choose the Right Category
Place your entry in the most specific category possible:

```
README.md
├── 🪟 Window Manager
│   ├── Stacking
│   ├── Tiling
│   └── Dynamic
├── 🎨 Color Schemes
├── 🔤 Fonts
│   ├── Sans-Serif
│   ├── Monospace
│   └── Nerd Fonts
├── 💻 Terminal Ecosystem
│   ├── Emulators
│   ├── Shells
│   ├── Prompts
│   └── CLI Tools
└── ... (see full TOC)
```

> ❓ **Not sure where it fits?** Open an Issue to discuss first!

### Step 3: Format Your Entry

#### 📝 Basic Template
```markdown
- [Tool Name](https://official-link) <sup>Protocol</sup> - Brief, compelling description of what it does and why it's awesome.
```

#### 📝 Enhanced Template (Recommended)
```markdown
- [Tool Name](https://official-link) <sup>X11 + Wayland</sup> ⭐⭐ - Brief description. Highlights: key feature 1, key feature 2. [🔗 Docs](https://docs-link)
```

#### 📝 For Theme Collections
```markdown
- [Theme Collection Name](https://repo-link) - Number+ themes for [target app]. Styles: style1, style2. Compatible with: app1, app2.
```

### Step 4: Add Metadata Tags

| Tag | Format | Example | When to Use |
|-----|--------|---------|-------------|
| **Protocol** | `<sup>X11</sup>`, `<sup>Wayland</sup>`, `<sup>X11 + Wayland</sup>` | `<sup>Wayland</sup>` | For WMs, bars, launchers, etc. |
| **Shell** | `<sup>zsh</sup>`, `<sup>bash</sup>`, `<sup>fish</sup>` | `<sup>zsh</sup>` | For prompts, shell plugins |
| **Difficulty** | `⭐` to `⭐⭐⭐⭐⭐` | `⭐⭐` | For tools with notable learning curve |
| **App Target** | `<sup>Firefox</sup>`, `<sup>Spotify</sup>` | `<sup>VSCode</sup>` | For app-specific themes/plugins |
| **License** | `<sup>MIT</sup>`, `<sup>GPL-3.0</sup>` | `<sup>CC0-1.0</sup>` | Optional, for clarity |

> 💡 **Tip**: Use `<sup>` tags for superscript metadata. Keep it minimal 1-3 tags max per entry.

### Step 5: Write a Great Description

#### ✅ Do:
```markdown
- [yazi](https://github.com/sxyazi/yazi) <sup>Rust</sup> ⭐⭐ - Blazing fast terminal file manager with async I/O, image preview, and vim-like keybindings. Highlights: tabs, multi-select, custom keymaps.
```

#### ❌ Don't:
```markdown
- [yazi](https://github.com/sxyazi/yazi) - A file manager.
```

#### Description Formula:
```
[What it is] + [Key differentiator] + [Notable features]. Highlights: [feature 1], [feature 2].
```

<br/>

## ✏️ Formatting Guidelines

### Markdown Standards
- Use `-` for list items (not `*` or `+`)
- Keep lines ≤ 120 characters where possible
- Use **bold** for emphasis, *italics* for subtle notes
- Use `> 💡` for tips, `> ⚠️` for warnings
- Use tables for comparisons (see existing entries)

### Link Rules
- ✅ Use absolute URLs: `https://github.com/user/repo`
- ✅ Use descriptive link text: `[Tool Name](https://link)`
- ❌ Don't use bare URLs: `https://github.com/user/repo`
- ❌ Don't use "click here" as link text

### Category Headers
```markdown
### Category Name  <!-- Level 3 header for sub-sections -->

- [Entry 1](https://link) - Description.
- [Entry 2](https://link) - Description.
```

### Tables (When Applicable)
```markdown
| Tool | Protocol | Difficulty | Description |
|------|----------|------------|-------------|
| [Name](https://link) | <sup>Wayland</sup> | ⭐⭐ | Brief description. |
```

> 📏 **Table Rule**: Only use tables when comparing 3+ similar items. For single entries, use list format.

<br/>

## ✅ Quality Standards

### For Tools/Applications
- [ ] Repository has ≥ 50 stars OR clear active development
- [ ] Last commit ≤ 2 years ago (or marked "stable/maintenance")
- [ ] Has basic documentation (README, wiki, or man page)
- [ ] No critical unresolved security issues
- [ ] Works on ≥ 1 major Linux distro without major hacks

### For Themes/Collections
- [ ] Includes installation instructions
- [ ] Has preview images or screenshots
- [ ] Compatible with current version of target app
- [ ] Clear license (preferably permissive: MIT, GPL, CC)

### For Tutorials/Guides
- [ ] Step-by-step instructions with commands
- [ ] Tested on ≥ 1 distro (specify which)
- [ ] Includes troubleshooting tips
- [ ] Updated within last year

### For Wallpapers/Assets
- [ ] High resolution (≥ 1920x1080)
- [ ] Clear license (CC0, CC-BY, or public domain preferred)
- [ ] Organized collection (not a single random image)
- [ ] Direct download or well-documented source

<br/>

## 🔄 Pull Request Process

### 1. Before You PR
- [ ] Search existing PRs to avoid duplicates
- [ ] Test your changes locally (preview markdown)
- [ ] Run `markdownlint README.md` if possible
- [ ] Ensure all links work (no 404s)

### 2. PR Title Format
```
<type>: <short description>

Examples:
feat: add Hyprlock to Screen Lockers
fix: update broken link for Catppuccin
docs: improve WM comparison table
chore: add difficulty ratings to Fonts section
```

#### Valid Types:
| Type | When to Use |
|------|-------------|
| `feat` | Adding new resources, sections, or features |
| `fix` | Correcting broken links, typos, formatting |
| `docs` | Improving documentation, guides, comments |
| `style` | Markdown formatting, whitespace, no logic change |
| `refactor` | Reorganizing content without changing meaning |
| `chore` | Maintenance tasks, metadata updates |

### 3. PR Description Template
```markdown
## What does this PR do?
[Brief summary]

## Resource Details
- **Name**: Tool/Theme Name
- **Category**: Where it's added
- **Protocol**: X11/Wayland/Both
- **Difficulty**: ⭐ rating (if applicable)
- **Why it's awesome**: [1-2 sentences]

## Checklist
- [ ] Entry follows formatting guidelines
- [ ] Link is valid and points to official source
- [ ] Description is concise and informative
- [ ] Added to correct category
- [ ] No duplicate entries
- [ ] Tested locally (if applicable)

## Screenshots/Preview (if applicable)
[Attach or link to preview]
```

### 4. After Submitting
- Monitor your PR for maintainer feedback
- Respond to review comments within 7 days
- Make requested changes promptly
- Be patient, reviews may take 1-2 weeks

<br/>

## 🔍 Review Criteria

Mainters will evaluate PRs based on:

### ✅ Acceptance Criteria
- [ ] Follows all formatting guidelines
- [ ] Meets quality standards for its category
- [ ] Adds unique value (not redundant with existing entries)
- [ ] Clear, accurate, and helpful description
- [ ] All links functional and properly formatted
- [ ] Appropriate metadata tags included

### ⚠️ Common Reasons for Requesting Changes
- Description too vague or promotional
- Wrong category placement
- Missing protocol/difficulty tags
- Link points to fork instead of upstream
- Resource not actively maintained
- Duplicate of existing entry (even if wording differs)

### ❌ Automatic Rejection Triggers
- Self-promotion without significant community value
- Paid-only tools with no free tier
- Resources requiring non-free dependencies
- Malicious or privacy-invasive software
- Entries with no documentation or installation guide

<br/>

## ❌ What We Don't Accept

### Content Restrictions
- ❌ **Self-promotion**: Your personal blog/tutorial unless widely referenced by community
- ❌ **Abandoned projects**: No commits in >2 years with no "stable" designation
- ❌ **Distros/ISOs**: This list is for customization tools, not OS installations
- ❌ **Kernel modules/drivers**: Too low-level for desktop ricing focus
- ❌ **Server-only tools**: Must have desktop/GUI relevance
- ❌ **Windows/macOS-only**: Must work on Linux (even via compatibility layer)

### Formatting Restrictions
- ❌ **All-caps descriptions**: "AMAZING TOOL!!!" → "A powerful, customizable tool."
- ❌ **Excessive emojis in entries**: Save emojis for section headers
- ❌ **Nested lists**: Keep entries flat for consistency
- ❌ **Inline code in descriptions**: Use backticks only for command examples in docs

### Ethical Restrictions
- ❌ **Telemetry-heavy tools** without opt-out
- ❌ **Non-free licenses** without clear justification
- ❌ **Resources that break other tools** without warning
- ❌ **Content with discriminatory language** in docs or community

<br/>

## 💡 Pro Tips

### For Faster Reviews
1. **Small, focused PRs**: One feature/resource per PR
2. **Follow the template**: Copy-paste the PR description template
3. **Test your links**: Use a link checker or manually verify
4. **Preview locally**: Catch formatting issues before submitting
5. **Reference issues**: Link to related Issues in your PR description

### For Better Descriptions
```markdown
# Weak:
- [tool](https://link) - A cool thing for your terminal.

# Strong:
- [tool](https://link) <sup>Rust</sup> ⭐ - Terminal utility that does X with Y benefit. Highlights: feature A, feature B. Compatible with Z.
```

### For Finding the Right Category
1. Search README.md for similar tools
2. Check the [full TOC](README.md#-contents)
3. When in doubt, add to the most specific sub-category
4. Still unsure? Ask in your PR description!

### For Maintaining Your Entry
- If you're the author: Update the entry if your project changes significantly
- If a link breaks: Submit a `fix:` PR or open an Issue
- If a project is abandoned: Suggest moving to "Archived" sub-section (if created)

<br/>

## 🆘 Getting Help

### Stuck? Try These:
1. **Read existing PRs**: See examples of accepted contributions
2. **Check Issues**: Your question may already be answered
3. **Ask in Discord**: Join communities linked in [README](README.md#-communities--resources)
4. **Open a Draft PR**: Get early feedback on formatting

### Need to Discuss First?
Open an Issue with:
```markdown
## Proposal: [Brief title]

### What I want to add/change:
[Description]

### Why it belongs in this list:
[Justification]

### Where it should go:
[Suggested category]

### Questions:
[Any uncertainties]
```

### Contact Maintainers
- 🐙 **GitHub**: [@flessan](https://github.com/flessan)
- 💬 **Discord**: [Server invite from README](README.md#-communities--resources)
- ✉️ **Email**: [admin@dotfiles.xyz](mailto:filingdot@gmail.com)

> ⏱️ **Response Time**: We aim to respond to Issues/PRs within 7 days. If longer, feel free to politely ping.

<br/>

## 🙏 Thank You!

Every contribution, big or small, helps make this resource better for the entire Linux ricing community. Whether you're adding a hidden-gem tool, fixing a typo, or suggesting a new category, your effort is valued.

> 🎨 **Happy Ricing, and Happy Contributing!**

<br/>

---

<div align="center">

  <sub>✨ Made with ❤️ by the Linux Ricing Community ✨</sub></br>
  <sub>🟡 filesdot community!11</sub>

</div>
