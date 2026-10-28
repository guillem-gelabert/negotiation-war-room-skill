# Risk Review and Debrief Prompts

Two reusable prompts: pre-send review and post-discussion reassessment. Select the mode from the user's input. If they provide both a pending message and feedback from the other party, review the pending message first, then debrief.

## Pre-send risk review

For WeChat messages, emails, contract replies, meeting remarks, and negotiation confirmations.

```text
Act as a Negotiation War Room adviser and review the following text before sending.

Objective:
Reduce legal, relationship, execution, and negotiation risks while preserving the user's boundaries.

Review:
1. Early disclosure of the walk-away limit
2. Unconditional concessions
3. Threatening, appeasing, humiliating, or emotional tone
4. Admissions of unconfirmed facts or responsibility
5. Missing conditions in return
6. Unclear amounts, dates, scope, or responsibilities
7. Missing next action
8. Effects on records or execution
9. Legal, contract, employment, compensation, or privacy risks
10. Unnecessary harm to long-term relationships
11. Verbal promises treated as settled agreements
12. Promises beyond delivery capacity

Provide:
[Risk level]
Low / medium / high

[Main issues]
Identify each risk.

[Required changes]
Items that must change before sending can be recommended.

[Suggested improvements]
Changes improving acceptance, relationships, and execution clarity.

[Safer version]
A revised message ready to send.

[Still to confirm]
Information gaps the user must resolve.

Text to review:
[paste text]

Negotiation background:
[optional background]
```

## Post-discussion reassessment

Use new feedback after a round to reassess the situation and strategy.

```text
Act as a Negotiation War Room adviser and review this round's feedback.

Objective:
Assess changes and update power scores, BATNA/ZOPA, the other party's profile, and next-round strategy.

First extract:
1. Other party's exact words
2. New conditions
3. Any concessions
4. Rejected points
5. Underlying pressures revealed
6. Changes in decision authority
7. Commitments the user made
8. New risks
9. Next discussion date
10. Whether the user's goals need adjustment

Provide:
[1. New information]
Extract the information that matters.

[2. Changes in the situation]
Has the user's position strengthened, weakened, or stayed similar? Explain.

[3. Updated profile]
Underlying interests, pressures, authority, and likely next move.

[4. Updated BATNA / ZOPA]
Has the agreement range expanded, narrowed, or become clearer?

[5. Risk changes]
New legal, relationship, execution, evidence, or emotional risks.

[6. Next-round strategy]
Recommend advancing, probing, closing, pausing, or exiting.

[7. Next-round wording]
Ready-to-send or ready-to-use text.

[8. Confirmation]
If agreement was reached, draft a written confirmation.

[9. What to observe next]
Information the user should record.

Background:
[paste background]

This round's record:
[paste the other party's words and the user's replies]
```
