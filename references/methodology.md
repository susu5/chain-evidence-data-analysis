# Chain Evidence Data Analysis Methodology

## Definition

Chain Evidence Data Analysis is a reusable method for analyzing any data file by placing it in the business chain, judging source authority, grading evidence strength, and converting findings into actions.

It answers five questions:

1. What is this file?
2. Can the data be trusted?
3. Which business-chain stage does it represent?
4. What does it prove, and what can it not prove?
5. What action should follow?

## Method Formula

```text
Chain Evidence Data Analysis
= file identification
+ analysis plan
+ data quality check
+ field semantics
+ source authority
+ business chain
+ statistical validation
+ logical attribution
+ evidence grading
+ strategy output
+ document review
```

## Five-Layer Model

| Layer | Key question | Output |
| --- | --- | --- |
| Data layer | Is the file usable and complete? | Data quality judgment |
| Semantic layer | What does each field mean in business terms? | Field dictionary |
| Source layer | Which source has authority for which claim? | Source authority map |
| Chain layer | Where does the evidence sit in the workflow? | Business chain map |
| Decision layer | What should the business do next? | Rules, SOP, recommendations |

## Multi-Turn Analysis Principle

Most real analysis is not completed in one conversation. Use a staged interaction model:

```text
intake -> analysis plan -> execution -> report -> next-round data plan
```

The analysis plan is part of the method, not an optional preface. It prevents premature conclusions, aligns expectations, and makes the work reproducible for another analyst.

The plan should be produced after initial file identification and before deep analysis. It should explain what will be checked, how the data will be segmented, which statistical and logic methods will be used, what outputs will be produced, and what assumptions may affect the result.

## Source Authority

Do not average all fields as if they are equal. Assign each source a role:

| Source type | Typical role | Caution |
| --- | --- | --- |
| System record | Process fact | May miss offline actions |
| Order/payment record | Result fact | Explains outcome, not motivation |
| User text/chat | Demand and objection evidence | Needs classification and samples |
| Sales label/comment | Process observation | May contain subjective bias |
| Teacher/expert rating | Human professional judgment | May vary by person and context |
| AI report/rating | Standardized judgment | Needs calibration and outlier review |
| Recommendation output | System decision | Must be checked against source inputs |

When sources conflict, preserve the conflict and define a review route.

## Evidence Grades

| Grade | Meaning | Decision use |
| --- | --- | --- |
| Strong evidence | Enough sample, reliable fields, clear baseline, multiple sources agree | Can support direct action |
| Medium evidence | Trend is clear but sample, field, or baseline has limits | Can support pilot or targeted change |
| Weak evidence | Signal exists but evidence is incomplete | Use as investigation direction |
| Hypothesis | Plausible but not yet supported | Do not use for final decisions |

## General Workflow

1. Identify file type, entity, row grain, IDs, time range, and business stage.
2. Produce an analysis plan before deep analysis.
3. Run data quality checks before conclusions.
4. Translate fields into business semantics.
5. Decide which source controls which type of claim.
6. Place evidence in the business chain.
7. Run descriptive, segmented, cross, difference, funnel, cohort, anomaly, text, or model-based analysis as needed.
8. Use logic tools to build hypotheses and explain causes.
9. Grade evidence.
10. Convert findings to action.
11. Produce a conclusion-first document.

## Standard Business Chain Examples

Use or adapt these chains:

```text
Acquisition -> contact -> appointment -> first experience -> feedback -> recommendation -> quote -> purchase -> renewal
```

```text
User input -> AI analysis -> human validation -> recommendation -> execution -> result -> review
```

```text
File source -> field meaning -> metric -> segment -> evidence -> decision
```

## Method Slogan

```text
Verify data before judging.
Plan before analyzing.
Define source before merging.
Build meaning before calculating.
Trace the chain before attributing.
Grade evidence before recommending.
```
