---
name: play-store-release
description: Prepare the ScoreLab Android app for a Google Play release — build checks, store listing, privacy and data-safety answers, and testing tracks — without submitting it.
---

# Play Store release preparation

The founder submits the release. Your job is to make everything ready and list exactly what they need to click.

## 1. Build checks

- Release build is an Android App Bundle (`.aab`), signed with the upload key, using Play App Signing.
- `targetSdkVersion` meets Google Play's current minimum requirement (check the current requirement; it rises every year).
- Version code is higher than any previous upload; version name follows `major.minor.patch`.
- No debug flags, test endpoints, hard-coded API keys or logging of personal data.
- App opens, logs in, loads tests, submits answers and shows results on at least one small and one large phone.

## 2. Store listing (draft in English and Hindi)

- App name (max 30 characters), short description (max 80), full description (max 4000).
- Feature list: test practice for RAS/RPSC, UPSC and SSC, result analysis, weak-topic detection, bilingual content.
- Screenshot plan: 4–8 phone screenshots with captions; feature graphic 1024×500.
- Category (Education), contact email, website (scorelab.co.in) and privacy policy URL.

## 3. Policy and safety

- Privacy policy page that matches what the app actually collects.
- Data-safety form answers: list each data type collected (for example name, email, phone, test activity), why, whether it is shared, and whether it is encrypted in transit.
- Content rating questionnaire answers.
- Target audience: if users under 18 are allowed, flag the extra Families policy requirements to the founder.

## 4. Testing and rollout plan

- New personal developer accounts must run a closed test with enough testers for the required period before applying for production; check the current numbers in Play Console help and tell the founder.
- Internal testing track first, then closed testing, then a staged production rollout (for example 10% → 50% → 100%).

## Deliver

A release checklist document with every item marked done, to-do (with owner), or needs the founder. Move the task to review.
