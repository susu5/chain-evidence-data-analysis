# Universal Chain Evidence Report Template

Use this template for formal reports, analysis documents, memos, or reusable handoffs. Keep the report conclusion-first and evidence-backed.

Before producing the final report, produce an analysis plan unless the user explicitly requests only a quick answer. The plan is the alignment document; the report is the final evidence-backed handoff. For medium or larger tasks, wait for user confirmation after the plan before executing analysis.

Recommended sequence:

```text
analysis plan -> user confirmation -> data inspection -> analysis execution -> final report -> next-round data plan
```

## Report Structure

```text
0. Analysis plan recap
1. Core conclusions
2. File identity and analysis goal
3. Data quality and trust judgment
4. Business chain placement
5. Field semantics and source authority
6. Key metric overview
7. Core findings
8. Segmented comparison
9. Cross analysis and combination insights
10. Conflicts, anomalies, and review points
11. Business attribution
12. Actionable recommendations
13. Rules / SOP / product logic
14. Evidence appendix
15. Data gaps and next analysis plan
```

## Section Guidance

### 0. Analysis plan recap

Briefly restate:

- Analysis goal
- Data used
- Main methods
- Output scope
- Known limitations

Keep this short. Do not let the final report become a process diary.

### 1. Core conclusions

State the most important 3-5 conclusions first. Include the decision implication, not only the metric.

### 2. File identity and analysis goal

Explain:

- File type
- Business object
- Row grain
- Time range
- Key IDs
- Business stage
- What this analysis is trying to decide

### 3. Data quality and trust judgment

Include:

- Row count and unique entity count
- Missing key fields
- Duplicate risk
- Time coverage
- Outliers
- Joinability
- Known caveats
- Overall trust rating

### 4. Business chain placement

Place the file in the workflow. Explain which upstream and downstream stages are missing.

### 5. Field semantics and source authority

Create a compact table:

| Field | Business meaning | Source type | Can support | Risk |
| --- | --- | --- | --- | --- |

### 6. Key metric overview

Define every metric with numerator, denominator, time window, exclusions, and caveat.

### 7. Core findings

Use the required finding format:

```text
Finding:
Evidence:
Impact:
Explanation:
Recommendation:
Evidence grade:
Validation needed:
```

### 8. Segmented comparison

Compare the most important dimensions, such as user type, channel, level, teacher, product, price band, time, action, or status.

### 9. Cross analysis and combination insights

Look for combinations, not only single factors:

```text
level x product
channel x action
teacher x outcome
price band x conversion
source rating x human rating
```

### 10. Conflicts, anomalies, and review points

List conflicts between sources, abnormal records, large gaps, impossible timestamps, outlier outcomes, and samples requiring review.

### 11. Business attribution

Separate:

- Confirmed cause
- High-probability explanation
- Possible explanation
- Unsupported hypothesis

### 12. Actionable recommendations

Use this table:

| Action | Owner | Expected value | Difficulty | Evidence grade | Priority |
| --- | --- | --- | --- | --- | --- |

### 13. Rules / SOP / product logic

Translate analysis into repeatable logic. Examples:

- Classification rule
- Review trigger
- Recommendation rule
- Sales SOP
- Teaching action
- Product display change

### 14. Evidence appendix

Include traceable sample IDs, raw text snippets when useful, table names, file names, calculation notes, and reproducible assumptions.

### 15. Data gaps and next analysis plan

State what to collect next:

- Missing fields
- Missing source
- Longer time range
- Better labels
- Control group
- More samples
- Human review

## Writing Rules

- Lead with conclusions.
- Do not write a diary of analysis steps.
- Attach evidence grades to important findings.
- State data caveats clearly.
- Keep recommendations concrete and owned.
- Distinguish correlation, explanation, and causality.
