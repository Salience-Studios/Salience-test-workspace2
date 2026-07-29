---
salience: "stage"
id: "ec4f9625-5008-41fc-9dc3-4f250383a4f3"
name: "Research"
type: "text"
position: 1
goal: "Establish what the market does and how we can fit into it"
declared_inputs: ["subject_context","attachments"]
allowed_tools: ["web_search:free","web_fetch:free","read_file:free"]
tool_ceiling_tokens: 20000
default_model: ""
---

# Web Design — 01_Research

Goal: Establish what the market does and how we can fit into it

Type: text. Runs as one request plus a Salience-side tool loop, and produces one markdown output.

## Inputs
- This subject's `Context.md`
- Files uploaded to this subject or run

Nothing outside this list is loaded. `CLAUDE.md` and this workspace's `Context.md` are always read first and are not declared here.

## Tools
- `web_search` — Search the web. Billed per query.
- `web_fetch` — Fetch one URL.
- `read_file` — Read a repo file or an attachment.

Ceiling: 20,000 tokens of tool results per run. A result that would exceed it pauses the run and asks. Nothing outside this list is callable.

## Do
- Researches potential compitition
- Researches pricing options

## Do not
- Build or write any code

## Output
One file: `outputs/<Subject>.md`.
Sections: A Markdown file that cleanly displays pricing and logistics findings

Either Cite a real source or ask if you don't know the answer. Nothing made up.
