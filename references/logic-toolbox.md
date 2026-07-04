# Logic Toolbox

Use these tools to turn statistical results into reliable business reasoning.

## MECE Decomposition

Break a problem into complete, non-overlapping parts.

Example for low conversion:

```text
user quality
sales action
product fit
price
timing
teacher/service experience
data quality
```

## Hypothesis Tree

Start with possible explanations, then map each to evidence.

Template:

```text
Problem:
Hypothesis:
Required evidence:
Current evidence:
Evidence grade:
Decision:
```

## Source Authority

Define what each source is allowed to prove.

Example:

```text
Orders prove purchase outcome.
Chat proves expressed concern or intent.
Sales notes prove sales-side observation.
AI ratings prove standardized model judgment.
Human expert ratings prove professional review under a specific context.
```

Do not let a weaker source override a stronger source for the wrong claim type.

## Conflict Analysis

Conflicts are high-value evidence. Look for:

- AI judgment vs human judgment
- System field vs raw text
- Recommendation vs actual outcome
- Sales label vs user expression
- Earlier status vs later status
- Expected level vs observed performance

For each conflict, write:

```text
Conflict:
Possible reason:
Business risk:
Review rule:
Next data needed:
```

## Counterfactual Thinking

Ask:

```text
Would the outcome likely have happened without this action?
```

Use this to avoid over-crediting actions taken on already high-intent users.

## Attribution Chain

Do not stop at the metric. Trace:

```text
what changed
where it changed
which segment changed
which action preceded it
which owner controls it
what should change next
```

## Decision Matrix

Rank recommendations:

| Action | Value | Difficulty | Evidence grade | Owner | Priority |
| --- | --- | --- | --- | --- | --- |

Prioritize high-value, low-difficulty, medium-or-strong evidence actions first.

## Claim Language

Use precise wording:

- Strong evidence: "The data supports..."
- Medium evidence: "The pattern suggests..."
- Weak evidence: "There is an early signal..."
- Hypothesis: "A plausible explanation is..."

Avoid saying "caused" unless there is a credible causal design, experiment, or strong quasi-experimental setup.
