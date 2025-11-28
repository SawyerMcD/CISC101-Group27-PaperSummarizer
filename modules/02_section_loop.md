Changelog: Added summary level.
Purpose: Process each section sequentially with uniform constraints.

Workflow per section:

Extraction:

Gather text: Capture raw section text and sub-chunks.

Equation hooks: Tag equations for Module 6.

Summarization:

5 bullets: Produce up to five factual bullets derived strictly from text.

Key values: Preserve numeric results and units.

Claims discipline: Use cautious language when evidence is limited.

Validation:

Content-only derivation: Confirm each bullet maps to specific sentences/phrases in the section.

Length checks: Flag if fewer than five valid bullets are possible.

Artifacts:

Section summary unit: Store bullets, key values, and flags for rendering.
"Summary Level” Modes (Module 02)  
The summarizer should support two summary levels for each section:


For each [Section] -- > Generate a short summary and a detailed summary 

If [short summary selected]:

    Yes --> [generate only a compact 1–2 sentence summary per section]    
    No --> [continue with detailed summary]


If [Detailed summary selected ]

    Yes --> [Generate a short paragraph plus a bullet list of 3–5 key points for each section]
    No --> [continue with short summary]

[Output: short Summary in 1-2 sentences, detailed Summary in short paragraph and bullet list]
