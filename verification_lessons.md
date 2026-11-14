# Verification & Lessons

**Matter:** CCU-OUC-2026-1147 (synthetic) · Kelworth Lab / AgentForge Cloud
**Run:** AutoClaw Legal Assistant on GLM-5.3-FlashX-Legal, five source files, no scoring notes uploaded.

> **Synthetic demo. Not legal advice.**

---

## How the run was measured

Before the run, we wrote a **private 20-issue answer key** for this synthetic deal and locked it out of the upload folder. AutoClaw never saw it. After the run, an **independent verification pass** compared the memo's claims against the source contracts — not against the agent's own confidence — and scored what was caught, partial, missed, or invented against that fixed key.

**Result:** **19.5 / 20.** Nineteen issues caught in full with a correct pinpoint cite and a usable fix, one in part, none missed. All six pre-registered cross-document conflicts were mapped. Where a fact was not in the paper (e.g., whether a product-analytics subprocessor receives workspace content, whether a SOC 2 report exists), the memo raised an open question instead of guessing.

A high score is not the same as "trust it." The verification pass still surfaced defects worth correcting — two of them material, and one of them a genuinely invented clause number.

## The two corrections worth repeating

**1. A top-priority item that the agent then quietly down-ranked.** The memo correctly flagged, as a P0 contradiction (row **C-07**), that the vendor's definition of "Customer Data" sweeps in account and tenant **telemetry/usage data**, which then falls under a training/"improvement" license — and that even deleting the obvious training clause leaves a separate usage-data license (**R-31**) intact. But in the **conditions-of-award table the decision-maker actually signs**, the matching fix (tighten the usage-data definition; no model-improvement use) landed at **P2 "raise"** — a tradeable item. That is the inconsistency that matters: a trap can be *found* and still get *down-ranked* where it counts. **Correction (APPLIED):** the fix is now **P0-17, status "must-agree"**, sat with the other P0 rows and folded into the P0-1 must-agree set. The former P2 rows were renumbered **P2-1…P2-3** to close the gap.

**2. An invented clause number.** Contradiction row **C-02** (order of precedence) cited "**SLA §1.12**." That is worse than a wrong-document pointer: **SLA Section 1 ends at §1.6**, so `SLA §1.12` does not exist at all — the agent synthesized a clause number. The provision it was reaching for is **MSA §1.12** (the definition of "SLA" and its update mechanics). **Correction (APPLIED):** the cite in `MEMO_executive_and_contradictions.md` now reads **MSA §1.12**, and C-02's DPA column now also cites **DPA §13** (*Term; Order of Precedence; Governing Law*), which the agent had omitted entirely. The substance of the precedence analysis held; the pointer was fabricated.

Smaller conforming fixes were also made (breach-clock arithmetic that understated a timing gap, and a `Checklist §3.6` hook on the disputed-invoice condition that pointed at the PO-terms paragraph instead of `MSA §3.2`), but the two above are the reusable lessons.

## Takeaways

- **Score the conditions table, not just the issue list.** The operative artifact is the table a general counsel or VP forwards. Verify severity there, not only in the narrative.
- **Pre-register a private answer key and keep it away from the agent.** Grade the run after the fact against a fixed denominator; don't edit the key to match the output.
- **Check every cite against the paper.** The one citation error here was a cross-reference the agent read in the wrong direction — exactly the kind of thing a human pass is for.

*Synthetic matter. No real client, student, or vendor data. Not legal advice.*
