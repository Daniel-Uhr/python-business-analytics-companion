## Assessment rubric

The rubric assesses decisions, coherence, reproducibility, and communication. Visual appearance alone does not replace conceptual quality. Total: **100%**. The weights are retained; the four levels describe quality without imposing an additional numerical score per level.

### 1. Understanding and observational unit — 10%

**Excellent.** Correctly identifies units, period, keys, types, and relationships for every table.

**Adequate.** Identifies the central elements, with minor omissions that do not affect results.

**Partial.** Confuses or omits some units, keys, or coverage.

**Insufficient.** Analyzes without understanding the data structure.

### 2. Quality and cleaning — 15%

**Excellent.** Diagnoses relevant problems and documents decisions, impacts, and alternatives.

**Adequate.** Treats the main problems and justifies most decisions.

**Partial.** Incomplete diagnosis or weakly justified decisions.

**Insufficient.** Ignores quality or alters data arbitrarily.

### 3. Transformation — 10%

**Excellent.** Creates coherent variables and analytical levels while preserving meaning and units.

**Adequate.** Appropriate transformations with minor documentation gaps.

**Partial.** Partly correct or poorly traceable transformations.

**Insufficient.** Incorrect, opaque, or question-incompatible variables.

### 4. Integration and cardinality — 15%

**Excellent.** Identifies units, selects correct keys, understands cardinalities, validates rows, and avoids improper multiplication.

**Adequate.** Joins correctly and performs essential checks.

**Partial.** The merge runs, but cardinality reasoning or validation is weak.

**Insufficient.** Incorrect keys, unjustified many-to-many joins, or invalid analytical data.

### 5. Indicators — 10%

**Excellent.** Defines coherent measures and states numerator, denominator, unit, and analytical level.

**Adequate.** Correct indicators with sufficient documentation.

**Partial.** Some correct indicators, but ambiguities or weak denominators remain.

**Insufficient.** Incorrect indicators or use without understanding.

### 6. Exploratory analysis — 10%

**Excellent.** Investigates distributions, groups, time, and unusual observations with clear questions.

**Adequate.** Covers the main patterns and interprets them appropriately.

**Partial.** Limited or mechanical exploration, weakly connected to questions.

**Insufficient.** Merely displays tables or numbers without investigation.

### 7. Visualization — 10%

**Excellent.** Produces 3–5 relevant, legible, interpreted charts with question, evidence, and limitation.

**Adequate.** Appropriate charts that are mostly well communicated.

**Partial.** Redundancy, poor chart choices, or incomplete interpretation.

**Insufficient.** Misleading charts, missing units, or disconnection from the analysis.

### 8. Storytelling — 8%

**Excellent.** Five conclusions connect evidence, interpretation, and implication without unjustified causal claims.

**Adequate.** Clear, supported conclusions with minor gaps.

**Partial.** Generic, repetitive, or partly unsupported conclusions.

**Insufficient.** Unsupported statements or unjustified causal claims.

### 9. Recommendations — 7%

**Excellent.** Presents 2–4 plausible actions, separated from evidence and consistent with limitations.

**Adequate.** Coherent recommendations connected to the analysis.

**Partial.** Vague recommendations or weak links to evidence.

**Insufficient.** Recommendations without analytical support or presented as causal findings.

### 10. Limitations and reproducibility — 5%

**Excellent.** Records limitations, decisions, and relative paths; Restart + Run All completes without errors.

**Adequate.** Reproducible notebook with the main limitations recorded.

**Partial.** Reproduction requires small fixes, or limitations are incomplete.

**Insufficient.** Nonreproducible notebook or missing limitations.

### Serious conceptual errors

The following can substantially reduce the assessment of the corresponding dimension:

- An unjustified many-to-many merge.
- Removing an observation only because it is extreme, without investigation and substantive justification.
- Treating structural missingness as an error.
- Imputing discounts without justification.
- Ignoring duplicates.
- Using an indicator without understanding its denominator.
- Confusing total revenue with average performance.
- Ignoring differences in active months.
- Making a causal claim.
- Presenting an unsupported recommendation.
- Submitting a notebook that does not run completely.

### Alternative solutions

A decision different from the reference pipeline can receive full credit when it is substantively justified, documented, consistently applied, and accompanied by an explanation of its effects on the results.
