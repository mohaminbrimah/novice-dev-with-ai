# 🌐 Web Development + AI Engineering Classroom

> **novice-dev-with-ai** — An AI-assisted classroom for learning modern web development
> from scratch. Built for complete beginners. Powered by Claude, GitHub Copilot, and
> the Everything Claude Code (ECC) AI agent system.

---

## 📋 Table of Contents

1. [What This Is](#what-this-is)
2. [What You Will Learn](#what-you-will-learn)
3. [Before You Start — Required Setup](#before-you-start--required-setup)
4. [How to Clone and Contribute](#how-to-clone-and-contribute)
5. [Your First Day — Step by Step](#your-first-day--step-by-step)
6. [Course Modules](#course-modules)
7. [How to Use AI Tools Responsibly](#how-to-use-ai-tools-responsibly)
8. [Repository Structure](#repository-structure)
9. [Student Contribution Rules](#student-contribution-rules)
10. [Code Standards Cheatsheet](#code-standards-cheatsheet)
11. [How to Ask for Help](#how-to-ask-for-help)
12. [Progression Milestones](#progression-milestones)

---

## What This Is

This is not just a code repository. It is a **complete learning environment** that combines:

- A structured HTML and CSS curriculum (8 modules)
- A pre-configured AI agent system for teaching and code review
- Real project exercises you build yourself
- A GitHub-based workflow that mirrors how professional developers work

The AI tools in this repository are configured to **teach you**, not do the work for you.
Every agent, every prompt, and every workflow is designed around one principle:

> **Understanding > Memorization > Code Generation**

---

## What You Will Learn

By the end of this course you will be able to:

| Skill | Module |
|---|---|
| Write valid HTML5 from scratch | 1–2 |
| Use semantic HTML elements correctly | 2 |
| Style pages with CSS (selectors, box model, typography) | 3 |
| Build layouts with CSS Flexbox | 4 |
| Build layouts with CSS Grid | 5 |
| Make websites work on any screen size | 6 |
| Make websites accessible to all users | 7 |
| Add interactivity with vanilla JavaScript | 8 |
| Use AI as a professional development tool | All |
| Work with Git and GitHub like a developer | All |

---

## Before You Start — Required Setup

Complete **every step** before your first class session.

### A. Install Required Software

| Software | Download Link | Purpose |
|---|---|---|
| **VS Code** | https://code.visualstudio.com | Code editor |
| **Git** | https://git-scm.com | Version control |
| **Google Chrome** | https://www.google.com/chrome | Browser + DevTools |
| **Node.js (LTS)** | https://nodejs.org | Required for some tools |

### B. Create Required Accounts

| Account | Link | Why You Need It |
|---|---|---|
| **GitHub** | https://github.com | Store and share your code |
| **Claude** | https://claude.ai | AI mentor access |

### C. Install VS Code Extensions

Open VS Code → Press `Ctrl+Shift+X` → Search and install each:

| Extension | Purpose |
|---|---|
| **Live Server** | Preview your HTML in the browser instantly |
| **Prettier** | Auto-format your code on save |
| **HTML CSS Support** | Smart autocomplete for CSS classes |
| **Auto Rename Tag** | Renames closing tags automatically |
| **Error Lens** | Shows errors inline in your code |
| **GitHub Copilot** | AI code suggestions (requires GitHub account) |

### D. Configure Git (One Time Only)

Open a terminal and run these two commands with your details:

```bash
git config --global user.name "Your Full Name"
git config --global user.email "your@email.com"
```

Verify it worked:

```bash
git config --list
```

You should see your name and email in the output.

---

## How to Clone and Contribute

### Step 1 — Fork the Repository

1. Go to: `https://github.com/[instructor-username]/novice-dev-with-ai`
2. Click the **Fork** button (top right)
3. This creates your own copy under your GitHub account

### Step 2 — Clone Your Fork to Your Computer

```bash
git clone https://github.com/YOUR-GITHUB-USERNAME/novice-dev-with-ai.git
```

Move into the folder:

```bash
cd novice-dev-with-ai
```

### Step 3 — Set the Original Repo as "Upstream"

This lets you pull updates from the instructor later:

```bash
git remote add upstream https://github.com/[instructor-username]/novice-dev-with-ai.git
```

Verify both remotes:

```bash
git remote -v
```

You should see `origin` (your fork) and `upstream` (instructor's repo).

### Step 4 — Create Your Personal Branch

```bash
git checkout -b student/your-name
```

Replace `your-name` with your actual name, all lowercase, hyphens for spaces:
- `student/john-doe`
- `student/amara-mensah`

### Step 5 — Create Your Project Folder

```bash
mkdir -p student-projects/your-name
cd student-projects/your-name
```

Create your first two files:

```bash
# On Windows (Command Prompt or PowerShell):
New-Item index.html
New-Item style.css
```

Or just create them in VS Code: File → New File → save as `index.html` inside your folder.

### Step 6 — Open Your Project in VS Code

```bash
# From the root of the repo:
code .
```

Or open VS Code, then File → Open Folder → select `novice-dev-with-ai`.

### Step 7 — Start Live Server

1. Open `student-projects/your-name/index.html` in VS Code
2. Right-click inside the file
3. Select **"Open with Live Server"**
4. Your browser opens at `http://127.0.0.1:5500/` — this auto-refreshes as you code

### Step 8 — Make Your First Commit

After writing some code:

```bash
git add .
git commit -m "add: my first HTML page"
git push origin student/your-name
```

### Step 9 — Submit a Pull Request (When Milestone Is Complete)

1. Go to your fork on GitHub.com
2. Click **"Compare & Pull Request"** (it appears after you push)
3. Set:
   - Base repository: `instructor/novice-dev-with-ai` → branch: `main`
   - Head repository: `your-fork` → branch: `student/your-name`
4. Title: `[Your Name] — Module [X] Complete`
5. Description: What you built, what you learned, any questions you have
6. Click **Create Pull Request**

---

## Your First Day — Step by Step

Follow this exact sequence on Day 1:

```
Step A → Complete the Required Setup section above
Step B → Fork and clone the repository (Steps 1–4 above)
Step C → Create your folder inside student-projects/your-name/
Step D → Create index.html and style.css
Step E → Open in VS Code + start Live Server
Step F → Type (do NOT copy-paste) the HTML boilerplate:

          <!DOCTYPE html>
          <html lang="en">
            <head>
              <meta charset="UTF-8">
              <meta name="viewport" content="width=device-width, initial-scale=1.0">
              <title>Your Name — My First Page</title>
              <link rel="stylesheet" href="style.css">
            </head>
            <body>
              <h1>Hello, World!</h1>
              <p>My name is [Your Name] and this is my first webpage.</p>
            </body>
          </html>

Step G → Save (Ctrl+S) and watch the browser update
Step H → Add your name to the <title> and <h1>
Step I → Add one more <p> about why you want to learn web development
Step J → Make your first Git commit:
          git add .
          git commit -m "add: day one - my first HTML page"
          git push origin student/your-name
Step K → Share your GitHub branch link with the instructor
```

Congratulations — you are now a developer who has shipped code to GitHub. 🎉

---

## Course Modules

The course is divided into 8 modules. You move to the next only when you
complete the milestone for the current one.

### Module 1 — What is HTML?
**Goal:** Understand what HTML is and write a valid page from memory.
- What is a webpage made of? (HTML + CSS + JS)
- The HTML boilerplate line by line
- Tags, elements, and attributes
- Opening and closing tags
- Viewing your page in the browser
- **Milestone:** Type the full boilerplate from memory and explain each line

### Module 2 — Semantic HTML5
**Goal:** Use the right HTML element for every piece of content.
- Why semantics matter (accessibility + SEO + readability)
- Page landmarks: `<header>`, `<nav>`, `<main>`, `<footer>`
- Content elements: `<section>`, `<article>`, `<aside>`
- Text: `<h1>`–`<h6>`, `<p>`, `<strong>`, `<em>`, `<blockquote>`
- Lists: `<ul>`, `<ol>`, `<li>`
- Links and images: `<a>`, `<img>` with required `alt` text
- Forms: `<form>`, `<input>`, `<label>`, `<button>`
- **Milestone:** Build a 4-region page with zero `<div>` elements

### Module 3 — Introduction to CSS
**Goal:** Style text, colors, and spacing using external CSS.
- Linking CSS to HTML
- Selectors: element, class, ID
- The box model: content, padding, border, margin
- Typography: font-family, font-size, color, line-height
- The CSS reset
- CSS custom properties (variables)
- **Milestone:** Style a page from scratch without referencing examples

### Module 4 — Layouts with Flexbox
**Goal:** Arrange elements in rows and columns using Flexbox.
- `display: flex` — turning on Flexbox
- Container properties: direction, justify-content, align-items, gap, wrap
- Item properties: flex-grow, flex-shrink, flex-basis, align-self
- Building a navigation bar with Flexbox
- Building a card row with Flexbox
- **Milestone:** Center any element on the page using Flexbox

### Module 5 — Layouts with CSS Grid
**Goal:** Build two-dimensional layouts using CSS Grid.
- `display: grid` — turning on Grid
- `grid-template-columns`, `grid-template-rows`
- The `fr` unit
- `gap`, `grid-column`, `grid-row`
- `grid-template-areas`
- Grid vs Flexbox — when to use which
- **Milestone:** Build a 3-column responsive card grid

### Module 6 — Responsive Design
**Goal:** Make your websites work perfectly on any screen size.
- Mobile-first thinking
- The viewport meta tag
- Media queries with `@media (min-width: ...)`
- Common breakpoints (480, 640, 768, 1024, 1280px)
- Responsive images: `max-width: 100%`
- Testing in Chrome DevTools (device toolbar)
- **Milestone:** Make a complete layout work on mobile, tablet, and desktop

### Module 7 — Accessibility
**Goal:** Ensure your websites work for every user, including those with disabilities.
- What is web accessibility and why it matters
- Screen readers and how they navigate pages
- Alt text for images (meaningful vs. decorative)
- Form labels and ARIA roles
- Color contrast requirements
- Keyboard navigation testing
- Using WAVE and Lighthouse to audit
- **Milestone:** Audit your own project and fix 5 accessibility issues

### Module 8 — Introduction to JavaScript
**Goal:** Add interactivity to your HTML pages using vanilla JavaScript.
- What JavaScript does (it controls behavior)
- Linking JS to HTML: `<script src="script.js">`
- Selecting elements: `document.querySelector()`
- Events: `addEventListener('click', ...)`
- Modifying the DOM: `textContent`, `classList.add/remove/toggle`
- Basic form validation
- Dark mode toggle project
- **Milestone:** Build a working form validator + dark mode toggle

---

## How to Use AI Tools Responsibly

AI tools in this classroom are **configured as mentors, not ghostwriters**.

### The AI Will Always:
- Explain concepts BEFORE showing code
- Give hints instead of full answers when you're stuck
- Ask you to explain code back before moving forward
- Celebrate what you got right before correcting mistakes
- Use plain English — no unexplained jargon

### You Must Always:
- Read the AI's explanation before copying any code
- Type code yourself (no copy-paste from AI)
- Try to fix bugs on your own before asking for help
- Be specific about what you've already tried

### Good AI Prompts (Memorize These)

```
"Explain what [concept] is in plain English before showing code."

"Show me the smallest example of [X]. Under 20 lines. Comment every new concept."

"My [element] is [not doing X]. I've tried [Y] and [Z].
 Here's my code: [paste]. Give me a hint, not the answer."

"Review my HTML using the beginner checklist.
 Tell me what I did well and one thing to improve."
```

### Prompts That Will Slow Your Learning (Avoid These)

```
❌ "Write my full project for me"
❌ "Fix all the bugs in my code"
❌ "Give me the final version of [X]"
❌ "Just give me the answer"
```

### The 3-Before-AI Rule

Before opening the AI chat, you must do three things:
1. Re-read the lesson notes for this module
2. Try one more approach on your own
3. Read the error message or inspect in Chrome DevTools

This rule makes you a stronger developer over time.
The best developers write better AI prompts because they understand the problem.

---

## Repository Structure

```
novice-dev-with-ai/
│
├── .claude/                         ← AI configuration (teacher-managed)
│   ├── CLAUDE.md                    ← Primary AI behavior config
│   ├── AGENTS.md                    ← 28 specialized AI agents
│   ├── WORKFLOWS.md                 ← Lesson workflow playbooks
│   ├── agents/                      ← html-educator, css-educator + 28 more
│   ├── skills/                      ← 125 AI workflow skills
│   ├── commands/                    ← 60 slash commands
│   ├── contexts/                    ← student.md, teacher.md
│   ├── hooks/                       ← Automation triggers
│   └── rules/                       ← html-standards.md, css-standards.md
│
├── curriculum/                      ← Module lesson content (teacher-managed)
│   ├── module-01-html-basics/
│   ├── module-02-semantic-html/
│   ├── module-03-css-intro/
│   ├── module-04-flexbox/
│   ├── module-05-grid/
│   ├── module-06-responsive/
│   ├── module-07-accessibility/
│   └── module-08-javascript/
│
├── student-projects/                ← YOUR CODE LIVES HERE ✏️
│   └── your-name/
│       ├── index.html
│       ├── style.css
│       ├── images/
│       └── README.md
│
├── exercises/                       ← Practice exercises (do in order)
│   ├── html/
│   ├── css/
│   └── js/
│
├── demos/                           ← Reference demos from the instructor
│   ├── flexbox-demo/
│   ├── grid-demo/
│   └── responsive-demo/
│
├── README.md                        ← You are here
└── LICENSE
```

---

## Student Contribution Rules

| Rule | Detail |
|---|---|
| **Work in your folder only** | Only edit files inside `student-projects/your-name/` |
| **Use your branch** | Always push to `student/your-name`, never to `main` |
| **Never edit `.claude/`** | The AI system is teacher-managed |
| **Never edit `curriculum/`** | Lesson content is teacher-managed |
| **Never edit another student's folder** | Respect boundaries |
| **Pull before you start** | Run `git pull upstream main` at the start of every session |
| **Commit messages must be descriptive** | See format below |

### Commit Message Format

```
add: description of what you created
fix: description of what you corrected
update: description of what you improved
learn: concept you practiced this session
```

Examples:
```bash
git commit -m "add: homepage with semantic HTML structure"
git commit -m "fix: missing alt text on all images"
git commit -m "update: navigation bar now responsive"
git commit -m "learn: CSS Flexbox card layout"
```

---

## Code Standards Cheatsheet

### HTML — The Minimum Every File Must Have

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Descriptive Title Here</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <!-- Your content here -->
  </body>
</html>
```

### CSS — The Minimum Every File Must Start With

```css
/* === Reset === */
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* === Base === */
body {
  font-family: system-ui, sans-serif;
  font-size: 1rem;
  line-height: 1.6;
}
```

### Quick Reference — Semantic Elements

| Content Type | Use This Element |
|---|---|
| Page header / site banner | `<header>` |
| Navigation links | `<nav>` |
| Primary page content | `<main>` |
| Thematic group of content | `<section>` |
| Standalone content (blog post, card) | `<article>` |
| Related but secondary content | `<aside>` |
| Page or section footer | `<footer>` |
| Important text | `<strong>` |
| Emphasized text | `<em>` |

---

## How to Ask for Help

### In the AI Chat (Claude / Copilot)

Use the student context template:

```
I am a beginner HTML/CSS student on Module [X].
Today I am trying to [describe your goal].

My current code:
[paste your HTML and/or CSS here]

What I've already tried:
[list what you attempted]

My question:
[specific question]
```

The more specific you are, the better the answer.

### In Class

1. Try to solve it yourself for 5 minutes first
2. Ask a classmate who has completed that exercise
3. Raise your hand for the instructor

### On GitHub (Pull Request Comments)

When submitting work, include in your PR description:
- What you built this session
- What was hardest about it
- Any questions you still have

The instructor will respond in the PR review.

---

## Progression Milestones

You do not advance to the next module until you demonstrate the milestone.
Milestones are assessed via a Pull Request — the instructor reviews your work.

| Module | Milestone Requirement |
|---|---|
| **1 — HTML Basics** | Type the full boilerplate from memory and explain every line out loud |
| **2 — Semantic HTML** | Build a complete 4-region page with zero `<div>` elements |
| **3 — CSS Intro** | Style a page (text, colors, box model) without referencing any examples |
| **4 — Flexbox** | Build a responsive navigation bar and a 3-card row using Flexbox only |
| **5 — Grid** | Build a 3-column card grid that collapses to 1 column on mobile |
| **6 — Responsive** | Make your existing project look correct on mobile, tablet, and desktop |
| **7 — Accessibility** | Run a WAVE audit, identify 5 issues, and fix all 5 in your code |
| **8 — JavaScript** | Build a working contact form validator + a dark/light mode toggle |

---

## 🛠 Tools Reference

| Tool | What It's For | How to Open |
|---|---|---|
| **Chrome DevTools** | Inspect, debug, test responsive layouts | F12 or right-click → Inspect |
| **Device Toolbar** | Test mobile layouts | DevTools → Ctrl+Shift+M |
| **W3C HTML Validator** | Check your HTML for errors | https://validator.w3.org |
| **W3C CSS Validator** | Check your CSS for errors | https://jigsaw.w3.org/css-validator |
| **WAVE** | Test accessibility | https://wave.webaim.org |
| **Lighthouse** | Full page audit | DevTools → Lighthouse tab |
| **Google Fonts** | Free web fonts | https://fonts.google.com |
| **Coolors** | Color palette generator | https://coolors.co |
| **Can I Use** | Browser support for CSS features | https://caniuse.com |

---

## ⚡ Quick Command Reference

```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/novice-dev-with-ai.git

# Add upstream (instructor repo) — one time only
git remote add upstream https://github.com/INSTRUCTOR/novice-dev-with-ai.git

# Pull latest from instructor
git pull upstream main

# Create your branch — one time only
git checkout -b student/your-name

# Switch to your branch
git checkout student/your-name

# Save and commit your work
git add .
git commit -m "add: what you built"
git push origin student/your-name

# Check status of your files
git status

# See your commit history
git log --oneline
```

---

*Built with ❤️ for the next generation of web developers.*
*This classroom uses AI to teach — not to think for you.*
