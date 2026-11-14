# X Post Draft — AutoClaw Round 3 (Legal Practice)

**Account:** Antonio Mastropaolo (CS professor, AURA Lab)
**Required:** mention `@AutoClawAIer`, include `#BuiltWithAutoClaw`, original public post, Context/Process/Result/Lessons. **Do NOT include the AutoClaw account email anywhere in the post.** Replace `[DEMO_URL]` with the public-kit link before posting.

---

## Thread version (2 posts)

### POST 1/2

Can an AI legal assistant do real in-house contract diligence — not a toy demo, a full vendor review?

I built a synthetic test: a public-university lab evaluating a cloud AI-agent vendor. Three contracts (MSA + DPA + SLA) plus the university's procurement checklist, deliberately inconsistent *across* documents so the hard issues only surface when you read them together.

I ran it through @AutoClawAIer on GLM-5.3-FlashX-Legal (Legal Assistant). One pass → a ~23k-word counsel memo: a 25-row cross-document contradiction matrix, 39 risk rows, 45 Word-ready redlines, a P0/P1/P2 conditions-of-award table, and 20 open questions. Verdict: do not proceed to a purchase order unless every P0 is agreed in writing.

#BuiltWithAutoClaw 🧵

### POST 2/2

How good was it, honestly?

I wrote a private 20-issue answer key *before* the run and never showed it to the agent. Scored afterward: 19.5/20 — all 6 cross-document conflicts mapped, 0 invented clauses or case law, and open questions raised where facts were genuinely missing.

But a high score ≠ trust it. My verification pass caught a real failure: the memo flagged a telemetry-swept-into-training-license trap as P0, then quietly down-ranked the fix to "raise" in the table a decision-maker actually signs. I moved it back to must-agree and corrected a wrong-document citation.

Lesson: grade the agent's decision *table*, not just its issue list — and check every cite against the paper.

Full reusable kit (method card + synthetic matter + redacted deliverables), all fictional, not legal advice: [DEMO_URL]

@AutoClawAIer #BuiltWithAutoClaw

---

## ALT — single-post version

I asked whether an AI legal assistant could run a full cloud-vendor contract review, not a toy demo. Built a synthetic university matter — MSA + DPA + SLA + procurement checklist, inconsistent across documents — and ran it through @AutoClawAIer on GLM-5.3-FlashX-Legal. One pass produced a ~23k-word counsel memo: cross-document contradiction matrix, 45 Word-ready redlines, a P0/P1/P2 conditions table, 20 open questions. I scored it against a private 20-issue answer key written before the run (never shown to the agent): 19.5/20, 0 invented clauses. My verification pass still caught one that matters — a P0 privacy trap it found but down-ranked in the sign-off table — which I corrected. Lesson: grade the agent's decision table, not just its issue list. Reusable kit (synthetic, not legal advice): [DEMO_URL] #BuiltWithAutoClaw

---

*Synthetic demo materials. Not legal advice. Keep the AutoClaw account email out of the public post; submit it only in the Round 3 form.*
