# copilot.md — Guidance for GitHub Copilot

## Project
This repository is a beginner-friendly micro-course website (GitHub Pages) to teach a 9th grader the basics of 3D modelling and how 3D printing works, using browser-based tools (primarily Tinkercad).

Audience: absolute beginner, 9th grade, macOS user, no prior CAD experience.

Primary goals:
- Explain concepts in simple, accurate language
- Provide short, step-by-step exercises
- Produce basic printable models (STL export)
- Prepare the student for an in-person session where the instructor will 3D print the designs

Tool focus:
- Tinkercad (browser-based, free)

## Output style rules
- Use short sentences.
- Use simple words; avoid jargon.
- Prefer bullet lists and checklists.
- Each lesson must include:
  - Goal
  - Time estimate
  - What you need
  - Steps (numbered, small steps)
  - Common mistakes / quick fixes
  - Deliverable (what to bring to next meeting)
- Keep each lesson to ~10–25 minutes.
- Avoid external dependencies, accounts beyond Tinkercad, or paid tools.

## Repository structure (target)
Generate and maintain content in this structure:

- index.md                       (homepage)
- README.md                      (repo overview)
- _config.yml                    (Jekyll theme config)
- lessons/
  - lesson-01-tinkercad-basics.md
  - lesson-02-nameplate-keychain.md
  - lesson-03-simple-house.md
  - lesson-04-holes-and-cutouts.md
  - lesson-05-export-stl-and-checks.md
- assets/
  - images/                      (optional screenshots)
  - stl-examples/                (optional sample STLs)

Keep links working on GitHub Pages:
- Use relative links like `/lessons/lesson-01-tinkercad-basics`

## Content requirements
### Homepage (index.md)
Must contain:
- What this course is
- What the student needs
- Lesson list with links
- Short note: “We will 3D print your models in the next meeting.”

### Lesson progression
Design lessons in this order:

1) Lesson 1 — Tinkercad Basics
- Navigate view: rotate / pan / zoom
- Add shapes
- Resize, rotate, move
- Align
- Group
Deliverable: saved Tinkercad design link or name

2) Lesson 2 — Nameplate / Keychain
- Box base + Text
- Align + group
- Optional keychain hole
Deliverable: STL export + screenshot

3) Lesson 3 — Simple House
- Body, roof, door, windows
- Use Align and Group
Deliverable: STL export

4) Lesson 4 — Holes and Cutouts
- Hole shapes
- Subtraction idea (make a hole through an object)
- Practical: keychain hole + simple stamp/cutter
Deliverable: STL export

5) Lesson 5 — Export and Print Checks
- How to export STL
- Check for: single solid object, not too thin, no floating parts
- Basic size guidance (mm)
Deliverable: “final” STL + short note of what it is

### 3D printing explanations
Include very short explanations only:
- “3D printing builds objects layer by layer.”
- “STL is the file that describes the shape.”
Do NOT include printer operation steps that require hardware access.

## Markdown formatting conventions
- Use headings:
  - `# Lesson X — Title`
  - `## Goal`
  - `## Time`
  - `## What you need`
  - `## Steps`
  - `## Common mistakes and fixes`
  - `## Deliverable`
- Use checkboxes for deliverables when helpful:
  - `- [ ] Exported STL`
- Avoid huge paragraphs.
- Keep the tone friendly and confident.

## Copilot tasks you may be asked to do
When requested, generate:
- New lesson pages using the required template
- Improvements to clarity (simpler language)
- A short glossary page (optional) with terms like: model, shape, group, align, hole, STL
- A “Week plan” page summarizing lessons and expected deliverables

## Non-goals / constraints
- Do not switch to Blender or professional CAD for this beginner course.
- Do not require installation of apps.
- Do not add JavaScript frameworks or build pipelines.
- Do not include paid courses.
- Keep everything accessible from a browser.

## Quality checklist (use before finalizing changes)
- [ ] Links work in GitHub Pages (use leading `/lessons/...`)
- [ ] Each lesson has all required sections
- [ ] Steps are numbered and granular
- [ ] Deliverable is clear and specific
- [ ] Language is simple enough for a beginner