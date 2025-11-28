Missing/empty sections:

Rule: If the section is missing or empty, do not fabricate content; output a placeholder and add a warning.

Outcome: Adds to Checks & Warnings.

Short sections (<50 words):

Rule: Provide only defensible bullets; annotate with short-section warning.

Outcome: Adds to Checks & Warnings.

Hallucination mitigation:

Rule: Every bullet must be traceable to the text; avoid external inference.

Outcome: If traceability is uncertain, downgrade specificity or omit.

Long-paper chunking:

Strategy:

Chunk by subheadings, figures, tables.

Maintain overlap of 1–2 sentences across chunks to retain context.

Local summarize → global reconcile: Summarize chunks, then unify into a section summary with conflict resolution favoring explicit statements in the text.

Outcome: Reliable summaries even when sections exceed context limits.
Strengthen Evidence & Hallucination Guardrails
1. Strict evdience mode: When evidence_mode = "strict": 
Summarizer should:
* Only include claims, equations, and results that appear in the provided text. 
* If it cannot find enough information, it must say so explicity (example: The source text does not provide enough detail to summarize this section in strict evidence mode.)
2. Section Warning Messages
For sections that are: 
  * missing/empty, or
  * too short (< 50 words)
If either of these apply, output a standardized warning, such as:
"Section skipped: no usuable text provided." 
"Section very short: summary may be incomplete."
