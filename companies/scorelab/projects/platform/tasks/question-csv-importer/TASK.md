---
name: Question CSV importer
slug: question-csv-importer
assignee: engineer
project: platform
---

Build a small, safe tool that imports an approved question-set CSV (the column format in the `exam-question-writing` skill) into the ScoreLab question bank.

It must validate every row (four options, a valid correct option, both languages present), skip and report bad rows, detect duplicates, support a dry run that changes nothing, and write to a test database first.

Deliver on a branch with instructions and a sample CSV. Move to review for the founder before it ever touches the live database.
