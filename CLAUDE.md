---
salience: "workspace"
kind: "claude"
name: "Northbang Studio"
---

# CLAUDE.md — Northbang Studio

Read this first. Then read `Context.md`. Both, every session.

## What this is
we build and run e-commerce store websites for physical product companies

## Voice and standards
Direct and plain. No hype, no filler.
Every claim specific enough to check.
Short sentences. Cut anything that reads as padding.

## Stack
Next.js, tailwind css, typescript, github, vercel for deployment

## Conventions
One file per completed stage, named for the subject it is about.
Markdown only. Keep every file short enough to load cheaply.
Never edit a prior stage's output — flag the conflict instead.

## Reading order
1. Read `CLAUDE.md` — this file.
2. Read `Context.md`.
3. Read the `Context.md` of the stage you are working in.
4. Read only what that stage lists under Inputs. Nothing beyond that unless the stage names it.

One stage at a time. Never skip ahead. Every completed stage produces one file in that stage's `outputs/`, named for the subject. Never edit a prior stage's output — flag the conflict instead.

## Structure
```
Northbang Studio/
├── CLAUDE.md       ← read first
├── Context.md      ← read second
├── Systems/        ← one folder per repeatable workflow
│   └── <System>/<NN_Stage>/{Context.md, References.md, outputs/}
└── Subjects/       ← one folder per client, project, or period
```

Keep every file short. No preamble, no recap of what you just did.
