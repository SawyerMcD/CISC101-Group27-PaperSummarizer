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
