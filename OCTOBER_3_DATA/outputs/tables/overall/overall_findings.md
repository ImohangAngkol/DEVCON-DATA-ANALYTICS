
## Overall findings

The five source datasets contain **129 participant-track
records**. Primary analyses include **127 records** and
exclude **2 records** with unresolved responses in the
questions being scored.

These totals describe records across tracks. They do not independently
verify the number of unique people across the entire program.

### Primary results

| Track | Included / source | Questions | Pre | Post | Difference |
| --- | --- | --- | --- | --- | --- |
| Teachers | 29/29 | 5 | 25.52% | 55.86% | +30.34 pp |
| Scratch | 22/22 | 5 | 50.00% | 75.45% | +25.45 pp |
| micro:bit Heat | 25/25 | 5 | 47.20% | 58.40% | +11.20 pp |
| micro:bit Flood | 25/26 | 5 | 67.20% | 66.40% | -0.80 pp |
| Arduino | 26/27 | 4 | 54.81% | 72.12% | +17.31 pp |

Here, pp means percentage points. Arduino results use four questions;
the other tracks use five.

### Teachers

Among **29 participants**, average scores were **25.52% before** and **55.86% after**, a difference of **+30.34 percentage points**.

**22** participants scored higher, **6** had unchanged scores, and **1** scored lower. This track used related but different pre/post questions.
### Scratch

Among **22 participants**, average scores were **50.00% before** and **75.45% after**, a difference of **+25.45 percentage points**.

**21** participants scored higher, **0** had unchanged scores, and **1** scored lower. This track used identical pre/post questions.
### micro:bit Heat

Among **25 participants**, average scores were **47.20% before** and **58.40% after**, a difference of **+11.20 percentage points**.

**13** participants scored higher, **8** had unchanged scores, and **4** scored lower. This track used identical pre/post questions.
### micro:bit Flood

Among **25 participants**, average scores were **67.20% before** and **66.40% after**, a difference of **-0.80 percentage points**.

**7** participants scored higher, **12** had unchanged scores, and **6** scored lower. This track used identical pre/post questions.
### Arduino

Among **26 participants**, average scores were **54.81% before** and **72.12% after**, a difference of **+17.31 percentage points**.

**19** participants scored higher, **4** had unchanged scores, and **3** scored lower. This track used related but different pre/post questions.

## Question-level priorities

The following items had the lowest post-test correctness within their
respective tracks. All ties are retained.

- **Teachers, Q1:** Abstraction. Post-test correctness was **9/29 (31.0%)**.
- **Scratch, Q3:** Abstraction. Post-test correctness was **10/22 (45.5%)**.
- **micro:bit Heat, Q1:** Decomposition. Post-test correctness was **9/25 (36.0%)**.
- **micro:bit Heat, Q3:** Abstraction. Post-test correctness was **9/25 (36.0%)**.
- **micro:bit Flood, Q3:** Abstraction. Post-test correctness was **1/25 (4.0%)**.
- **Arduino, Q2:** Hardware: PWM output (analogWrite) range, 0–255. Post-test correctness was **15/26 (57.7%)**.

Review question wording, answer keys, and selected responses alongside
these rates before attributing them solely to learning difficulties.

## Interpretation across tracks

The results show different patterns across the five assessments.
Higher group averages do not mean every participant improved, and a
nearly unchanged average can conceal improvements on some questions and
decreases on others.

Track differences cannot establish which workshop was most effective.
The tracks assessed different content and involved different groups.
Arduino also uses fewer scored questions in the primary analysis.

No pooled score is presented because combining these percentages could
obscure differences in assessment content and scoring.



## Data-quality decisions

### micro:bit Flood

The primary analysis contains **25 participants**
and shows a difference of
**-0.80 percentage points**.

The workbook calculation includes **26 participants**
and treats X responses as incorrect, producing
**-3.85 percentage points**.

The meaning of X remains unresolved. Keep both calculations labeled
and use the complete-pair result as the primary finding.

### Arduino

The primary Q1–Q4 analysis contains **26 participants**
and shows a difference of
**+17.31 percentage points**.

The original workbook calculation uses five questions and
**27 participants**, producing
**+14.81 percentage points**.

These differences reflect both scoring and inclusion decisions.
The ABCD key for Q5 must be clarified before reporting a validated
full-assessment result.

## Recommendations

1. **Prioritize the identified post-test difficulties.**
   Use the question-level table to select focused practice activities.
   Review both the item and its answer choices before drawing conclusions.

2. **Resolve the outstanding scoring issues.**
   Confirm X responses and the intended Arduino Q5 scoring using original
   assessment records or the data owner. Document approved corrections.

3. **Strengthen future assessment design.**
   Use identical or demonstrably comparable pre/post questions when
   estimating change. Include multiple questions per skill and a practical
   task to reduce reliance on a single item.

4. **Assess retention.**
   Add a later assessment to examine whether participants retain and apply
   the concepts beyond the immediate post-test.

5. **Keep report labels explicit.**
   Show sample size, questions scored, and any exclusions beside results.
   Avoid presenting differences between tracks as an effectiveness ranking.

## Limitations

The analysis uses small track-level samples and short assessments.
There is no comparison group, and question difficulty may differ between
phases and tracks. Repeated questions may also influence post-test results.

Some records or questions are excluded because their scoring is unresolved.
These decisions affect the population and content represented by the results.

The findings describe recorded assessment performance. They do not
establish causation, long-term retention, or complete mastery.

## Next stage: exploratory prediction

The prediction notebook will examine whether pre-test information helps
predict held-out participants' post-test scores.

Models should be evaluated separately by track initially, using the same
documented scoring definitions. Arduino's provisional target is the
post-test Q1–Q4 total.

Use participant-level validation, training-fold preprocessing, and simple
baselines. Do not use post-test answers or score differences as predictors.
Multiple answers from one participant must not be treated as independent
participants.

Report prediction error and variability. Predictive performance does not
measure the causal effectiveness of the workshops.
