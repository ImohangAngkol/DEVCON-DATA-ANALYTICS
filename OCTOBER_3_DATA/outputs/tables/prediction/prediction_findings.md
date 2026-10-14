## Prediction results

The results below use held-out predictions from repeated five-fold cross-validation. Metrics are averaged across complete repetitions.

### Teachers

Sample: **29 participants**; target: post-test score out of **5**.

- **No change:** MAE **1.586 answers** (31.72 percentage points); RMSE **2.034**; R² **-1.114**; within one answer **58.6%**.
- **Training mean:** MAE **1.269 answers** (25.37 percentage points); RMSE **1.455**; R² **-0.083**; within one answer **50.5%**.
- **Ridge:** MAE **1.151 answers** (23.02 percentage points); RMSE **1.436**; R² **-0.056**; within one answer **40.3%**.
- **Small tree:** MAE **1.107 answers** (22.15 percentage points); RMSE **1.349**; R² **0.068**; within one answer **42.2%**.

**Ridge had lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **+0.118 answers**. It beat both baselines in **95%** of repetitions.

**Small tree had lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **+0.161 answers**. It beat both baselines in **95%** of repetitions.

### Scratch

Sample: **22 participants**; target: post-test score out of **5**.

- **No change:** MAE **1.545 answers** (30.91 percentage points); RMSE **1.706**; R² **-1.682**; within one answer **59.1%**.
- **Training mean:** MAE **0.825 answers** (16.50 percentage points); RMSE **1.095**; R² **-0.107**; within one answer **63.4%**.
- **Ridge:** MAE **0.753 answers** (15.07 percentage points); RMSE **1.135**; R² **-0.189**; within one answer **65.0%**.
- **Small tree:** MAE **0.730 answers** (14.61 percentage points); RMSE **1.065**; R² **-0.048**; within one answer **65.7%**.

**Ridge had lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **+0.071 answers**. It beat both baselines in **95%** of repetitions.

**Small tree had lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **+0.095 answers**. It beat both baselines in **90%** of repetitions.

### micro:bit Heat

Sample: **25 participants**; target: post-test score out of **5**.

- **No change:** MAE **0.880 answers** (17.60 percentage points); RMSE **1.166**; R² **-0.316**; within one answer **84.0%**.
- **Training mean:** MAE **0.784 answers** (15.69 percentage points); RMSE **1.061**; R² **-0.090**; within one answer **65.0%**.
- **Ridge:** MAE **0.862 answers** (17.24 percentage points); RMSE **1.074**; R² **-0.117**; within one answer **56.2%**.
- **Small tree:** MAE **0.819 answers** (16.38 percentage points); RMSE **1.092**; R² **-0.155**; within one answer **59.8%**.

**Ridge did not have lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **-0.077 answers**. It beat both baselines in **0%** of repetitions.

**Small tree did not have lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **-0.035 answers**. It beat both baselines in **10%** of repetitions.

### micro:bit Flood

Sample: **25 participants**; target: post-test score out of **5**.

- **No change:** MAE **0.600 answers** (12.00 percentage points); RMSE **0.872**; R² **-0.231**; within one answer **92.0%**.
- **Training mean:** MAE **0.704 answers** (14.09 percentage points); RMSE **0.822**; R² **-0.095**; within one answer **80.0%**.
- **Ridge:** MAE **0.689 answers** (13.79 percentage points); RMSE **0.809**; R² **-0.063**; within one answer **80.8%**.
- **Small tree:** MAE **0.692 answers** (13.84 percentage points); RMSE **0.806**; R² **-0.058**; within one answer **82.4%**.

**Ridge did not have lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **+0.015 answers**. It beat both baselines in **0%** of repetitions.

**Small tree did not have lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **+0.012 answers**. It beat both baselines in **0%** of repetitions.

### Arduino

Sample: **26 participants**; target: post-test score out of **4**.

- **No change:** MAE **1.077 answers** (26.92 percentage points); RMSE **1.301**; R² **-0.651**; within one answer **84.6%**.
- **Training mean:** MAE **0.867 answers** (21.68 percentage points); RMSE **1.052**; R² **-0.081**; within one answer **59.2%**.
- **Ridge:** MAE **0.916 answers** (22.89 percentage points); RMSE **1.127**; R² **-0.240**; within one answer **59.2%**.
- **Small tree:** MAE **0.905 answers** (22.63 percentage points); RMSE **1.122**; R² **-0.230**; within one answer **67.1%**.

**Ridge did not have lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **-0.048 answers**. It beat both baselines in **0%** of repetitions.

**Small tree did not have lower average MAE than both baselines.** Its MAE reduction relative to the training-mean baseline was **-0.038 answers**. It beat both baselines in **10%** of repetitions.

## What these results mean

A model is useful only if its errors improve on appropriate baselines.
Beating the no-change baseline alone may simply reflect an overall shift
between pre-test and post-test scores. Beating the training-mean baseline
provides stronger evidence that pre-test responses contribute predictive
information in this evaluation.

Small differences between methods should be interpreted cautiously.
The same participants are reused across repetitions, so repetition
counts and error-bar variation are not independent statistical evidence.

If a baseline performs as well as or better than the models, that is a
valid finding. These data may not support useful individual prediction
from pre-test correctness alone.

## Limits of this analysis

Each track contains only 22–29 participants before exclusions. Evaluation
uses participants from the same observed workshop group and does not
establish performance for future cohorts or previously unseen schools.

Random participant splits may place participants from the same school
in both training and validation folds. Generalization to new schools
would require a separate school-grouped evaluation with sufficient data.

The models use correctness indicators, which do not distinguish between
different incorrect answer choices. The assessments are short, and
Teachers and Arduino use different pre/post questions.

Arduino predictions concern Q1–Q4 only. Unresolved post-test outcomes
are excluded from evaluation rather than assigned invented targets.

Model settings were fixed in advance. Any model selected after inspecting
these results would require further validation before being called a
validated best model.

## Conclusions for reporting

Report the prediction errors, the baseline comparisons, the sample size,
and the scoring definition together.

Do not describe MAE or within-one-answer rates as exact prediction
accuracy. Do not convert MAE into an invented accuracy percentage.

This analysis evaluates prediction from pre-test responses. It does not
estimate the causal effect of the workshop, and no model has yet been
validated on an independent future cohort.
