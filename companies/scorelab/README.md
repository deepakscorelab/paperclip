# ScoreLab — AI agent company

ScoreLab is an AI-powered exam-prep platform ([scorelab.co.in](https://scorelab.co.in) and an Android app) for Indian competitive exams: RAS/RPSC, IAS/UPSC and SSC. This package sets up ScoreLab's AI team in [Paperclip](https://github.com/paperclipai/paperclip): four agents, their skills, projects, starter tasks and daily routines.

## How it works

A hub-and-spoke company. The founder is the board. The CEO turns goals into weekly priorities and delegates to three specialists. **Nothing goes public without the founder's approval** — questions, posts, releases and database changes all arrive as drafts for review.

```
Founder (board)
└── CEO
    ├── Content Lead          question bank + daily current affairs
    ├── Social Media Manager  Telegram, Instagram, YouTube, WhatsApp Channel
    └── Engineer              Android app, website, Supabase, Play Store
```

## Org chart

| Agent | Title | Reports to | Skills | Model | Monthly budget |
| --- | --- | --- | --- | --- | --- |
| CEO | Chief Executive Officer | Founder | weekly-planning | Claude Sonnet 5.5 | $15 |
| Content Lead | Head of Exam Content | CEO | exam-question-writing, current-affairs-digest | Claude Sonnet 5.5 | $40 |
| Social Media Manager | Social Media Manager | CEO | social-post-drafting | Claude Sonnet 5.5 | $25 |
| Engineer | Full-Stack Engineer | CEO | play-store-release | Claude Opus 5.5 | $40 |

Budgets are a starting point; each agent pauses automatically at its limit. Change them in Paperclip at any time.

## Daily rhythm (India time)

| When | Routine | Agent | Output for your review |
| --- | --- | --- | --- |
| Daily 6:13 am | Daily current affairs | Content Lead | 8–12 verified news items with practice MCQs |
| Daily 7:17 am | Daily question set | Content Lead | 25 bilingual MCQs as CSV (topic rotates by weekday) |
| Daily 10:23 am | Daily post pack | Social Media Manager | Posts for all four channels |
| Sunday 5:11 pm | Weekly content calendar | Social Media Manager | Next week's channel plan |
| Monday 8:47 am | Weekly plan | CEO | Priorities, delegated tasks, what needs you |

## Projects and starter tasks

- **Play Store Launch** (Engineer): release readiness checklist, store listing draft.
- **Platform** (Engineer): database path recommendation (full Supabase vs Laravel + Supabase), question CSV importer.
- **Question Bank** (Content Lead): RAS Rajasthan GK starter set (100 questions) plus the daily routines.
- **Social Channels** (Social Media Manager): app launch campaign plan plus the daily and weekly routines.
- **Company kickoff** (CEO): a first two-week plan and the list of what the team needs from you.

## Getting started

1. Install Paperclip on your server and sign in to Claude Code there (`claude` → log in with your Claude account, or set an Anthropic API key).
2. Import this company:

   ```sh
   paperclipai company import --from ./companies/scorelab
   ```

   or from GitHub: `paperclipai company import --from https://github.com/deepakscorelab/paperclip/tree/main/companies/scorelab`
3. Optional secrets: `ELEVENLABS_API_KEY` (voiceovers for the Social Media Manager) and `GH_TOKEN` (lets the Engineer open pull requests).
4. Open the CEO's **Company kickoff** task and let it run. Review drafts in your inbox each day.

## References

- [Agent Companies specification](https://agentcompanies.io/specification)
- [Paperclip](https://github.com/paperclipai/paperclip)
