Module 1: Intake & setup
Purpose: Normalize inputs, establish processing plan, and pre-validate content.

Inputs: Paper text, section list, audience.

Core actions:

Section normalization:

Map sections: Align user-provided section names to detected paper sections using exact title matching and common aliases (e.g., “Methods” ≈ “Materials and Methods”).

Order enforcement: Preserve user-given order; if not provided, use paper’s native order.

Detection and sizing:

Missing/empty sections: Identify sections not present or lacking substantive text.

Short sections (<50 words): Mark as short.

Chunking plan:

Per-section chunking: Break long sections into logical sub-chunks using headings/subheadings, paragraphs, and figure/table references.

Overlap strategy: Include small overlaps across chunks to preserve continuity.

Metadata capture:

Section word counts: Store counts for guardrail checks.

Equation presence: Pre-scan for LaTeX/math constructs.
