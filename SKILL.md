---
name: chain-evidence-data-analysis
description: Universal data and file analysis workflow for business decision-making. Use when the user asks to analyze, summarize, diagnose, compare, validate, report on, or produce recommendations from any data, file, spreadsheet, Excel, CSV, JSON, PDF, HTML report, chat log, system export, learner report, sales record, course record, order file, metric table, or mixed source material. Trigger whenever the request combines data/files/source material with analysis, insights, reporting, diagnosis, statistical comparison, segmentation, SOP, recommendations, or decision support.
---

# Chain Evidence Data Analysis

Use this skill to turn any file or data source into a decision-ready analysis. The method is:

```text
First verify data, then define sources.
First build meaning, then trace the business chain.
First segment, then compare differences.
First evidence, then conclusions.
First attribution, then action.
```

## Core Method

Apply the Chain Evidence Data Analysis formula:

```text
file identification
+ analysis plan
+ data quality check
+ field semantics
+ source authority
+ business chain placement
+ statistical validation
+ logical attribution
+ evidence grading
+ strategy output
+ report review
```

Always treat a file as evidence from one part of a larger business chain, not as isolated rows.

## Staged Interaction Rule

Analysis is often too large for one response. For any medium, standard, deep, multi-file, or decision-impacting task, do not jump directly to the final report.

Use this staged flow:

```text
Stage 1: understand the task and inspect available files
Stage 2: produce an analysis plan
Stage 3: execute the analysis after the plan is accepted or the user asks to continue
Stage 4: produce the final report or handoff
Stage 5: list unresolved gaps and next-round data needs
```

The first substantive response should usually be an analysis plan, not final conclusions. If the user explicitly asks for a quick answer or the file is very simple, use quick mode and still include a short plan before conclusions.

The analysis plan must include:

```text
Analysis goal:
Available data:
Initial file judgment:
Key questions:
Data quality checks:
Segmentation and comparison plan:
Statistical methods:
Logic and attribution plan:
Expected outputs:
Risks and data gaps:
Execution order:
```

For formal plan output, use `references/analysis-plan-template.md`.

## Workflow

1. **Identify the file**
   - Determine file type, business object, row grain, time range, key IDs, and likely business stage.
   - State what the file can and cannot support before analyzing deeply.

2. **Produce the analysis plan**
   - Summarize the intended analysis route before performing the full analysis.
   - State the questions, data checks, segmentation logic, methods, output format, risks, and execution order.
   - Ask for confirmation only when the plan requires a business choice, missing source, or risky assumption. Otherwise continue if the user has clearly asked to proceed.

3. **Run a data quality check**
   - Check row count, unique entity count, missing values, duplicates, time coverage, outliers, inconsistent codes, and join keys.
   - Do not draw business conclusions before this step.
   - For detailed checks, use `references/data-quality-checklist.md`.

4. **Build field semantics**
   - Translate important fields into business meaning.
   - Classify fields as facts, human judgments, AI judgments, user expressions, process states, tags, or derived metrics.
   - Define numerator, denominator, time window, exclusions, and caveats for every metric.

5. **Determine source authority**
   - Separate source roles instead of merging them too early.
   - Examples: system records are process facts; orders are result facts; user messages are demand evidence; sales labels are process observations; AI ratings are standardized judgments; teacher or expert ratings are human validation.
   - If sources conflict, preserve the conflict and route it to review instead of silently averaging.

6. **Place the evidence in the business chain**
   - Map data to stages such as acquisition, contact, appointment, lesson, feedback, AI analysis, recommendation, quote, purchase, renewal, or retention.
   - Ask where the problem appears, where it begins, who owns the action, and which next step the file can improve.

7. **Analyze with statistics**
   - Start with descriptive statistics and distributions.
   - Segment by important business dimensions.
   - Use cross analysis, difference analysis, funnel analysis, cohort analysis, correlation, regression, anomaly detection, and text analysis when useful.
   - For method selection, use `references/statistics-toolbox.md`.

8. **Analyze with logic**
   - Use MECE decomposition, hypothesis trees, conflict analysis, counterfactual thinking, attribution chains, and decision matrices.
   - Avoid treating correlation as causation unless the data design supports causal claims.
   - For logic tools, use `references/logic-toolbox.md`.

9. **Grade evidence**
   - Mark each important finding as `strong evidence`, `medium evidence`, `weak evidence`, or `hypothesis`.
   - Evidence grading must consider sample size, source reliability, source agreement, field completeness, and whether a comparison baseline exists.

10. **Output decisions**
   - Convert findings into rules, SOP changes, labels, recommendation logic, review mechanisms, product changes, sales actions, teaching actions, or next-data requirements.
   - Rank actions by value, difficulty, evidence strength, and owner.

11. **Produce the document**
   - If the user asks for a report, memo, handoff, analysis document, or reusable output, use `references/report-template.md`.
   - Keep the report conclusion-first: conclusion, evidence, risk, action, then detailed tables.

## Output Modes

- **Quick mode**: core conclusion, data risks, 3-5 findings, and next actions.
- **Standard mode**: full analysis report with data quality, segmentation, evidence grades, and recommendations.
- **Deep mode**: report plus SOP/rules/product logic, evidence appendix, and next-round data plan.

Choose the smallest mode that satisfies the user. Use standard mode when the user asks for a document or report.

## Required Finding Format

For every major finding, write:

```text
Finding:
Evidence:
Impact:
Explanation:
Recommendation:
Evidence grade:
Validation needed:
```

## Guardrails

- Do not skip the data quality check.
- Do not skip the analysis plan for medium, standard, deep, multi-file, or decision-impacting work.
- Do not merge sources with different authority without explaining the source roles.
- Do not state causality from correlation alone.
- Do not rely only on averages; segment and inspect outliers.
- Do not output conclusions without evidence grades.
- Do not hide data gaps; state what fields, samples, time ranges, or comparison groups are missing.
- Do not write a process diary. Write conclusion-first, evidence-backed analysis.

## Reference Routing

- Read `references/methodology.md` when the user wants the full method, training material, or a reusable framework.
- Read `references/analysis-plan-template.md` when producing the first-step analysis plan.
- Read `references/report-template.md` when producing a formal report or document.
- Read `references/statistics-toolbox.md` when choosing statistical methods or explaining quantitative evidence.
- Read `references/logic-toolbox.md` when building hypotheses, attribution, source authority, or decision logic.
- Read `references/data-quality-checklist.md` before or during structured file inspection.
