---
name: Database path recommendation
slug: database-path-recommendation
assignee: engineer
project: platform
---

ScoreLab is moving its database to Supabase and must choose between:

1. a full move off Laravel to Supabase (Supabase Auth, database, storage and edge functions), or
2. keeping the Laravel backend and connecting it to a Supabase Postgres database.

Write a recommendation document comparing both on: data safety and backups, security (row-level security, auth), ability to handle large numbers of students, cost, effort and risk of the switch, and how question uploads would work. End with a recommended path, a step-by-step migration plan with a rollback plan, and the decisions the founder must make.

Do not change any live system. Move to review for the founder.
