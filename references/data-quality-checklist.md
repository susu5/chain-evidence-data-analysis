# Data Quality Checklist

Run this checklist before making business conclusions.

## File Identity

- What is the file type?
- Is it raw data, processed data, or a report?
- What business object does one row represent?
- What is the time range?
- What are the key IDs?
- Which business stage does it describe?

## Structure

- Row count
- Column count
- Column names
- Data types
- Empty columns
- Duplicated columns
- Mixed-language or mixed-format fields

## Entity Grain

Confirm whether one row is:

- One user
- One order
- One lesson
- One chat message
- One event
- One report
- One recommendation
- One aggregated group

Do not calculate user-level metrics from event-level rows without grouping correctly.

## Key Fields

Check:

- User ID / UID
- Time
- Status
- Outcome
- Source
- Owner
- Level/category
- Amount/score
- Text/comment
- Join keys across files

## Missing Values

For every core field, report:

- Missing count
- Missing rate
- Whether missingness is random or concentrated
- Impact on conclusions

## Duplicates

Check:

- Duplicate rows
- Duplicate IDs
- Multiple records per user
- Repeated status updates
- Repeated messages

Decide whether duplicates are errors or valid repeated events.

## Time Checks

Check:

- Parseable timestamps
- Min/max time
- Time gaps
- Impossible order of events
- Timezone issues
- Before/after window definitions

## Value Checks

Check:

- Out-of-range numbers
- Negative amounts when not expected
- Impossible rates
- Unknown categories
- Mixed level formats
- Extreme values

## Joinability

For multi-file analysis:

- Which key joins files?
- How many records match?
- How many do not match?
- Is the join one-to-one, one-to-many, or many-to-many?
- Does joining change the row grain?

## Trust Rating

End the checklist with one of:

```text
High trust: suitable for direct analysis.
Medium trust: suitable with caveats.
Low trust: only directional analysis.
Blocked: cannot support the requested analysis without more data.
```

Explain the reason and the safest next step.
