Module 5: Hallucination mitigation and methodology checks
Field consistency check (non-evidentiary):

Purpose: Identify internal inconsistencies relative to typical domain reporting without asserting external facts.

Rule: If a typical element (e.g., sample size, variables, statistical tests) is not reported in the provided text, flag as “missing from this paper’s text” rather than “incorrect.”

Methodology red flags detection:

Missing sample sizes: Flag absent or ambiguous n.

Missing variables: Flag undefined independent/dependent variables or predictors/outcomes.

Unreported statistical tests: Flag absent test names when statistical significance is claimed.

Ambiguous metrics or units: Flag unclear definitions or inconsistent units.

Incomplete procedures: Flag missing details critical to replication (e.g., training hyperparameters, data splits).

Output:

Methodology red flags list: Concise bullet list referencing the sections where the issue was detected.
