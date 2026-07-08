---
name: SUSU5-chain-evidence-data-analysis
description: Universal data/file analysis method with a mandatory plan-first workflow. Use whenever the user asks to analyze, summarize, diagnose, compare, validate, interpret, report on, or produce recommendations from data, files, spreadsheets, Excel, CSV, JSON, PDF, HTML reports, chat logs, system exports, learner reports, sales records, course records, order files, metric tables, or mixed source material. Also use for Chinese requests such as 数据分析, 分析文件, 分析表格, 分析报告, 看这个数据, 诊断数据, 输出分析方案, 生成分析报告, 总结文件, 业务分析, 统计分析, 转化分析, SOP分析, 归因分析, or 涉及数据/文件并需要分析. For medium or larger work, first output an analysis plan/分析方案 and wait for user confirmation before executing the analysis.
---

# SUSU5 Chain Evidence Data Analysis

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

Analysis is often too large for one response. For any medium, standard, deep, multi-file, or decision-impacting task, do not jump directly to data execution or the final report.

Use this mandatory staged flow:

```text
Stage 1: understand the task and inspect available files
Stage 2: produce an analysis plan
Stage 3: stop and ask the user to confirm or revise the plan
Stage 4: execute the analysis only after the plan is confirmed
Stage 5: produce the final report or handoff
Stage 6: list unresolved gaps and next-round data needs
```

The first substantive response must be an analysis plan, not final conclusions, unless the user explicitly asks for a very quick answer or says to skip confirmation and execute directly. If the file is simple, use quick mode and still include a short plan before conclusions.

After producing the plan, stop and ask for confirmation using direct language such as:

```text
请确认这个分析计划是否可以执行；如果可以，我会按这个方案继续分析。
```

Do not continue into data analysis in the same response after the plan unless the user explicitly said in the current request that no confirmation is needed.

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
Confirmation question:
```

For formal plan output, use `references/analysis-plan-template.md`.

## Workflow

1. **Identify the file**
   - Determine file type, business object, row grain, time range, key IDs, and likely business stage.
   - State what the file can and cannot support before analyzing deeply.

2. **Produce the analysis plan**
   - Summarize the intended analysis route before performing the full analysis.
   - State the questions, data checks, segmentation logic, methods, output format, risks, and execution order.
   - End with a clear confirmation question and wait. Continue only after the user confirms, revises the plan, or explicitly asks to execute without confirmation.

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
- Do not execute analysis in the same response as the plan unless the user explicitly waives confirmation.
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
