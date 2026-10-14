Climate Champions pre/post CSV datasets

Five track files plus participants_all, responses_long and question_reference.
All files use UTF-8 with BOM and snake_case headers. Load with pandas.read_csv.
Track files and participants_all have one row per track participation. Use track + participant_id as the record key. Combined and track files overlap; do not concatenate both.
Source: 10_03 Climate Champions Pre & Post Analytics Data.xlsx, transcription and answer key tabs. Restricted identity keys are excluded.

Scores ending _workbook preserve existing workbook calculations. Percentages were converted from 0-1 to 0-100; change_pp_workbook is percentage points. They remain unvalidated, particularly Arduino Q5.
Raw answers are preserved, including X. Confirm the meaning of X before scoring.
Arduino Q5 has answer key ABCD: confirm its intended rule. No new scoring rule was assumed.
responses_long.is_correct_provisional is 1 or 0 only for A-D answers with a single-letter key; unresolved answers/keys are blank. Do not silently treat blanks as incorrect or use varying denominators without documenting the rule.
The workbook says Scratch and both micro:bit tracks use identical pre/post items. Teachers and Arduino use different items; avoid matched per-item gain claims for them.
School text has not been standardized. Workbook example-cell status and cross-track participant identity have not been verified.

Jupyter example (after extracting this ZIP):
import pandas as pd
teachers = pd.read_csv("teachers.csv")
participants = pd.read_csv("participants_all.csv")
responses = pd.read_csv("responses_long.csv")
