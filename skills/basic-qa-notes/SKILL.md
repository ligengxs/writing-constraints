---
name: basic-qa-notes
description: When explicitly invoked as $basic-qa-notes in the current user turn, answer project questions and maintain concise, reusable project notes.
---

# Basic Q&A with project notes

Answer the user's current question directly. When the answer reveals durable project context, record it in a short Markdown note so future sessions can use the file instead of the chat history.

## Locate the note

- Follow an existing project convention or the user's specified path. If neither exists, create a Markdown note in the relevant project root with a concise, content-based filename in lowercase kebab case, such as `teleop-setup-notes.md` or `deployment-decisions.md`. The filename should identify the topic or component covered by the note; do not use generic names such as `notes.md`, `output.md`, or `qa-notes.md` unless the project convention requires one.
- Read only the relevant sections and source files needed for the question. Treat notes as a navigation aid, and verify claims against current code or documents when they may have changed.
- Do not copy long conversation transcripts into the note.

## Maintain useful context

- Capture concise facts that help answer future questions: project purpose, component and file locations, agreed decisions with rationale, commands that were verified, unresolved questions, and next steps.
- Distinguish verified facts from assumptions or proposals. Include file paths and dates when they make a claim easier to check or likely to age.
- Update or replace stale entries instead of appending a new version of the same answer. Remove resolved questions and redundant detail. Keep the note easy to scan.
- Avoid storing secrets, credentials, personal data, or large generated output. If the conversation contains them, summarize only the safe operational lesson.

## Respond

- Give a concise answer and link the relevant note or source file. Mention material uncertainty or changes to the note.
- If the answer has no durable project value, answer without editing documentation.
