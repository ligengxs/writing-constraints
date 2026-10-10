---
name: asd-ste100
description: Use ASD-STE100 as a writing reference when drafting or reviewing technical documentation, including READMEs, operator guides, setup instructions, and maintenance procedures. Apply clarity principles to Chinese documentation without claiming English-standard compliance. Does not apply to creative writing or changes to executable code.
---

# ASD-STE100 writing reference

Use Simplified Technical English principles to make technical prose clear and unambiguous. Preserve the document's language, audience, technical meaning, and requested scope.

## Scope and compliance

- Treat ASD-STE100 as a writing reference by default. This skill is not the specification or its approved dictionary.
- Do not describe output as certified or fully compliant from style editing alone. For a formal compliance request, obtain the applicable specification edition and dictionary, then check vocabulary and writing rules against them. Identify checks that cannot be completed.
- Do not invent rule numbers, approved words, dictionary entries, or numerical limits from memory. Use the applicable specification for such claims. Official source: https://www.asd-ste100.org/.
- For Chinese text, apply the clarity and terminology principles below. English vocabulary restrictions and word-count rules do not directly establish compliance for Chinese text. Do not translate unless requested.

## Writing constraints

- Use one consistent term for each component, state, and operation. Prefer an existing project glossary or the actual UI label. Explain unfamiliar abbreviations at first use when needed by the audience.
- Prefer concrete words and explicit actors. Use active voice where the actor matters. Use imperative verbs for instructions.
- Keep each sentence focused on one action or main idea. Split complicated conditions and explanations without losing their relationships.
- Use a numbered list for an ordered procedure. Give each step one main action; keep a tightly related action together only when this makes execution clearer.
- State prerequisites and conditions before the action they control. Make the object of each action explicit when a pronoun could refer to more than one thing.
- Separate actions, explanations, and expected results when combining them makes the procedure hard to follow. Distinguish a required action from an optional action.
- Preserve the strength of requirements: do not turn "must" into "should", or an option into a requirement. Preserve negation, exceptions, sequence, units, and numerical values.
- Prefer direct wording over nominalizations, idioms, vague qualifiers, and unnecessary synonyms. Keep necessary technical nouns and verbs; do not substitute a simpler word that changes their meaning.
- Keep applicable warnings before the hazardous action. Preserve their conditions and consequences. Do not invent hazards or add unsupported safety claims.

## Editing and review

Read enough surrounding content to understand the procedure and terminology. Resolve factual wording from available source material; flag a material ambiguity instead of inventing behavior.

Preserve commands, code blocks, identifiers, paths, configuration keys, UI labels, and links exactly unless the user also requests a technical correction. Check that the edited prose still matches those artifacts.

For an edit request, deliver the edited text or update the requested files. For a review request, identify consequential ambiguities and give concrete replacements. Do not expand a focused review into an unrelated rewrite.

Before finishing, check terminology consistency, action order, requirement strength, and technical meaning. Report unresolved factual questions or limits on requested compliance checks; omit routine style commentary unless requested.

## Example

Original: "Prior to initiating the procedure, it should be ensured that the power supply has been disconnected."

Reference-style rewrite: "Make sure that the power supply is disconnected before you start the procedure."

The rewrite preserves the original verification action. Change it to "Disconnect the power supply" only if the intended procedure requires the operator to perform that action.
