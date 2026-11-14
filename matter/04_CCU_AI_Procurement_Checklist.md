# Coastal Commonwealth University
# Cloud AI-Agent Procurement Checklist
## Office of University Counsel / Strategic Sourcing
### Playbook Version 2.1 — 15 August 2026 (fictional institutional guidance)

*This checklist is a wholly fictional university playbook prepared for a synthetic counsel exercise. It is not the policy of any real institution, is not legal advice, and does not create authority to contract.*

---

## 1. Purpose and Application

This Checklist states the minimum legal, privacy, security, accessibility, and procurement positions that Coastal Commonwealth University ("**CCU**" or the "**University**"), a public institution of higher education organized under the laws of the Commonwealth of Virginia, expects to see in paper for a cloud AI-agent or similar software-as-a-service tool used in teaching, research, or administration.

It is intended for use by the Office of University Counsel, Strategic Sourcing, Information Security, and the sponsoring unit (here, Kelworth Lab) when reviewing a vendor's master agreement, data processing addendum, and service level agreement. **Material deviation from a P0 item is a block or a condition of award, not a business concession the laboratory may waive.** P1 items should be negotiated or risk-accepted only in writing by an official with delegated contracting authority. P2 items should be raised and documented.

This Checklist does not itself authorize signature, does not amend the University's actual (fictional) Board-approved terms, and does not substitute for unit-level data-classification review.

---

## 2. How Counsel Should Use This Document

1. Identify the contracting party (must be the University, not a laboratory or principal investigator).
2. Map each requirement below to a cited clause in the vendor's MSA, DPA, SLA, and order form (or record a gap).
3. Flag cross-document inconsistencies (for example, an MSA license that undercuts a DPA training prohibition, or an SLA "sole remedy" that undercuts breach or security obligations).
4. Produce recommended redlines, a short P0/P1/P2 issue list, and conditions of award.
5. Do not rely on marketing statements, security white papers, or verbal assurances in lieu of contract text.

---

## 3. Contracting Party, Authority, and Public-Institution Overlay

CCU is a public instrumentality. Vendor paper written for private commercial customers is often unworkable without amendment. Counsel shall confirm the following institutional constraints and shall not recommend signature on terms that exceed the University's legal authority.

**3.1 Contracting party.** The agreement must run to Coastal Commonwealth University. Individual faculty, staff, or students may not bind the University. Click-through terms presented to Authorized Users shall not amend the negotiated agreement.

**3.2 Sovereign immunity and damages.** The University does not, and as a matter of Virginia public-institution practice should not be asked to, waive sovereign immunity, consent to unlimited indemnities, or agree to liability that exceeds appropriations or statutory authorization. Mutual limitation-of-liability clauses may be considered, but they must not function as a waiver of immunity or as an obligation to indemnify a vendor for the vendor's own acts beyond what law permits.

**3.3 Choice of law and venue.** **Preferred: laws of the Commonwealth of Virginia, without a mandatory exclusive out-of-state venue.** Acceptable alternative: the agreement is silent on governing law and venue, or provides for venue in a Virginia state court of competent jurisdiction. **Not acceptable as a baseline: exclusive venue in another state (including Delaware or California), a jury-trial waiver that the University lacks authority to give, or a class-action waiver imposed on the University as a public body.** The paper must not contain a "no public-entity terms" clause that places the burden on the University to determine that it may lawfully agree to an out-of-state exclusive venue.

**3.4 Indemnifying a vendor.** **Public-procurement and appropriations constraints generally prohibit the University from defending or indemnifying a private vendor**, particularly on an open-ended basis and particularly for intellectual-property claims arising from the University's ordinary research use of the service (including prompts and research inputs) or for disputes among collaborators. A narrowly drafted infringement indemnity *from* the vendor for the vendor's service and models is expected. A one-sided customer indemnity of the vendor is a P0 defect.

**3.5 Auto-renewal, term, and appropriations.** **Automatic renewal of a multi-seat subscription is disfavored and, where Fees would commit funds beyond the current appropriation or fiscal period, may be unauthorized.** Acceptable structures include: a firm initial term with renewal only upon a written University purchase order or notice of intent to renew; or auto-renewal that the University may decline on not less than thirty (30) days' notice, with a reminder notice from the vendor at least ninety (90) days before renewal. A sixty (60) day non-renewal window that can cause a missed deadline, combined with vendor-set renewal pricing, is not acceptable without amendment.

**3.6 Purchase orders and vendor portals.** University purchase-order terms and required public-procurement certifications may not be declared "void" or "for administrative convenience only." Late-payment interest, gross-up, and collection-cost clauses must be conformed to applicable Virginia prompt-payment and collections rules.

**3.7 Public records.** The University is subject to the Virginia Freedom of Information Act and related public-records duties. Confidentiality clauses must permit disclosures required by law, with reasonable notice to the vendor where legally permitted. The vendor may not prohibit filing or production of the agreement when production is legally required.

**3.8 Assignment.** Assignment by the vendor, including in a change of control, requires prior written notice and, for assignment to a competitor, a sanctioned party, or an entity that cannot meet these Checklist requirements, University consent. The University must be able to assign internally among units or to a successor public entity without vendor consent.

---

## 4. Intellectual Property, Outputs, and Model Training

**4.1 Ownership (P0).** The University owns Customer Data, including prompts, inputs, uploaded code and notes, and Outputs generated for University users, subject only to the vendor's pre-existing rights in the service and models. Any assignment of Outputs must be clean and not undercut by a surviving vendor license.

**4.2 License to the vendor (P0).** Any license to the vendor shall be limited to hosting, processing, and displaying Customer Data and Outputs as necessary to provide the service to the University, to fix technical issues, and to generate de-identified, aggregated operational statistics that do not identify the University or any individual. **The vendor shall not receive a license to use Customer Data, prompts, Outputs, or telemetry to train, fine-tune, benchmark, or otherwise improve foundation models or the vendor's models or other products**, whether or not a particular record is classified as "personal data." A drafting gap between "Customer Data" and "Customer Personal Data" that permits training on research content is a P0 defect.

**4.3 Feedback and improvements.** Feedback licenses must be limited and non-exclusive. The University will not assign ownership of faculty or student suggestions in a way that could capture research ideas.

**4.4 Publication and open source.** The agreement must not restrict the University's right to publish research (other than a reasonable, short review for vendor confidential information that is not research result) or to release University-owned code under an open-source license of the University's choosing.

---

## 5. Privacy, FERPA, and Data Protection

**5.1 Data types.** The sponsoring unit must classify data before go-live. For Kelworth Lab's contemplated use: no PHI/HIPAA is in scope. **Student education records, or personally identifiable information from education records, may appear in researcher or research-assistant work product and shall be treated as FERPA-sensitive.**

**5.2 FERPA (P0 if education records may be present).** If the service will receive education records, the vendor must: (a) act as a "school official" with a legitimate educational interest, or under another FERPA-authorized condition documented in the agreement; (b) use the records only to provide the service to the University; (c) not redisclose personally identifiable information except as the University directs or FERPA permits; (d) maintain direct University control as FERPA requires, including through subcontracting limits; and (e) return or destroy education records at the University's direction. **Product-analytics, advertising, or similar subprocessors (including tools such as Mixpanel or comparable telemetry vendors) shall not receive education records or identifiable research-workspace content unless a documented FERPA-compatible justification exists and the University has approved that subprocessor in writing.**

**5.3 No training on personal or research data (P0).** The DPA and the MSA must consistently prohibit training and fine-tuning on Customer Data. A DPA prohibition that is overridden by an MSA license, or that applies only to "Customer Personal Data" while research code and notes are treated as train-able "Customer Data," fails this requirement.

**5.4 Subprocessor transparency (P0/P1).** The vendor shall provide a current subprocessor list, **advance notice of at least thirty (30) days before a new subprocessor processes University data** (emergency replacements excepted, with prompt after-the-fact notice), and a meaningful right to object. Notice periods that conflict across the MSA and DPA, or after-the-fact notice only, fail this requirement. Analytics subprocessors should be removable or excludable for research and education-records workloads.

**5.5 International transfers.** Standard contractual clauses, if needed, must be properly incorporated, with a United Kingdom addendum or Swiss addendum where relevant. Optional non-U.S. regions (including Singapore or other APAC regions) shall not be enabled without a separate University decision. Transfer-impact assessments remain the vendor's duty to support with documentation.

**5.6 Breach notice (P0/P1).** **Notice of a personal-data or education-records breach, or of a security incident affecting University data, must be given without undue delay and in any event within seventy-two (72) hours of the vendor becoming aware.** "Commercially reasonable efforts," "five business days," or an unbounded "without undue delay" with no outer limit is not sufficient. The University, not the vendor, determines its notifications to students, faculty, regulators, and partners, with vendor cooperation. Breach costs (forensics, notice, reasonable credit monitoring, and regulatory defense arising from the vendor's failure) shall be borne by the vendor and shall not be excluded from liability or confined to service credits.

**5.7 Customer instructions.** The DPA must allow the University to give reasonable documented instructions consistent with Applicable Data Protection Law and FERPA, not only instructions that fit the vendor's existing product settings.

---

## 6. Security and Data Residency

**6.1 Security commitment (P0).** The contract must contain affirmative security obligations (administrative, technical, and physical measures), not merely a reference to a policy the vendor may change, and not a disclaimer that reduces security to an "as is" service.

**6.2 Assurance packages (P0/P1).** **The vendor shall, on request and under NDA if needed, provide a current SOC 2 Type II report covering security and, preferably, confidentiality and availability, and a summary of an independent penetration test not more than twelve (12) months old.** A contractual ban on University-directed testing is acceptable only if the vendor's own independent testing and report-summary commitment is solid. The University's information-security office may still require a questionnaire and residual-risk acceptance.

**6.3 Data residency (P0).** **Customer Data at rest shall be stored in the United States.** Cross-border support access, global content-delivery, or telemetry that sends identifiable content or education records outside the United States requires prior University approval and a documented transfer mechanism.

**6.4 Encryption and access control.** Encryption in transit and at rest, multi-factor authentication for administrative access, tenant isolation, and logging of privileged access are required.

**6.5 Remedies for security failure (P0).** **Service credits shall not be the sole remedy for a security failure, personal-data breach, or loss of University data.** Availability credits may be the exclusive remedy for ordinary downtime that is not a security or data-protection event.

---

## 7. Liability, Insurance, and Remedies

**7.1 Liability floor (P0).** **The vendor's aggregate cap for ordinary claims shall be not less than the greater of (a) twelve (12) months' fees paid or payable under the applicable order or (b) Five Hundred Thousand United States Dollars (US $500,000).** A cap measured on three (3) months' fees is not acceptable for this spend class or for a research-data workload.

**7.2 Carve-outs (P0).** The cap shall not apply to (or shall be subject to a higher super-cap for) the vendor's willful misconduct or gross negligence; infringement indemnity; breach of confidentiality; and **data-protection or security failures, including forensic, notification, and regulatory costs.** Mutual consequential-damages waivers may be accepted if these carve-outs are preserved and if the waiver does not extinguish direct breach costs.

**7.3 Insurance (P0/P1).** The vendor shall maintain, at minimum: commercial general liability not less than $1,000,000 per occurrence / $2,000,000 aggregate; technology errors-and-omissions and cyber liability, including privacy-breach response, not less than $2,000,000 per claim; and workers' compensation as required by law. The University shall be named as an additional insured where commercially standard, and certificates and reasonably acceptable endorsements shall be provided on request and at renewal. Self-insurance requires prior review.

---

## 8. Term, Termination, Exit, and Handover

**8.1 Convenience termination.** The University should be able to terminate for convenience on not more than thirty (30) days' notice, with a refund of prepaid unused fees, or at least with a wind-down that does not require ninety (90) days of continued paid term after the University has decided to exit. A vendor right to terminate for convenience on thirty (30) days' notice is acceptable only if accompanied by a prepaid-fee refund and a usable handover period. Imbalanced periods (University 90 days / vendor 30 days) should be reversed or equalized.

**8.2 Exit and handover (P0).** **Upon termination or expiry, the University must have a commercially reasonable transition period of not less than ninety (90) days, and preferably one hundred eighty (180) days, of continued access or equivalent export assistance**, to retrieve Customer Data in a usable, documented, machine-readable format, followed by certified deletion. **A short export window (for example, thirty (30) days) followed by deletion obligations that cut off a required handover is a P0 defect.** Deletion schedules in the DPA must be aligned with, and must not undercut, the MSA transition period. Managed export assistance shall be available at a reasonable rate if self-service tools are insufficient. Parallel-run or transition assistance shall be available as an option, not disclaimed in full.

**8.3 Survival of training licenses.** No license to use Customer Data or Outputs for model training shall survive termination. Deletion must include a commitment not to retain University content in training corpora or, if extraction is not feasible for already-embedded weights, an express, narrow grandfather with no further training use of University data after the termination date.

---

## 9. Accessibility

**9.1 Standard (P0/P1).** **The service, including the administrative console and primary user interface, shall conform to the Web Content Accessibility Guidelines (WCAG) 2.1 Level AA and to Section 508 of the Rehabilitation Act, 36 C.F.R. Part 1194, as applicable to a public university's information and communications technology.** Virginia information-technology accessibility expectations shall also be met.

**9.2 Documentation.** The vendor shall provide a current Voluntary Product Accessibility Template (VPAT) or equivalent accessibility conformance report, and shall remediate material non-conformance on a documented timeline. Failure of accessibility is a service defect, not merely a support issue, and shall not be excluded from ordinary warranty or termination-for-cause rights.

**9.3 Guest and student users.** Collaborator and student research-assistant users must be able to use core workflows with assistive technology. Accessibility is an institutional civil-rights obligation and is not waivable by the laboratory.

---

## 10. Publicity, Audit, Export, and Operational Terms

**10.1 Name and logo (P0).** **The vendor shall not use the University's name, logos, marks, or the name of any laboratory or faculty member in publicity, customer lists (beyond a factual, unadorned text list if required), case studies, or press, without the prior written approval of University Communications** (or as required by law). An opt-out-after-the-fact right is not a substitute for prior consent. The University may make factual statements that it uses the service.

**10.2 Audit of the University.** Vendor audits of University use, if any, require not less than fifteen (15) business days' notice, must be limited to usage records reasonably necessary to confirm seat counts, must not include general access to research systems or facilities, and must not occur more than once per twelve (12) months absent a good-faith belief of material non-compliance. On-site audits of a public campus require additional coordination. The University should have a corresponding right to receive security reports (see Section 6.2).

**10.3 Export assistance.** The vendor shall reasonably cooperate with the University's export-control review (for example, by describing hosting locations, support-access locations, and available access-control features). A one-sided customer warranty with an express disclaimer of any vendor assistance is not acceptable for a research university, even if the unit does not presently intend to place export-controlled data on the service.

**10.4 SLA quality (P1).** For a research-production workload, target monthly uptime should be at least 99.9%, or 99.5% only with a meaningful credit scale and a cap of not less than 25% of the monthly fee for a severe outage. **Scheduled maintenance must be subject to a notice period (preferably 72 hours or more) and a reasonable monthly duration cap; uncapped, unannounced maintenance is not acceptable.** Force majeure should be narrowly drawn and should not excuse foreseeable infrastructure failures the vendor can contract for. Support for a laboratory with collaborators should include a severity-1 path with same-day response, not email-only weekday coverage with vendor-only severity classification. Service credits are not the exclusive remedy for data loss or security incidents (see Section 6.5).

---

## 11. Conditions-of-Award Snapshot (for counsel's memo)

| # | Requirement | Floor | Typical severity if missed |
| :--- | :--- | :--- | :--- |
| A | University ownership of prompts, inputs, Outputs | Clean ownership; license to vendor limited to providing the service | P0 |
| B | No model training on Customer Data | Consistent MSA + DPA prohibition; no "personal data only" gap | P0 |
| C | FERPA-capable terms if education records possible | School-official / no unauthorized redisclosure; no unapproved analytics subprocessor on education records | P0 |
| D | Exit / handover | ≥ 90 days (prefer 180) usable access or export, then certified deletion | P0 |
| E | Liability cap | ≥ 12 months' fees or US $500,000, with security/confidentiality carve-outs | P0 |
| F | Insurance | CGL $1M/$2M; cyber/E&O $2M; certificates on request | P0/P1 |
| G | Publicity | No name/logo use without prior written approval | P0 |
| H | Law / venue / immunity | Virginia or silent; no exclusive out-of-state venue; no unauthorized immunity waiver or vendor indemnity by the University | P0 |
| I | Data residency | US at rest; approved transfer tools if any cross-border access | P0 |
| J | Security assurance | SOC 2 Type II and pen-test summary on request | P0/P1 |
| K | Breach notice | In all events within 72 hours | P0/P1 |
| L | Accessibility | WCAG 2.1 AA and Section 508; VPAT on request | P0/P1 |
| M | Auto-renewal | Opt-in or University-friendly non-renewal / appropriations-safe | P1 |
| N | SLA | Meaningful credits; noticed, capped maintenance; credits not sole remedy for breach | P1 |

---

## 12. Document Control

| Field | Value |
| :--- | :--- |
| Owner (fictional) | Office of University Counsel, in consultation with Strategic Sourcing and Information Security |
| Version | 2.1 (15 August 2026) |
| Applies to | Cloud AI-agent and similar research/teaching SaaS procurements |
| Related (fictional) matter | CCU-OUC-2026-1147 — Kelworth Lab / AgentForge Cloud evaluation |

---

*CCU Cloud AI-Agent Procurement Checklist, Version 2.1. Fictional institutional guidance for AutoClaw Round 3 demonstration use only. Not legal advice.*
