
## Overall findings

The dataset contains **26 participants**. The main paired analysis
includes **25 participants** with complete A–D responses and excludes
**1 unresolved record(s)** from both phases of the comparison.

The average score changed from **67.2%** to
**66.4%**, a difference of **-0.8 percentage points**.

- Higher post-test scores: **7 (28.0%)**
- Unchanged scores: **12 (48.0%)**
- Lower post-test scores: **6 (24.0%)**

## Question-level findings

- **Q1 — Decomposition:** 56.0% pre-test → 80.0% post-test (+24.0 percentage points).
- **Q2 — Pattern Recognition:** 76.0% pre-test → 72.0% post-test (-4.0 percentage points).
- **Q3 — Abstraction:** 12.0% pre-test → 4.0% post-test (-8.0 percentage points).
- **Q4 — Conditional logic / algorithm:** 92.0% pre-test → 80.0% post-test (-12.0 percentage points).
- **Q5 — Debugging:** 100.0% pre-test → 96.0% post-test (-4.0 percentage points).

The lowest post-test correctness was **Q3 (Abstraction): 4.0%**.

The highest post-test correctness was **Q5 (Debugging): 96.0%**.

Across the five questions, there were
**8 incorrect-to-correct transitions**
and **9 correct-to-incorrect transitions**.
These are question-response counts, not counts of distinct participants.

## Effect of the unresolved responses

When X is scored as incorrect, the sensitivity group contains
**26 participants**. Its average
scores are **67.7%** before and
**63.8%** after, a change of
**-3.8 percentage points**.

The complete-pair result is the primary result. The sensitivity result
documents the effect of the workbook's scoring treatment; it does not
confirm the meaning of X.

## Limitations

The group is small, each assessment has only five questions, and there
is no comparison group. Repeating identical questions may also influence
post-test responses. Excluding unresolved records may affect how well
the results represent all participants.

The findings describe immediate assessment performance, not long-term
retention or a proven causal effect of the workshop.

## Interpretation of the results

Average performance was nearly unchanged, decreasing from 67.2% to
66.4%. Across the 25 participants and five questions, this represents
one fewer correct response overall: 84 before and 83 after.

Although seven participants improved and six scored lower, the size
of their individual changes also matters. Counting participants alone
does not determine whether the group average increases.

### Different patterns across questions

Decomposition showed the clearest improvement, increasing from 56% to
80%. Six participants changed from incorrect to correct, while none
changed from correct to incorrect.

Abstraction requires the most urgent review. Only one participant
answered correctly after the workshop. Twenty-two answered incorrectly
in both assessments, and two changed from correct to incorrect.
Check the original question, answer key, and recorded responses before
attributing this result solely to difficulty understanding abstraction.

Conditional logic decreased from 92% to 80%. Three participants changed
from correct to incorrect, suggesting that this item also deserves review.

Debugging remained the strongest post-test result at 96%. Its 100%
pre-test correctness left no room for an increase on this item.

### Effect of the unresolved record

The complete-pair analysis shows a change of -0.80 percentage points.
Including the unresolved post-test as zero changes the result to
-3.85 percentage points.

The treatment of this record therefore affects the apparent size of
the decline. Report the 25-participant result as the primary analysis
and label the 26-participant result as the sensitivity comparison.


## Recommendations

### Review the lowest post-test results

The following are relative priorities within this assessment, rather than
a formal pass/fail classification:

- **Q3 — Abstraction:** Review this item and its distractors; 24 of 25 participants answered incorrectly on the post-test (4.0% correct).
- **Q2 — Pattern Recognition:** Review this item and its distractors; 7 of 25 participants answered incorrectly on the post-test (72.0% correct).
- **Q1 — Decomposition:** Review this item and its distractors; 5 of 25 participants answered incorrectly on the post-test (80.0% correct).

Use a practical flood-alert exercise that asks participants to identify
the sensor input, divide the system into tasks, trace threshold decisions,
and debug an incorrect alert.

### Examine decreases

- Review **Q2 (Pattern Recognition)**, which decreased by 4.0 percentage points. Inspect answer choices and question wording before proposing an explanation.
- Review **Q3 (Abstraction)**, which decreased by 8.0 percentage points. Inspect answer choices and question wording before proposing an explanation.
- Review **Q4 (Conditional logic / algorithm)**, which decreased by 12.0 percentage points. Inspect answer choices and question wording before proposing an explanation.
- Review **Q5 (Debugging)**, which decreased by 4.0 percentage points. Inspect answer choices and question wording before proposing an explanation.

### Resolve the X responses

Confirm the meaning of X with the data owner or original assessment
records. Preserve the original entries and document any approved scoring
change before updating the analysis.

### Check retention

Use a later assessment with comparable questions and a practical task to
examine whether participants retain and apply the concepts.

### Later machine-learning analysis

Use pre-test information to predict post-test scores. Do not use post-test
answers or score changes as input features.

Keep participants with unresolved post-test outcomes out of supervised
model evaluation until those outcomes are confirmed. Evaluate predictions
on held-out participants and compare with simple baselines, including
predicting no change and predicting the training group's mean post-test
score.

Report mean absolute error in score points or percentage points. With
only 25 complete pairs, results should be treated as exploratory.
