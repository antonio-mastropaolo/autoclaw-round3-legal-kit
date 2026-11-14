# X Post Draft — AutoClaw Round 3 (Legal Practice)

**Account:** Antonio Mastropaolo (CS professor). **Personal benchmark — not an institutional endorsement, and not legal advice.** The matter is set at a fictional university (Coastal Commonwealth University) and involves only fictional parties; no real institution, department, or person is depicted.

**Required:** mention `@AutoClawAIer`, include `#BuiltWithAutoClaw`, original public post, and the four labelled sections **Context / Process / Result / Lessons**. **Do NOT include the AutoClaw account email anywhere in the post** — it goes in the Round 3 form only.

---

## Recommended: labelled single post

The four section labels are spelled out so a judge scanning for them finds them. ~2,013 characters plus the tags — needs a premium long post; if the account is not premium, use the 7-post thread below.

**CONTEXT** — Can an AI legal assistant do real in-house contract diligence, not a toy demo? I built a synthetic matter: a public university's School of Computing buying seats on a cloud AI-agent platform. Three vendor contracts (MSA + DPA + SLA) plus the university's own AI-procurement checklist, deliberately inconsistent *across* documents — a comfort sentence in one is quietly undone by a licence or an exclusive-remedy clause in another.

**PROCESS** — One pass through @AutoClawAIer on GLM-5.3-FlashX-Legal (Legal Assistant), uploading only the five source files — never my scoring notes. The prompt required pinpoint cites, a fact-vs-inference split, a dedicated cross-document contradiction pass, and a conditions table. It produced a long counsel memo (full run ~23,000 words) with a 25-row contradiction matrix (C-01–C-25), 45 clause-level redline asks (Markdown, ready to paste into a Word mark-up — no .docx ships), and a P0/P1/P2 conditions-of-award table.

**RESULT** — Verdict: do not proceed to a purchase order unless every P0 is agreed in writing. I scored it against a private 20-issue answer key written *before* the run and never shown to the agent: **19.5/20**, all six pre-registered cross-document conflicts mapped. A high score is not trust — my verification pass still caught a real failure: it flagged a telemetry-swept-into-training-licence trap as P0, then down-ranked the fix to "raise" in the very table a decision-maker signs. I moved it back to must-agree, and fixed a cite where it had **invented a clause number** (SLA §1.12 does not exist; the provision is MSA §1.12).

**LESSONS** — Grade the agent's decision *table*, not just its issue list — a trap can be found and still get down-ranked where it counts. And check every cite against the paper: the one fabricated pointer here was a cross-reference read in the wrong direction.

Synthetic, fictional parties, not legal advice. Kit (method card + full matter, re-runnable): https://github.com/antonio-mastropaolo/autoclaw-round3-legal-kit

@AutoClawAIer #BuiltWithAutoClaw

---

## Thread fallback — 7 posts, each under 280 (non-premium accounts)

### 1/7

**CONTEXT** — Can an AI legal assistant do real in-house contract diligence, not a toy demo? I built a synthetic matter: a university unit buying a cloud AI-agent platform. Vendor MSA + DPA + SLA plus the university's procurement checklist, inconsistent *across* documents.

### 2/7

The hard part isn't any single clause. A comfort sentence in one document is quietly undone by a licence clause, an exclusive-remedy sentence, or a precedence rule in another. A single-document redline misses every one of those.

### 3/7

**PROCESS** — One pass through @AutoClawAIer on GLM-5.3-FlashX-Legal. I uploaded only the five source files, never my scoring notes. Output: a ~23k-word counsel memo (full run), a 25-row contradiction matrix, 45 redline asks, a P0/P1/P2 conditions table.

### 4/7

**RESULT** — Verdict: no purchase order unless every P0 is agreed in writing. Scored against a private 20-issue key written before the run, never shown to the agent: **19.5/20**, all six pre-registered cross-document conflicts mapped.

### 5/7

**LESSONS** — A high score isn't trust. My verification pass caught it flagging a telemetry-into-training-licence trap as P0, then down-ranking the fix to "raise" in the table a decision-maker signs. Moved back to must-agree.

### 6/7

It had also **invented a clause number** — SLA §1.12 doesn't exist; the provision is MSA §1.12.

### 7/7

Grade the decision *table*, not just the issue list, and check every cite against the paper.

Synthetic, not legal advice. Kit: https://github.com/antonio-mastropaolo/autoclaw-round3-legal-kit

@AutoClawAIer #BuiltWithAutoClaw

---

*Synthetic demo materials. Fictional parties. Not legal advice, and not an institutional endorsement. Keep the AutoClaw account email out of the public post; submit it only in the Round 3 form.*
