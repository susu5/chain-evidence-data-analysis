# Analysis Plan Template

Use this template before deep analysis. This is the first formal output for medium, standard, deep, multi-file, or decision-impacting tasks. After this plan, stop and wait for user confirmation before executing analysis.

## When to Use

Produce an analysis plan when:

- The user provides one or more files for analysis.
- The request involves business decisions, recommendations, SOP, rules, or a formal report.
- The data has multiple sources, uncertain fields, or possible source conflicts.
- The analysis likely requires data quality checks, segmentation, statistical methods, or text classification.

For very small quick questions, provide a short version of this plan before the answer.

## Plan Structure

```text
Analysis goal:
Available data:
Initial file judgment:
Key questions:
Data quality checks:
Field semantics and source authority:
Business chain placement:
Segmentation and comparison plan:
Statistical methods:
Logic and attribution plan:
Expected outputs:
Risks and data gaps:
Execution order:
Confirmation needed:
Confirmation question:
```

## Section Guidance

### Analysis goal

State the decision the analysis should support. Avoid vague goals such as "analyze the file"; translate it into a decision question.

### Available data

List files, sheets, tables, reports, or pasted content currently available. Include file type and likely business object.

### Initial file judgment

State the early view of row grain, IDs, time range, and what the file likely can or cannot prove.

### Key questions

List 3-8 analysis questions. Example:

```text
Which segment performs best?
Where does the funnel drop?
Which source conflicts need review?
Which action should be changed first?
```

### Data quality checks

State the checks to run first:

- Row count and unique count
- Missing values
- Duplicates
- Time coverage
- Outliers
- Category consistency
- Joinability

### Field semantics and source authority

State which fields need interpretation and which source controls each claim type.

### Business chain placement

Map the file to stages of the workflow and list missing upstream/downstream data.

### Segmentation and comparison plan

State the planned cuts, such as:

- User type
- Channel
- Level
- Teacher/owner
- Product/material
- Price band
- Time period
- Action
- Outcome

### Statistical methods

Choose only useful methods:

- Descriptive statistics
- Segmentation
- Cross analysis
- Difference/lift analysis
- Funnel analysis
- Cohort analysis
- Correlation/regression
- Anomaly detection
- Text classification

### Logic and attribution plan

State how conclusions will be reasoned:

- MECE decomposition
- Hypothesis tree
- Source conflict analysis
- Counterfactual check
- Attribution chain
- Decision matrix

### Expected outputs

State the deliverables:

- Quick summary
- Standard report
- Deep report
- Evidence table
- SOP/rules
- Data dictionary
- Next-round data plan

### Risks and data gaps

State known limitations before analysis. This protects the final report from overclaiming.

### Execution order

List the steps in the order they will be done.

### Confirmation needed

Use one of:

```text
Waiting for confirmation: the plan is ready and analysis should not start until the user approves.
Revision needed: the user must choose analysis goal / source priority / output format.
Blocked: missing required data.
```

For medium or larger tasks, do not use "No confirmation needed" unless the user explicitly says to skip confirmation or directly asks to execute without waiting.

### Confirmation question

End the plan with a direct confirmation question:

```text
请确认这个分析计划是否可以执行；如果可以，我会按这个方案继续分析。也可以告诉我需要调整的目标、维度或输出形式。
```

## Short Plan Format

For quick tasks:

```text
I will first check data quality, then identify field meaning and source authority, then segment and compare the key outcome, and finally output findings with evidence grades and next actions.
```

If the task is not obviously quick, use the full plan and wait for confirmation.
