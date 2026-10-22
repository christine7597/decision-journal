---
doc: scope
status: draft
---

# Decision Journal

A personal journal that locks in your predictions before you decide, then shows you how your confidence compares with how often you're actually right.

## The Unique Kernel
A live **Reality Check** on the new-decision form: as you type your confidence, it compares it with your actual hit rate on past decisions made at similar confidence — "You say 80%. At similar confidence you've been right 3 of 6 times (50%)." It stays quiet rather than invent a statistic when there isn't enough data.

Supporting it: predictions are **locked after saving**, so hindsight can't rewrite them, and "was the prediction right?" is recorded **separately** from "was the outcome good for me?" — being right and having a good outcome are different things.

## Who It's For
The learner: someone who wants honest feedback on their own judgment. Today, decisions get made and the original expectation is forgotten or quietly revised after the fact.

## The Core Loop
Predict → save (locked) → wait → review what actually happened → compare confidence with accuracy. You come back when a decision comes due for review, and every review sharpens the next Reality Check.

## Inspiration & Identity
Not discussed yet; `3-prd` covers look and feel.

## Why This Matters to the Learner
They want to know whether their confidence means anything, and to separate good judgment from good luck.

## What "Working" Looks Like
In about a minute on screen, in the learner's words:
1. Start with a clearly labeled sample journal.
2. Create a new decision, enter the expected outcome and confidence, and **see the Reality Check compare that confidence with past accuracy** (the "oh, that's cool" beat).
3. Save it and show that the prediction is locked.
4. Open a sample decision that is due for review, record what actually happened, and separately rate whether the prediction was right and whether the outcome was good.
5. Finish on the updated insights.

"The warning is the highlight, but I want the complete loop: predict, save, review, compare."

## The POC Boundary
- Front-end only, saved in the browser's localStorage. No login or backend.
- Sample journal of 8–10 fictitious entries, clearly labeled as sample data and never containing the learner's personal information. Any statistic drawn from it is labeled as sample data.
- New-decision form: decision, expected outcome, optional reasoning, life area, mood, confidence %, review interval (1 week / 1 month / 3 months).
- Live Reality Check based on past decisions at similar confidence.
- Prediction locked once saved.
- Decisions show as due for review once their review interval has passed.
- Outcome review: what happened; prediction came true (Yes / Partly / No); outcome was good for me (Good / Mixed / Bad).
- Journal list with filters: All / Open / Resolved, and life area.
- Insights: confidence compared with actual hit rate.

Open rule details for `3-prd`: what counts as "similar confidence," how "Partly" counts toward a hit, and the minimum number of past records before the Reality Check speaks up.

## Later
- Insight breakdowns by mood and by life area. Both are recorded on every entry from day one, but 8–10 samples spread across 6 moods and 6 areas would mean 1–2 records per group, which is exactly the invented-statistics trap.

## Explicitly Cut
- Login, accounts, sync, backend: unnecessary for a single-user journal; localStorage is enough to prove the loop.
- Real personal data in the demo: the public repo and video must use fictitious entries only.
