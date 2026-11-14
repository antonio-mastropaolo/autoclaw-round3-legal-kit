# University Cloud-AI Vendor Review Kit

**An AutoClaw Round 3 — Legal Practice entry.** A complete, reusable in-house-counsel workflow for reviewing a cloud AI-agent vendor's **MSA + DPA + SLA** against a public university's procurement playbook — run end to end in **AutoClaw (GLM-5.3-FlashX-Legal)**, then independently verified by a human.

> **Synthetic demo. Not legal advice.** Every party, contract, and fact in this kit is fictional (Coastal Commonwealth University / Kelworth Lab vs AgentForge Cloud). Nothing here is an agreement of, or advice about, any real university, vendor, Microsoft, OpenAI, Anthropic, Z.ai, or AutoClaw. Do not use these drafts in place of advice from qualified counsel.

---

## Context — the problem

A fictional public research lab (Kelworth Lab, at Coastal Commonwealth University) wants seats on a cloud AI-agent platform. The service will hold unpublished research, code, and possibly student/collaborator data. Counsel has a 14-day clock and the vendor's standard paper: a Master Subscription Agreement, a Data Processing Addendum (with annexes), and a Service Level Agreement, plus the university's own AI-procurement checklist.

The hard part is not any single clause. It is that a "comfort" sentence in one document is quietly undone by a license, an exclusive-remedy clause, or a precedence rule in another. A single-document redline misses that. The task: decide whether the university may proceed to a purchase order, and on exactly what conditions — with pinpoint cites, cross-document conflict mapping, Word-ready redlines, and a conditions-of-award table a VP for Research can sign.

## Process — how AutoClaw helped

1. **Built a synthetic matter packet** (this kit's `matter/` folder): intake brief, MSA, DPA, SLA, and a university procurement checklist — deliberately uneven and internally inconsistent, so a reviewer can practice real issue-spotting.
2. **Ran it through AutoClaw's Legal Assistant** on **GLM-5.3-FlashX-Legal**, uploading only the five source files (never any scoring notes). The master prompt required pinpoint section cites, a fact-vs-inference split, a dedicated cross-document contradiction pass, Word-ready redlines, a conditions-of-award table, and open questions — with an explicit instruction never to invent a statute, case, or clause number.
3. **AutoClaw produced a long counsel memo** (~23,000 words in the full run). What ships in this kit is about 14,000 words of it, and **every count below is checkable in the repo**: a 25-row cross-document contradiction matrix (C-01–C-25), 45 prioritized redline asks (MSA/DPA/SLA/Order Form), and a 30-item conditions-of-award table (P0-1–18, P1-1–9, P2-1–3) — disposition: *do not proceed to a PO unless every P0 is agreed in writing.* The full memo's per-issue risk rows (39) and open questions (20) were **not published**, so those two numbers are on faith, not checkable here.
4. **Scored and verified it by hand.** Before the run we wrote a **private 20-issue answer key** (never uploaded to the agent). After the run, a human checked each claim against the source paper.

## Result

- **Score vs the private key: 19.5 / 20** (19 caught in full with a correct cite and a usable fix; 1 in part; 0 missed). It mapped all 6 cross-document conflicts and, where it lacked a fact, raised an open question instead of guessing.
- **A verification pass still found real defects to correct** — most importantly a privacy item the memo flagged as a top-priority (P0) contradiction but then down-ranked in the conditions table the decision-maker actually signs, plus one wrong-document citation. **Both are corrected in this kit**: the usage-data fix is now condition **P0-17 ("must-agree")** instead of a P2 "raise", and the C-02 cite reads **MSA §1.12**. See `verification_lessons.md`.
- **A deliverable pack others can reuse:** executive recommendation + contradiction matrix, conditions-of-award table, a one-page method card, and the full synthetic matter so you can re-run it yourself.

## Lessons — what to reuse

- **Grade the agent's decision table, not just its issue list.** A sharp agent can *find* a trap and still *down-rank* its fix where it counts. We caught exactly that.
- **Use a pre-registered private answer key, and verify every cite against the paper.** The agent never sees the key; the key only scores the run afterward.
- **Cross-document reading is the whole game.** Precedence, exclusive-remedy, and surviving-license clauses can quietly defeat a protection stated elsewhere. Map conflicts across documents, not clause-by-clause.
- **Format is part of the work.** A conditions-of-award table a VP can forward beats a wall of prose.

---

## Files in this kit

| File | What it is |
| :--- | :--- |
| [`README.md`](README.md) | This overview (Context / Process / Result / Lessons). |
| [`METHOD_CARD.md`](METHOD_CARD.md) | One-page, forkable method for any public-institution cloud-AI vendor review. |
| [`MEMO_executive_and_contradictions.md`](MEMO_executive_and_contradictions.md) | Public excerpt of the AutoClaw memo: executive recommendation + the cross-document contradiction matrix. |
| [`conditions_of_award_public.md`](conditions_of_award_public.md) | The P0 / P1 / P2 conditions-of-award table and disposition. |
| [`redlines_priorities.md`](redlines_priorities.md) | The 45 prioritized redline asks (MSA / DPA / SLA / Order Form), clause-by-clause drafting language **ready to paste into a Word tracked-change mark-up** (no `.docx` ships). |
| [`verification_lessons.md`](verification_lessons.md) | How the run was scored and the specific errors the human verification pass corrected. |
| [`matter/`](matter/) | The full synthetic matter packet (intake brief, MSA, DPA, SLA, procurement checklist) — re-run it yourself. |

## How to reuse this kit

1. Rewrite `matter/00_matter_brief.md` and the checklist for *your* institution and data classification. Keep real client, student, or vendor data out.
2. Open AutoClaw → **Legal Assistant** → **GLM-5.3-FlashX-Legal**. Upload only the matter brief, MSA, DPA, SLA, and checklist.
3. Require pinpoint cites, a fact-vs-inference split, a cross-document contradiction matrix, prioritized redlines, and a conditions-of-award table.
4. Convert the redline asks into real Word tracked changes.
5. Score against your own pre-written answer key **after** the run — never upload it — and verify every cite against the paper before you rely on anything.

> **A note on the private answer key.** To measure the run honestly, we scored it against a private 20-issue answer key written **before** the run and never shown to the agent: the result was **19.5/20**. The key itself is not published, and it was not part of what AutoClaw reviewed.

*University Cloud-AI Vendor Review Kit · Prepared for AutoClaw Round 3 (Legal Practice). Synthetic materials only. Not legal advice.*
