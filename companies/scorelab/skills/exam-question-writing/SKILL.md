---
name: exam-question-writing
description: Write exam-standard, bilingual (Hindi + English) multiple-choice questions for RAS/RPSC, IAS/UPSC and SSC, verified and formatted for upload to the ScoreLab question bank.
---

# Exam question writing

Use this whenever you write practice or mock-test questions for ScoreLab.

## Match the exam

- **RAS/RPSC (Prelims):** general studies with heavy weight on Rajasthan — history, art and culture, geography, polity and administration, economy, and current events. Factual and statement-based questions are common.
- **IAS/UPSC (Prelims GS):** statement-based questions ("Which of the statements given above is/are correct?"), match-the-following, and assertion–reason. Test understanding, not just recall.
- **SSC (CGL, CHSL, MTS, GD):** shorter, direct questions in general awareness, reasoning, quantitative aptitude and English. Quant and reasoning questions need a worked solution.

## Each question must have

- One clear question stem and four options (A–D), with exactly one correct answer.
- Plausible wrong options: no joke options, no "all of the above" unless the exam really uses it.
- A short explanation (2–4 sentences) of why the answer is right, and why the trap option is wrong when useful.
- Hindi and English versions with the same meaning. Use standard exam terminology in Hindi (as in RPSC/UPSC Hindi papers), not word-for-word machine translation.
- A source: official site, PIB, government report, NCERT, or a standard reference book.

## Checks before you hand over

1. Is the answer correct and still true today (no outdated office-holders, figures or schemes)?
2. Could two options be argued as correct? If so, rewrite.
3. Is the difficulty tag honest (easy / medium / hard)?
4. Is it a near-duplicate of another question in the set?
5. If you are not sure, set `flag` to explain why instead of guessing.

## Output format

Deliver a CSV file with these columns, one row per question:

`exam, subject, topic, difficulty, question_en, option_a_en, option_b_en, option_c_en, option_d_en, question_hi, option_a_hi, option_b_hi, option_c_hi, option_d_hi, correct_option, explanation_en, explanation_hi, source, flag`

- `exam`: RAS, RPSC, UPSC, SSC-CGL, SSC-CHSL, etc.
- `correct_option`: A, B, C or D.
- `flag`: empty when verified; otherwise a short note.

Also post a summary comment: number of questions, topics covered, how many are flagged and why.
