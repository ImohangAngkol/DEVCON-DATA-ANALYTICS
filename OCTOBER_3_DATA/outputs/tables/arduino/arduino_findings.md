
## Overall findings

The dataset contains **27 participants**. The primary analysis uses
**26 participants** with valid Q1–Q4 responses in both phases.
**1 participant(s)** are excluded from this comparison because
of unresolved responses within Q1–Q4.

Q5 is excluded for everyone because its answer key is recorded as ABCD
and its intended scoring has not been confirmed. A Q5 response of X
does not independently exclude a participant from the Q1–Q4 analysis.

### Primary four-question results

Average scores were **54.8% before** and
**72.1% after**, a difference of
**+17.3 percentage points**.

- Higher post-test scores: **19 (73.1%)**
- Unchanged scores: **4 (15.4%)**
- Lower post-test scores: **3 (11.5%)**

These are paired participant totals on different assessment questions.
They should not be interpreted as changes on identical items.

### Question-level snapshots

**Q1**
- Pre-test: Arduino structure: void setup() runs once — **1/26 (3.8%)**.
- Post-test: Arduino structure: void loop() runs continuously — **20/26 (76.9%)**.

**Q2**
- Pre-test: Hardware: analog input (ADC) range, 0–1023 — **9/26 (34.6%)**.
- Post-test: Hardware: PWM output (analogWrite) range, 0–255 — **15/26 (57.7%)**.

**Q3**
- Pre-test: Circuit design: why a resistor limits current — **26/26 (100.0%)**.
- Post-test: Circuit design: consequence of omitting a resistor — **23/26 (88.5%)**.

**Q4**
- Pre-test: Conditional logic: sensor-triggered actuator (if) — **21/26 (80.8%)**.
- Post-test: Conditional logic: sensor-triggered actuator (if/else) — **17/26 (65.4%)**.

### Original workbook scoring

For all **27 participants**, the workbook's
five-question scoring produces averages of
**42.96% before** and
**57.78% after**, with a difference of
**+14.81 percentage points**.

Under its exact-match formula, individual A–D responses do not match the
Q5 key ABCD. This leaves Q5 with zero credited responses. Agreement with
these formulas confirms scoring consistency, not the validity of the key.

The primary four-question scores and original workbook scores use
different denominators. They must remain clearly labeled in any report.

## Limitations

The assessment is short, the sample is small, and there is no comparison
group. The pre/post questions differ, so differences in difficulty may
contribute to score differences.

The primary analysis covers only four questions and omits the content
represented by Q5. Excluding unresolved Q1–Q4 responses may also affect
how well the results represent all participants.

These findings do not establish long-term retention, complete Arduino
proficiency, or a causal workshop effect.

## Interpretation of the results

For the 26 participants with complete Q1–Q4 responses, average scores
increased from 54.81% to 72.12%. This corresponds to an increase from
2.19 to 2.88 correct answers out of four.

Nineteen participants scored higher on the post-test. Nine answered
all four post-test questions correctly, compared with none on the
pre-test. However, one participant scored zero on the post-test,
showing that outcomes varied.

### Priorities for reinforcement

The lowest post-test correctness was on the PWM output-range question:
15 of 26 participants answered correctly (57.7%). The conditional
if/else question was next lowest, with 17 correct responses (65.4%).
These items suggest priorities for further practice.

The resistor question had the highest post-test correctness:
23 of 26 participants answered correctly (88.5%).

### Interpret different questions carefully

Q1 had 3.85% correctness before and 76.92% after, but the questions
tested setup() and loop(), respectively. This difference cannot be
described as a measured improvement on the same question.

Likewise, lower post-test correctness on the resistor and conditional
logic questions does not by itself establish that participants lost
knowledge, because the questions differed between assessments.

### Keep scoring methods separate

For the same 26 participants, four-question averages were 54.81% and
72.12%, while the workbook's five-question averages were 43.85% and
57.69%. This difference comes from the denominator: the workbook
includes Q5 while awarding no credit for individual A–D responses.

Excluding Q5 changes the score scale and assessed content. It does
not represent additional learning. The four-question results remain
provisional until the intended Q5 scoring is confirmed.


## Recommendations

### Resolve the Q5 key

Check the original pre-test and post-test questions and their scoring
instructions. Confirm whether ABCD represents multiple acceptable
answers, a multiple-selection requirement, or a recording error.

Do not select an interpretation solely because it produces higher scores.
After clarification, document the approved rule and recompute the results.

### Review unresolved responses

Confirm the meaning of X using the original records or the data owner.
Preserve the original values and document any correction.

### Reinforce the lowest post-test item results

- **Q2: Hardware: PWM output (analogWrite) range, 0–255** — 15 of 26 correct (57.7%).

Use practical exercises that connect Arduino program structure, input
and output ranges, resistors, and conditional decisions. Explain the
differences between setup() and loop(), and between analogRead() and
analogWrite(), using short examples and code tracing.

### Improve future assessment comparisons

Use identical or demonstrably comparable pre/post questions when the
goal is to measure change. Include more than one question per skill
and a practical task where possible.

### Later prediction analysis

A provisional model can predict the post-test Q1–Q4 total from pre-test
Q1–Q4 responses. Clearly label its target as a score out of four.

Keep post-test answers and score differences out of the input features.
Evaluate on held-out participants and compare against simple baselines,
including the training-group mean and the participant's pre-test score.

With only 26 complete pairs, predictive results are exploratory.
Resolve Q5 before making claims about prediction of the full assessment.
