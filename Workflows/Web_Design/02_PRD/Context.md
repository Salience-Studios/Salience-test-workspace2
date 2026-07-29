---
salience: "stage"
id: "ba9b03a0-1913-409b-bb6f-1f0c6bd3156e"
name: "PRD"
type: "text"
position: 2
goal: "Creating a Product Requirement document for the website using the research output and starting client paramaters."
declared_inputs: ["subject_context","attachments","stage:01_Research"]
allowed_tools: ["web_search:free","web_fetch:free","read_file:free"]
tool_ceiling_tokens: 20000
default_model: ""
---

# Web Design — 02_PRD

Goal: Creating a Product Requirement document for the website using the research output and starting client paramaters.

Type: text. Runs as one request plus a Salience-side tool loop, and produces one markdown output.

## Inputs
- This subject's `Context.md`
- Files uploaded to this subject or run
- The approved output of `01_Research` for this subject

Nothing outside this list is loaded. `CLAUDE.md` and this workspace's `Context.md` are always read first and are not declared here.

## Tools
- `web_search` — Search the web. Billed per query.
- `web_fetch` — Fetch one URL.
- `read_file` — Read a repo file or an attachment.

Ceiling: 20,000 tokens of tool results per run. A result that would exceed it pauses the run and asks. Nothing outside this list is callable.

## Do
- Creates PRD

## Do not
- Write code

## Output
One file: `outputs/<Subject>.md`.

