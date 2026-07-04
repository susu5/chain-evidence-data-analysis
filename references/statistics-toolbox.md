# Statistics Toolbox

Use the smallest statistical method that can answer the business question. Prefer interpretable methods before complex models.

## Descriptive Statistics

Use for the first pass.

Check:

- Count
- Unique count
- Mean
- Median
- Min/max
- Percentiles
- Standard deviation
- Share/ratio
- Distribution shape

Answers:

- What is the overall situation?
- Is the sample usable?
- Is the metric concentrated or dispersed?
- Are there obvious outliers?

## Segmentation

Segment by dimensions such as:

- User type
- Channel
- Level
- Teacher or owner
- Product or material
- Price band
- Time period
- Action taken
- Outcome status

Answers:

- Which group performs better or worse?
- Where is the problem concentrated?
- Which group should receive a different action?

## Cross Analysis

Cross two or more dimensions:

```text
level x teacher type
level x material
channel x sales action
price band x conversion
source rating x human rating
```

Use when single-factor analysis is too shallow.

## Difference Analysis

Compare:

- Group A vs Group B
- Converted vs not converted
- Before vs after
- Top vs bottom
- Current vs baseline
- Experiment vs control when available

Metrics:

- Absolute difference
- Relative difference
- Lift
- Share difference
- Median difference

Always state whether the difference is large enough to matter in business terms.

## Correlation

Use to check whether two variables move together.

Guardrail:

```text
Correlation is not causation.
```

Write correlation claims as signal or hypothesis unless the design supports causal inference.

## Regression and Control Variables

Use when several factors may affect the same outcome.

Common uses:

- Logistic regression for conversion, purchase, churn, pass/fail.
- Linear regression for amount, score, duration, count.
- Control variables to check whether one factor still matters after accounting for others.

Explain results in plain language:

```text
After controlling for channel and level, this factor is still associated with higher conversion.
```

## Funnel Analysis

Use for staged workflows:

```text
lead -> contact -> appointment -> experience -> quote -> purchase
```

Check:

- Count at each step
- Step conversion
- Drop-off
- Segment-specific drop-off
- Action before next-step movement

## Cohort Analysis

Use when time or batch matters:

- New users by week
- Users from a campaign
- Users after a rule change
- Teacher/material batches

Answers:

- Did later batches improve?
- Is behavior stable over time?
- Does a new rule work after launch?

## Anomaly Detection

Flag but do not automatically delete:

- Extreme values
- Impossible timestamps
- Sudden level jumps
- Source conflicts
- Duplicate IDs
- Unusually dense actions
- Mismatched status

Classify anomalies as:

- Data error
- Real business exception
- High-value special case
- Review-required sample

## Text Analysis

Use for chats, comments, feedback, reports, and notes.

Methods:

- Keyword extraction
- Theme classification
- Intent detection
- Objection classification
- Sentiment or attitude
- Action tagging
- Raw evidence sampling

Always keep representative raw examples when text evidence supports a recommendation.
