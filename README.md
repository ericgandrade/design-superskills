# 🎨 Design Superskills v1.0.1

9 AI skills for UI/UX design, brand identity, design systems, diagrams, presentations, and banner design. Install once across all 8 AI platforms.

![Version](https://img.shields.io/badge/version-1.0.1-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Skills](https://img.shields.io/badge/skills-9-brightgreen.svg)
![Platforms](https://img.shields.io/badge/platforms-8-orange.svg)

## 🚀 Quick Install

**One-liner (recommended):**
```bash
curl -fsSL https://raw.githubusercontent.com/ericgandrade/design-superskills/main/scripts/install.sh | bash
```

**Or use NPX (zero-install):**
```bash
npx design-superskills
```

The installer detects and installs to all 8 AI platforms on your machine: Claude Code, GitHub Copilot, OpenAI Codex, OpenCode, Gemini CLI, Antigravity, Cursor IDE, AdaL CLI.

**Other methods:**
```bash
# npm global
npm install -g design-superskills

# With bundles
npx design-superskills --bundle ui-ux -y
npx design-superskills --bundle visual -y
```

**Local install (no npm/npx required):**
```bash
git clone https://github.com/ericgandrade/design-superskills
cd design-superskills

./scripts/local-install.sh        # Interactive
./scripts/local-install.sh -y     # Auto-install to all detected platforms
./scripts/local-install.sh -y -q  # Silent (CI / scripted)
```

**Uninstall:**
```bash
curl -fsSL https://raw.githubusercontent.com/ericgandrade/design-superskills/main/scripts/uninstall.sh | bash
```

## 🔌 Claude Code Plugin (Native)

Requires **Claude Code v1.0.33+** (`claude --version` to check).

**Method 1: Interactive UI (Inside a running `claude` session) — Recommended**

```text
/plugin marketplace add ericgandrade/design-superskills
/plugin install design-superskills@design-superskills
```

**Method 2: Local test (no install needed)**

```bash
git clone https://github.com/ericgandrade/design-superskills
claude --plugin-dir ./design-superskills
```

### Once installed — all 9 skills under the `design-superskills:` namespace

```
/design-superskills:ui-ux-pro-max
/design-superskills:design
/design-superskills:design-system
/design-superskills:brand
/design-superskills:ui-styling
/design-superskills:slides
/design-superskills:banner-design
/design-superskills:mermaid-diagram
/design-superskills:excalidraw-diagram
```

## ✨ Features

- **9 Design & Visual Skills** - Full creative toolset
- **Zero-Config Install** - Run once, works everywhere
- **Curated Bundles** - UI/UX, Brand & Identity, Visual & Diagrams
- **8 Platform Support** - GitHub Copilot, Claude Code, Codex, OpenCode, Gemini, Antigravity, Cursor, AdaL
- **No API Keys Required** - All skills run natively in your AI tool

## 📦 Available Skills

### 🖥️ UI/UX Design
| Skill | Version | Purpose |
|-------|---------|---------|
| **ui-ux-pro-max** | v1.0.1 | Comprehensive design intelligence for web and mobile — 50+ styles, 161 color palettes, 57 font pairings, UX guidelines, and stack-specific best practices across React, Next.js, Vue, Svelte, Angular, Astro, Flutter, SwiftUI, and more |
| **design** | v1.0.1 | Full design suite: logo generation (55 styles), corporate identity (50 deliverables), HTML presentations, banner design (22 styles), icon design (15 styles, SVG), and social photo generation |
| **ui-styling** | v1.0.1 | UI styling with shadcn/ui, Tailwind CSS, responsive layouts, accessible components, dark mode implementation, and consistent cross-platform styling patterns |

### 🎯 Brand & Identity
| Skill | Version | Purpose |
|-------|---------|---------|
| **brand** | v1.0.1 | Brand identity guidance: brand voice definition, visual identity standards, messaging frameworks, asset management, consistency reviews, style guides, color palette management, and typography specifications |
| **design-system** | v1.0.1 | Create and maintain design systems with three-layer token architecture (primitive, semantic, component), CSS variables, spacing/typography scales, and component specifications |

### 📊 Visual & Diagrams
| Skill | Version | Purpose |
|-------|---------|---------|
| **slides** | v1.0.1 | Strategic HTML presentations with Chart.js data visualizations, design tokens, responsive layouts, copywriting formulas (AIDA, PAS), and contextual slide strategies for pitches, reports, and education |
| **banner-design** | v1.0.1 | Design banners in any of 22 styles (minimalist, gradient, glassmorphism, neon, retro, geometric, etc.) for social media, advertising, web heroes, and print across all major platforms |
| **mermaid-diagram** | v1.0.1 | Generate Mermaid diagram syntax from plain-language descriptions — flowchart, sequence, class, state, ER, mindmap, Gantt, and more |
| **excalidraw-diagram** | v1.0.1 | Create hand-drawn style diagrams in Excalidraw JSON format — architecture sketches, concept maps, user flows, C4 context, and org charts. Ready to paste into Obsidian or Excalidraw directly |

## 🎯 Curated Bundles

```bash
# UI/UX Design (3 skills)
npx design-superskills --bundle ui-ux -y

# Brand & Identity (2 skills)
npx design-superskills --bundle brand-identity -y

# Visual & Diagrams (4 skills)
npx design-superskills --bundle visual -y

# All Design Skills (complete collection)
npx design-superskills --bundle all -y
```

## 🚀 Quick Start Examples

```bash
# Design a modern landing page
claude -p "design a SaaS landing page hero section with glassmorphism style in Next.js + Tailwind"

# Create a Mermaid architecture diagram
claude -p "create a C4 context diagram for a multi-tenant SaaS platform"

# Build a design system
claude -p "create a design system with primitive tokens for a fintech product"

# Generate an Excalidraw sketch
claude -p "sketch the user flow for an onboarding wizard in Excalidraw"

# Design a social media banner
claude -p "create a LinkedIn banner in gradient style announcing a product launch"
```

## 💻 Supported Platforms

- **GitHub Copilot CLI** - Terminal AI assistant (`~/.github/skills/`)
- **Claude Code** - Anthropic's Claude in development (`~/.claude/skills/`)
- **OpenAI Codex** - GPT-powered coding assistant (`~/.codex/skills/`)
- **OpenCode** - Open source AI coding assistant (`~/.agent/skills/`)
- **Gemini CLI** - Google's Gemini in terminal (`~/.gemini/skills/`)
- **Antigravity** - AI coding assistant (`~/.gemini/antigravity/skills/`)
- **Cursor IDE** - AI-powered code editor (`~/.cursor/skills/`)
- **AdaL CLI** - AI development assistant (`~/.adal/skills/`)

## ⌨️ Compatibility & Invocation

| Tool | Type | Invocation Example | Path |
|------|------|--------------------|------|
| **Claude Code** | CLI | `/ui-ux-pro-max help me...` | `~/.claude/skills/` |
| **Gemini CLI** | CLI | `Use mermaid-diagram to...` | `~/.gemini/skills/` |
| **Codex CLI** | CLI | `Use design-system to...` | `~/.codex/skills/` |
| **Antigravity** | IDE | *(Agent Mode)* `Use skill...` | `~/.gemini/antigravity/skills/` |
| **Cursor** | IDE | `@ui-styling` in Chat | `~/.cursor/skills/` |
| **Copilot** | Ext | *(Paste skill content manually)* | N/A |
| **OpenCode** | CLI | `opencode run @excalidraw-diagram` | `~/.agent/skills/` |
| **AdaL CLI** | CLI | *(Auto)* Skills load on-demand | `~/.adal/skills/` |

## ⚡ CLI Commands & Shortcuts

| Command | Shortcut | Purpose |
|---------|----------|---------|
| `install` | `i` | Install skills |
| `list` | `ls` | List installed skills |
| `status` | `st` | Show global install status + version differences |
| `update` | `up` | Smart update (outdated + missing skills) |
| `uninstall` | `rm` | Remove skills |
| `doctor` | `doc` | Check installation |

```bash
npx design-superskills i -a -y -q    # Install all, skip prompts, quiet mode
npx design-superskills status         # Show global status + skill version differences
npx design-superskills up -y          # Update outdated + install missing skills
npx design-superskills ls -q          # List with minimal output
npx design-superskills --list-bundles # Show available bundles
```

## 📋 System Requirements

- Node.js 14+ (for installer)
- One or more supported platforms installed

## 🔒 Privacy

design-superskills does not collect, store, transmit, or share any user data.

- **No external servers** — no backend, no telemetry, no network requests of its own
- **No API keys required** — all skills run within your AI tool using native tools
- **No logging** — nothing is recorded outside of your local session
- **Open source** — all skill logic is fully auditable

## 📄 License

MIT - See [LICENSE](./LICENSE) for details.

## 🔗 Quick Links

- 📝 [Changelog](CHANGELOG.md) - Release history
- 🐛 [Issues](https://github.com/ericgandrade/design-superskills/issues) - Report problems

## Part of the Superskills Family

| Package | Skills | Focus | Install |
|---------|--------|-------|---------|
| [claude-superskills](https://github.com/ericgandrade/claude-superskills) | 18 | Core: orchestration, planning, research & content | `npx claude-superskills` |
| [obsidian-superskills](https://github.com/ericgandrade/obsidian-superskills) | 6 | Obsidian knowledge management | `npx obsidian-superskills` |
| [career-superskills](https://github.com/ericgandrade/career-superskills) | 20 | Job search & career development | `npx career-superskills` |
| [product-superskills](https://github.com/ericgandrade/product-superskills) | 8 | Product management & GTM strategy | `npx product-superskills` |
| **design-superskills** | 9 | UI/UX design, brand & diagrams | `npx design-superskills` |
| [avanade-superskills](https://github.com/ericgandrade/avanade-superskills) | 3 | Avanade-branded content (private) | `git clone git@github.com:ericgandrade/avanade-superskills.git` |

---

**Built with ❤️ by [Eric Andrade](https://github.com/ericgandrade)**

*Version 1.0.1 | May 2026*
