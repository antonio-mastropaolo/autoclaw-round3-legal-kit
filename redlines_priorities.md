# Redline Priorities (Word-ready) — AutoClaw Legal Run, verified

**Matter:** CCU-OUC-2026-1147 (synthetic) · Coastal Commonwealth University / AgentForge Cloud
**Source:** AutoClaw (GLM-5.3-FlashX-Legal) counsel memo, Section 4, checked against the paper.
**Use:** Convert these clause-by-clause asks into tracked-change `.docx` mark-ups (MSA, DPA, SLA).
**Classification:** Synthetic matter. Not legal advice. No scoring-key content appears in this file.

# 4. Tracked-change redline priorities (Word-ready)

Organized MSA, then DPA, then SLA, then Order Form. P0 first inside each document. Drafting language is intended to be pasted into a mark-up. Where a change must appear in more than one document to be effective, it is marked **[cross-document]**.

## 4.A Master Subscription Agreement

### MSA-R1 — Delete the training license — P0 — [cross-document with DPA-R1]

**Section:** §6.3(d), and the survival of §6.3(d) in §7.2 and §12.4.

**Current text (close paraphrase / short quote):** License grant includes "(d) to operate, develop, improve, benchmark, and train the Service, Provider's models, and Provider's other current and future products and services, including by using prompts, Customer Data, Outputs, and associated telemetry as training, fine-tuning, or evaluation material. The license in subsection (d) survives termination to the extent training or improvement artifacts have already been incorporated into Provider's models or systems and cannot reasonably be extracted."

**Proposed replacement:** Delete subsection (d) in its entirety. Add as a new §6.3(d) (or a new §6.3A):

> **(d) Prohibited uses.** Provider shall not use Customer Data, Outputs, prompts, inputs, embeddings, logs, traces, telemetry, or associated metadata to train, fine-tune, distill, benchmark, evaluate, or otherwise improve any foundation model, any Provider model, or any other Provider product or service, whether or not any such record is classified as personal data, and whether or not such record is de-identified or aggregated, except solely to generate de-identified, aggregated operational statistics that do not identify Customer or any Authorized User or data subject and that do not include Customer Data content. Provider shall not permit any Subprocessor or Third-Party Service to do so. This prohibition survives termination or expiry. If any Provider model as of the Effective Date has already been trained on Customer Data, Provider shall not use Customer Data for any further training after the Effective Date and shall, upon written request, describe in reasonable detail the category of such prior use. Provider shall not retain Customer Data in any training corpus.

**Why.** Snapshot B and Brief §5.2. A DPA-only ban fails because of MSA-first precedence (C-01, C-02). This language must appear in both documents.

### MSA-R2 — Clean Output ownership — P0

**Section:** §6.4.

**Current text:** Assignment "Subject to Section 6.3" and "conditioned on Customer's compliance with this Agreement."

**Proposed replacement:**

> **6.4 Outputs.** As between the Parties, Customer owns all right, title, and interest in and to Outputs generated for Customer, including Outputs generated from Customer Data or Authorized User prompts. Provider hereby assigns to Customer all right, title, and interest Provider may have in such Outputs, free and clear of any license under Section 6.3, subject only to (i) Provider's and its licensors' pre-existing rights in the Service and in any pre-existing or third-party material that may be reflected in Outputs, and (ii) Provider's ownership of the underlying models. Customer acknowledges that Outputs may be similar to outputs generated for other customers. Nothing in this Section 6.4 limits Customer's right to publish research results or to release Customer-owned code under an open-source license of Customer's choosing.

**Why.** Snapshot A. Removes the compliance clawback and the §6.3 subordinate license.

### MSA-R3 — Limit the Service license; define Usage Data; fix §6.1 and §6.6 — P0 — [cross-document]

**Section:** §6.1; §6.3 chapeau; new definition in §1; §6.6.

**Current text:** §6.3 chapeau is a broad "host, copy, process, transmit, display, adapt, and otherwise use." §6.1: Provider owns improvements "including any developments arising from Provider's use of Customer Data or Outputs in accordance with this Agreement." §6.6: usage data may be used "to operate, support, and improve Provider's products and for other lawful business purposes."

**Proposed replacement (chapeau and §6.1 / §6.6):**

> **6.3 License to Customer Data and Outputs.** Customer hereby grants to Provider a worldwide, non-exclusive, royalty-free, fully paid-up license (without right to sublicense except to Subprocessors engaged in accordance with the DPA) to host, copy, process, transmit, and display Customer Data and Outputs solely: (a) to provide, maintain, secure, and support the Service to Customer; (b) to prevent or address service, security, or technical issues affecting the Service as provided to Customer; and (c) to create de-identified, aggregated, or statistical operational data that does not reasonably identify Customer, any Authorized User, or any data subject and that does not include Customer Data content. No other license is granted.

> **6.1 Provider IP.** [Retain existing ownership of the Service, Documentation, and pre-existing models.] Provider owns improvements to the Service and to Provider's pre-existing models that Provider develops independently, without use of Customer Data, Outputs, prompts, or telemetry restricted by Section 6.3. No improvement, weight, or artifact trained or tuned on Customer Data or Outputs is Provider IP.

> **6.6 Usage Data.** "**Usage Data**" means technical and operational metrics about the configuration, performance, and use of the Service that do not include Customer Data content, Outputs, prompts, inputs, embeddings, file contents, or identifiable user content, and that do not identify Customer or any Authorized User. Provider may collect and use Usage Data solely to operate, secure, and support the Service to Customer. Usage Data is not a license to train or improve models.

**Why.** Closes the telemetry / usage-data back door (C-07, R-31) that would survive even if §6.3(d) were deleted.

### MSA-R4 — Feedback is a non-exclusive license, not an assignment — P0

**Section:** §6.5.

**Current text:** Provider may use feedback "without restriction or obligation, and Customer hereby assigns to Provider all right, title, and interest in such feedback."

**Proposed replacement:**

> **6.5 Feedback.** If Customer or an Authorized User provides suggestions or other feedback concerning the Service, Customer grants Provider a non-exclusive, royalty-free, worldwide license to use that feedback to improve the Service, provided that such use does not use, disclose, or train on Customer Data or Outputs and does not assign ownership of any research idea, method, or result. Customer does not assign any Intellectual Property Rights in Feedback.

**Why.** Checklist §4.3.

### MSA-R5 — Ninety / one-hundred-eighty day handover, then certified deletion — P0 — [cross-document with DPA-R3]

**Section:** §12.4; delete or recast §12.5.

**Current text:** 30-day request-or-lose export; professional-services rates for extra help; no transition assistance.

**Proposed replacement:**

> **12.4 Effect of Termination; Handover.** Upon termination or expiry: (a) the rights granted to Customer under Section 2.1 terminate, except as provided in this Section 12.4; (b) Customer shall pay all outstanding Fees, subject to any refund under this Agreement; and (c) **for a period of one hundred eighty (180) days (or such longer period as Customer requests) following the effective date of termination or expiry (the "Handover Period"), Provider shall continue to make the Service, or a read-only export environment functionally equivalent for retrieval purposes, available to Customer for the sole purpose of retrieving Customer Data and Outputs**, and shall upon request provide managed export assistance at no additional charge if the Service's ordinary export tools are insufficient to produce Customer Data and Outputs in a usable, documented, machine-readable format reasonably designated by Customer. Deletion clocks under the DPA shall not begin, and Provider shall not delete Customer Data or Outputs, until the Handover Period ends. After the Handover Period, Provider shall delete Customer Data and Outputs from production and backup systems in accordance with the DPA and shall, within thirty (30) days, provide a written attestation of deletion signed by a responsible officer or security lead. Provider shall not retain Customer Data or Outputs in any training corpus or model weight. Sections 1, 5, 6.1, 6.3, 6.5, 7, 9.3, 10, 11, 12.4, 13, 14, 16, 17, and 18 survive termination or expiry, provided that no license to use Customer Data or Outputs for training or improvement survives.

> **12.5 Wind-Down.** The Handover Period in Section 12.4 is a contractual transition obligation. Provider shall, at Customer's written request, provide reasonable additional transition assistance at rates not to exceed the professional-services rates stated on the applicable Order Form, if any, or otherwise at rates agreed in writing before the work is performed.

**Why.** Snapshot D; Brief §5.3. Opening ask is 180 days; the floor I will still accept is 90. If the vendor will give only 90, replace "one hundred eighty (180) days" with "ninety (90) days" and keep the rest.

### MSA-R6 — Delete or recast the Customer indemnity — P0

**Section:** §10.1.

**Current text:** Open-ended indemnity including prompts / Outputs IP and collaborator disputes.

**Proposed replacement:**

> **10.1 Customer Indemnity.** To the extent permitted by applicable law and by Customer's status as a public institution of higher education, Customer shall defend Provider against a third-party claim alleging that Customer Data, as provided by Customer, infringes a third party's copyright or trade secret, **but only to the extent the claim does not arise from Provider's Service, models, training methods, Outputs as generated by the Service, or Provider's breach of this Agreement or the DPA**. Customer has no obligation to indemnify Provider for (i) any allegation relating to prompts, inputs, or Outputs generated by the Service; (ii) any dispute among Customer, Authorized Users, guest collaborators, or other institutions; (iii) Provider's or a Subprocessor's acts or omissions; or (iv) any claim that would constitute a waiver of sovereign immunity or an obligation not authorized by applicable law. Nothing in this Section 10.1 requires Customer to indemnify Provider for Provider's own negligence, willful misconduct, or violation of law.

**Why.** Checklist §3.4 names a one-sided customer indemnity of the vendor a P0 defect. If counsel's confirmed authority is even narrower, delete §10.1 entirely and rely on §10.4.

### MSA-R7 — Widen the vendor indemnity; remove exclusive-remedy — P0

**Section:** §10.2 last sentence; §10.2 exclusions.

**Proposed replacement (operative changes):**

> Provider shall defend, indemnify, and hold harmless Customer and its regents, officers, employees, and agents from and against any third-party claim alleging that the Service, the models made available as part of the Service, or Provider's Materials infringe or misappropriate a third party's Intellectual Property Rights, and shall pay those damages, costs, and reasonable attorneys' fees finally awarded or agreed in a settlement approved by Customer. The defense obligation is not limited to U.S. copyright or U.S. patent. Provider has no obligation to the extent the claim arises solely from Customer Data as provided by Customer and not from the Service or Outputs, or from combination with software not provided by Provider, if the claim would have been avoided without that combination. If Provider believes the Service may be subject to an infringement claim, Provider shall (A) procure the right for Customer to continue using the Service, or (B) modify or replace the Service so that it is non-infringing with no material loss of functionality, and only if (A) and (B) are not commercially reasonably available, (C) terminate the affected Service and refund prepaid unused Fees for the terminated portion for the remainder of the then-current term, plus a pro-rata refund of any Handover Period that cannot be delivered. **This Section 10.2 is not Customer's exclusive remedy for Provider's breach of this Agreement, the DPA, or the SLA, or for Provider's negligence, willful misconduct, or violation of law.** Provider's obligations under this Section 10.2 are not subject to the cap in Section 11.2.

**Why.** Checklist §3.4; pairs with R-06 so the indemnity is not swallowed by MSA §11.2.

### MSA-R8 — Cap floor and carve-outs — P0 — [cross-document with DPA-R8]

**Section:** §11.2; §11.3.

**Proposed replacement:**

> **11.2 Liability Cap.** EXCEPT FOR THE CARVE-OUTS IN SECTION 11.3, EACH PARTY'S TOTAL, CUMULATIVE LIABILITY ARISING OUT OF OR RELATING TO THIS AGREEMENT SHALL NOT EXCEED THE GREATER OF (A) THE FEES PAID OR PAYABLE BY CUSTOMER UNDER THE APPLICABLE ORDER FORM DURING THE TWELVE (12) MONTHS IMMEDIATELY PRECEDING THE EVENT GIVING RISE TO THE CLAIM, OR (B) FIVE HUNDRED THOUSAND UNITED STATES DOLLARS (US $500,000). IF THE CLAIM ARISES BEFORE TWELVE MONTHS OF FEES HAVE ACCRUED, THE CAP SHALL BE THE GREATER OF THE FEES PAID OR PAYABLE TO DATE UNDER THAT ORDER FORM AND US $500,000.

> **11.3 Carve-Outs.** The limitations in Sections 11.1 and 11.2 do not apply to: (a) a Party's willful misconduct or gross negligence; (b) Provider's indemnification obligations under Section 10.2; (c) a Party's breach of Section 7 (Confidentiality); (d) Provider's breach of Section 8.2 or of the DPA, including any Personal Data Breach or Security Incident, and any related forensic, notification, credit-monitoring, restoration, and regulatory-defense costs; (e) Customer's payment obligations; and (f) liability that cannot be limited under applicable law. The exclusion of consequential damages in Section 11.1 does not apply to the foregoing carve-outs and does not exclude direct costs of reconstituting lost Customer Data. Nothing in this Section 11 waives sovereign immunity or creates an obligation exceeding Customer's appropriations.

**Why.** Checklist §7.1–7.2; snapshot E; Brief §5.5. On this spend, the floor is US $500,000.

### MSA-R9 — Credits are not exclusive for security / data-protection — P0 — [cross-document with SLA-R1, SLA-R2]

**Section:** §8.3.

**Proposed replacement:**

> **8.3 Downtime and Service Levels.** Provider's availability commitment, and Customer's exclusive remedy for ordinary unavailability that is not a Security Incident, Personal Data Breach, data-loss event, or breach of Section 8.2 or of the DPA, is set forth in the SLA. Service credits under the SLA are Customer's exclusive remedy **only** for that ordinary unavailability. Service credits are not Customer's exclusive remedy, and are not Provider's entire liability, for any Security Incident, Personal Data Breach, loss or corruption of Customer Data, breach of Section 8.2, breach of the DPA, or any other breach of this Agreement.

**Why.** Checklist §6.5; Brief §5.4. Must be said in the MSA, the DPA, and the SLA or the exclusive-remedy sentences will restore themselves.

### MSA-R10 — Governing law, venue, jury, class, public-entity — P0

**Section:** §17.1–17.5.

**Proposed replacement:**

> **17.1 Governing Law.** This Agreement shall be governed by the laws of the Commonwealth of Virginia, without regard to its conflict-of-laws principles, excluding the United Nations Convention on Contracts for the International Sale of Goods.

> **17.2 Venue.** The state courts of the Commonwealth of Virginia of competent jurisdiction, and the United States District Court for the District in which Customer's principal campus is located, shall have jurisdiction. Customer does not waive any venue, forum, or immunity protection available to it as a public institution. Provider consents to that jurisdiction.

> **17.3 No Jury or Class Waiver.** The Parties do not waive trial by jury. Customer does not waive any right to proceed in a representative capacity that a public institution may have. Any class-action waiver is deleted.

> **17.4 Injunctive Relief.** [Retain, limited to Intellectual Property Rights and Confidential Information, and without waiving immunity.]

> **17.5 Public-Entity Terms.** This Agreement is with a public institution of higher education organized under the laws of the Commonwealth of Virginia. Customer's sovereign immunity is reserved. Nothing in this Agreement requires Customer to determine that it may agree to a term it has not agreed to. Public-records disclosures required by law are permitted under Section 7 and Section 18.10. In the event of a conflict between this Agreement and a term that Customer is not authorized to accept, the unauthorized term is void and the remainder continues.

**Why.** Checklist §3.3; snapshot H. If vendor refuses Virginia, the acceptable fallback is silence on law and venue, or Virginia state court. Exclusive Wilmington plus jury plus class waiver is not a fallback.

### MSA-R11 — Affirmative security commitment — P0 — [cross-document with DPA-R7]

**Section:** §8.2.

**Proposed replacement:**

> **8.2 Security.** Provider shall implement and maintain administrative, technical, and physical safeguards appropriate to the risk, including at least the measures described in DPA Annex III, encryption of Customer Data in transit (TLS 1.2 or higher) and at rest, logical tenant isolation, multi-factor authentication for Provider administrative access, logging of privileged access, and a written information-security program reviewed at least annually. Provider shall not materially diminish those measures during a then-current Term. Upon written request, Provider shall provide (i) a current SOC 2 Type II report covering security and, preferably, confidentiality and availability, under NDA if needed, and (ii) a summary of an independent penetration test completed within the preceding twelve (12) months. Customer's Information Security office may submit a security questionnaire. Provider shall not be required to permit on-site testing of a multi-tenant production environment if the assurance package in this Section 8.2 is current and complete.

**Why.** Checklist §6.1–6.2; snapshot J; Brief §5.4. A changeable "description" is not a commitment.

### MSA-R12 — Subprocessor commercial term yields to the DPA — P0 — [cross-document with DPA-R4]

**Section:** §8.5.

**Proposed replacement:**

> **8.5 Subprocessors and Infrastructure.** Provider may engage Subprocessors only in accordance with DPA Section 7, as revised. Provider shall give Customer at least thirty (30) days' prior written notice before a new Subprocessor processes Customer Data (emergency replacements excepted, with prompt after-the-fact notice). Customer's objection rights, and the right to exclude product-analytics or advertising Subprocessors from education records and identifiable research-workspace content, are as set forth in the DPA. Continued use of the Service does not authorize a Subprocessor that Customer has objected to. In the event of conflict, the DPA controls this subject matter.

**Why.** C-05. The current "this Agreement controls" sentence is what makes the 15-day DPA notice unsafe.

### MSA-R13 — Insurance — P0 / P1

**Section:** New §11.5 (or new §10A).

**Proposed insertion:**

> **11.5 Insurance.** During the Term and for three (3) years thereafter, Provider shall maintain: (a) commercial general liability insurance of not less than US $1,000,000 per occurrence and US $2,000,000 aggregate; (b) technology errors-and-omissions and cyber liability insurance, including privacy-breach response, of not less than US $2,000,000 per claim; and (c) workers' compensation as required by law. Customer shall be named as an additional insured on the CGL policy where commercially standard. Upon request and at each renewal, Provider shall provide certificates of insurance and reasonably acceptable endorsements. Insurance is in addition to, and not in lieu of, Provider's liability under this Agreement.

**Why.** Checklist §7.3; snapshot F; Brief §5.5.

### MSA-R14 — Accessibility — P0 / P1

**Section:** New §9.4.

**Proposed insertion:**

> **9.4 Accessibility.** The Service, including the administrative console and primary user interface, shall conform to the Web Content Accessibility Guidelines (WCAG) 2.1 Level AA and to Section 508 of the Rehabilitation Act, 36 C.F.R. Part 1194, as applicable to a public university's information and communications technology, and to applicable Virginia information-technology accessibility expectations. Upon request, Provider shall provide a current Voluntary Product Accessibility Template (VPAT) or equivalent accessibility conformance report and shall remediate material non-conformance on a documented timeline. Failure of accessibility is a service defect and is not excluded from Section 9.2 or from termination for cause.

**Why.** Checklist §9; snapshot L.

### MSA-R15 — Publicity — P0

**Section:** §14.2.

**Proposed replacement:**

> **14.2 Provider Publicity.** Provider shall not use Customer's name, logos, Marks, or the name of any laboratory, school, or faculty member, in publicity, customer lists, websites, sales materials, press releases, case studies, or other promotional materials, without the prior written approval of Customer's University Communications office (or as required by law). A factual, unadorned text listing of Customer as a customer, with no logo or quotation, may be used only if Customer has not objected in writing within fifteen (15) days after Provider's request. Customer may make factual statements that it uses the Service.

**Why.** Checklist §10.1; snapshot G; Brief §5.7. Opt-out-after-the-fact is not a substitute.

### MSA-R16 — Purchase orders and payment — P1

**Section:** §5.2; §5.3.

**Proposed replacement:**

> **5.2 Payment Terms.** Invoices are due thirty (30) days from a correct invoice, or such longer period as applicable Virginia prompt-payment law requires, whichever is later. Customer may withhold payment of amounts disputed in good faith pending resolution. Interest on late undisputed amounts, collection costs, and any gross-up shall apply only to the extent permitted by applicable Virginia prompt-payment and collections rules. [Human to confirm current figures.]

> **5.3 Purchase Orders.** Customer may issue a purchase order. If an Order Form incorporates Customer's purchase-order terms or required public-procurement certifications, those terms and certifications control to the extent they do not reduce Provider's obligations under the DPA or the SLA. In the event of conflict, the negotiated Agreement controls except that public-procurement certifications required by law remain effective.

**Why.** Checklist §3.6.

### MSA-R17 — Auto-renewal — P1

**Section:** §12.1; conform §5.5.

**Proposed replacement:**

> **12.1 Term.** This Agreement commences on the Effective Date and continues until all Order Forms have expired or been terminated (the "**Term**"). Each Order Form has the initial subscription term stated therein. **The Order Form shall not automatically renew.** Renewal requires a written University purchase order or written notice of intent to renew. Provider shall provide a reminder notice at least ninety (90) days before the end of the then-current subscription term. If the Parties elect a fallback auto-renewal structure, Customer may decline renewal on not less than thirty (30) days' notice, and Provider shall give that reminder at least ninety (90) days before renewal. Renewal Fees shall not increase by more than [X]% unless agreed in a signed Order Form at least ninety (90) days before renewal.

**Why.** Checklist §3.5; snapshot M.

### MSA-R18 — Convenience termination — P1

**Section:** §12.2.

**Proposed replacement:**

> **12.2 Termination for Convenience.** Customer may terminate this Agreement or any Order Form for convenience by giving Provider at least thirty (30) days' prior written notice. Upon the effective date of such termination, Provider shall refund prepaid, unused Fees covering the period after the effective date, and Customer shall have the Handover Period in Section 12.4. Provider may terminate for convenience only on at least ninety (90) days' prior written notice, with a refund of prepaid unused Fees and the Handover Period.

**Why.** Checklist §8.1.

### MSA-R19 — Assignment — P1

**Section:** §16.1.

**Proposed replacement:**

> **16.1 Assignment.** Customer may assign this Agreement internally among its units or to a successor public entity without Provider's consent, upon notice. Provider shall not assign or transfer this Agreement, including by change of control, merger, or sale of assets, without Customer's prior written consent, except to an Affiliate that is not a competitor and that agrees in writing to be bound by this Agreement and the DPA. Provider shall give Customer at least thirty (30) days' prior written notice of any permitted assignment. Customer may withhold consent if the assignee is a competitor of Customer, a sanctioned party, or cannot meet the requirements of Customer's applicable procurement checklist.

**Why.** Checklist §3.8.

### MSA-R20 — Audit — P1

**Section:** §15.1.

**Proposed replacement:**

> **15.1** Provider or a third-party auditor designated by Provider may audit Customer's usage records reasonably necessary to confirm seat counts and usage limits, on at least fifteen (15) business days' prior written notice, during ordinary business hours, and not more than once in any twelve (12) month period unless Provider has a good-faith belief of material non-compliance. Audits shall not include general access to research systems or facilities. On-site audits of Customer's campus require additional coordination with Customer. Customer has the reciprocal right to receive the assurance reports in Section 8.2.

**Why.** Checklist §10.2.

### MSA-R21 — Export cooperation — P1

**Section:** §13.2.

**Proposed replacement:**

> **13.2 Customer Responsibility; Provider Cooperation.** Customer is responsible for determining whether Customer Data or Customer's research activities are subject to export-control or sanctions restrictions and for obtaining any required licenses. Provider shall reasonably cooperate with Customer's export-control review, including by describing hosting locations, support-access locations, and available access-control features (including guest-seat restrictions). Provider is not obligated to classify Customer Data or to apply for licenses on Customer's behalf.

**Why.** Checklist §10.3.

### MSA-R22 — Public records — P1

**Section:** §18.10; conform §7.1.

**Proposed replacement:**

> **18.10 Public Records.** Customer may record, file, and disclose this Agreement to the extent required by the Virginia Freedom of Information Act or any other law applicable to Customer. Where legally permitted, Customer shall give Provider reasonable prior notice of a compulsory disclosure and shall reasonably cooperate to seek confidential treatment of pricing and technical information. Provider shall not prohibit filing or production of this Agreement when production is legally required.

**Why.** Checklist §3.7.

### MSA-R23 — Publication / open source — P1

**Section:** New §6.7.

**Proposed insertion:**

> **6.7 Publication and Open Source.** Nothing in this Agreement restricts Customer's right to publish research results or to release Customer-owned code under an open-source license of Customer's choosing. Provider may require a reasonable, short review (not to exceed ten (10) business days) of a proposed publication solely to identify Provider Confidential Information that is not a research result.

**Why.** Checklist §4.4.

### MSA-R24 — Policy updates cannot rewrite P0s by continued use — P2

**Section:** §18.5.

**Proposed change:** Delete "or earlier if Customer agrees in writing or continues to use the Service for thirty (30) days after notice of a material change without objecting in writing." Replace with: updates take effect on the next renewal, or earlier if agreed in a writing signed by both Parties. Any change that materially reduces privacy, security, FERPA, residency, IP, liability, or accessibility protections is void as to Customer unless signed by an authorized University contracting official.

### MSA-R25 — Force majeure — P1

**Section:** §18.2.

**Proposed change:** Add: "Force majeure does not include failures of infrastructure that Provider could reasonably have contracted for, including failures of Provider's primary cloud host, and does not excuse a Security Incident or Personal Data Breach caused by Provider's or a Subprocessor's failure to maintain the measures required by Section 8.2 or the DPA." Conform SLA §3(e).

### MSA-R26 — Appropriations / immunity reservation — P0 (with R-10)

**Section:** New §17.6.

**Proposed insertion:**

> **17.6 Appropriations; Immunity.** Customer's payment obligations are subject to available appropriations. Nothing in this Agreement requires Customer to spend funds beyond the current appropriation or fiscal period, to waive sovereign immunity, or to indemnify Provider beyond what applicable law permits. If a court or attorney general of the Commonwealth determines that a term is unauthorized, that term is modified to the minimum extent necessary to make it authorized, or severed, and the remainder continues.

**Why.** Checklist §3.2, §3.5.

### MSA-R27 — Order of precedence — P0 — [cross-document with DPA-R10, SLA-R7]

**Section:** Preamble (conflict paragraph); §8.1.

**Proposed replacement of the preamble conflict sentence:**

> In the event of a conflict among those documents, the following order of precedence shall apply, unless an Order Form expressly and specifically states otherwise with respect to a numbered section of this Agreement: (i) the Order Form, with respect to seats, Fees, term dates, and any University-specific rider; (ii) the Data Processing Addendum, with respect to the processing of Customer Data, Customer Personal Data, education records, Subprocessors, international transfers, security measures, and Personal Data Breach or Security Incident notice; (iii) this Agreement; (iv) the SLA, solely with respect to the calculation of Uptime Percentage and the issuance of Service Credits for ordinary unavailability; and (v) any acceptable-use or similar policy posted on the Provider site, which shall not amend this Agreement, the DPA, or the SLA. No exclusive-remedy, "entire liability," or precedence sentence in this Agreement, the DPA, or the SLA shall be read to defeat a protection stated in a higher-ranking document on that subject.

**Why.** C-02. Without this, MSA-R1 / MSA-R9 will not stick.

---
## 4.B Data Processing Addendum

### DPA-R1 — Training ban on all Customer Data and Outputs — P0 — [cross-document with MSA-R1]

**Section:** §4 heading and §4.2–4.3.

**Proposed replacement:**

> **4. USE LIMITATIONS; NO TRAINING ON CUSTOMER DATA**
>
> **4.1** Provider shall not sell Customer Personal Data, as "sale" is defined under the CCPA, or otherwise disclose Customer Personal Data except as permitted by this DPA and the Agreement.
>
> **4.2** Provider shall not use Customer Data, Customer Personal Data, Outputs, prompts, inputs, embeddings, logs, traces, or telemetry to train, fine-tune, distill, benchmark, evaluate, or otherwise develop, improve, or generalize any machine-learning, foundation, or other model, and shall not permit Subprocessors or Third-Party Services to do so. This prohibition applies whether or not a record is classified as personal data and whether or not it is de-identified or aggregated, except solely for de-identified aggregated operational statistics that do not identify Customer, any Authorized User, or any data subject and that do not include Customer Data content.
>
> **4.3** Provider may process Customer Data only to provide, maintain, secure, and support the Service to Customer, including retrieval-augmented generation confined to Customer's tenant. This Section 4 survives termination. If extraction of already-embedded artifacts is not feasible, Provider shall not use Customer Data for any further training after the termination or expiry date and shall treat remaining weights as subject to the use limitation in this Section 4.

**Delete current §4.3** ("Nothing in this Section 4 limits any license or right granted to Provider under the Agreement…").

**Why.** C-01. This is the DPA half of snapshot B.

### DPA-R2 — FERPA school-official terms — P0

**Section:** New §2A (or new §5A).

**Proposed insertion:**

> **2A. Education Records; FERPA.** To the extent Customer Personal Data includes education records or personally identifiable information from education records as defined by the U.S. Family Educational Rights and Privacy Act ("**FERPA**"), Provider is a "school official" with a legitimate educational interest, engaged by Customer to provide the Service. Provider shall: (a) use education records solely to provide the Service to Customer; (b) not redisclose personally identifiable information except as Customer directs or as FERPA permits; (c) remain under the direct control of Customer with respect to education records, including Subprocessors; (d) not use education records for product analytics, advertising, or model training; and (e) return or destroy education records at Customer's direction, including during the Handover Period and at deletion. Provider shall not designate Mixpanel, Inc. or any other product-analytics, advertising, or telemetry Subprocessor to receive education records or identifiable research-workspace content unless Customer has approved that Subprocessor in a signed writing that documents a FERPA-compatible justification.

**Why.** Checklist §5.2; snapshot C; Brief §4–5. Human confirmation of CCU's current FERPA designation practice should sit with the University's FERPA officer; the contractual ask does not wait on that confirmation.

### DPA-R3 — Deletion aligned to handover — P0 — [cross-document with MSA-R5]

**Section:** §11.1–11.4.

**Proposed replacement:**

> **11.1** Upon termination or expiry, Provider shall not delete Customer Data or Customer Personal Data during the Handover Period in Section 12.4 of the Agreement. During the Handover Period, Provider shall make Customer Data and Outputs available for export in a usable, documented, machine-readable format, and shall provide managed export assistance at no additional charge if ordinary tools are insufficient. After the Handover Period, Provider shall delete Customer Data and Customer Personal Data from production systems within thirty (30) days, and from backups within one hundred twenty (120) days thereafter by ordinary overwrite, and shall provide the attestation in DPA §11.3.
>
> **11.2** Provider may retain Customer Personal Data only to the extent required by applicable law, subject to this DPA until deleted.
>
> **11.3** Upon written request, Provider shall provide a written attestation of deletion from a responsible officer or security lead. De-identified aggregated operational statistics that do not identify Customer or any individual may be retained. Provider shall not retain Customer Data, Outputs, prompts, or telemetry in any training corpus or model weight.
>
> **11.4** This Section 11 is aligned with, and does not cut off, the Handover Period. Extended managed transition beyond the Handover Period is available as described in MSA §12.5.

**Why.** C-04; snapshot D.

### DPA-R4 — Subprocessors: 30 days, objection, analytics exclusion — P0 — [cross-document with MSA-R12]

**Section:** §7.3–7.4; Annex II notes.

**Proposed replacement of §7.3:**

> **7.3** Provider shall maintain a current list of Subprocessors in Annex II. Provider shall provide Customer with written notice of the addition or replacement of a Subprocessor at least thirty (30) days before the new Subprocessor begins processing Customer Data or Customer Personal Data (or as soon as reasonably practicable, and in any event within forty-eight (48) hours, in the case of an emergency replacement, followed by the same 30-day objection window). Customer may object to a new Subprocessor on reasonable data-protection, security, FERPA, or residency grounds by written notice within fifteen (15) days of Provider's notice. If the Parties cannot resolve the objection, Customer may (i) terminate the affected Service with a refund of prepaid unused Fees, or (ii) continue the Service and require Provider to process the affected data without the objected-to Subprocessor. Product-analytics, advertising, and similar Subprocessors, including Mixpanel, Inc., shall not receive education records or identifiable research-workspace content unless Customer has approved that Subprocessor in a signed writing. Customer's failure to object within the objection period authorizes the Subprocessor for uses other than those excluded in the preceding sentence.

**Why.** C-05, C-10, R-13, R-14.

### DPA-R5 — Breach notice: 72 hours from awareness; DPA controls — P0 — [cross-document with SLA-R3]

**Section:** §10.1; add a controls sentence.

**Proposed replacement of §10.1 first sentence, plus new §10.4:**

> **10.1** Provider shall notify Customer of a Personal Data Breach or Security Incident without undue delay, and in any event within seventy-two (72) hours, after becoming aware of it. "Aware" means Provider or a Subprocessor knows or reasonably should know of the event. Provider's determination, confirmation, or classification is not a precondition to the clock. Notice shall be sent to the security or privacy contact designated on the Order Form and to any additional contact Customer designates in writing.

> **10.4** This Section 10 controls over any conflicting notice period, trigger, or "in lieu of" sentence in the Agreement or the SLA, including SLA Section 5.1. Notice under this Section 10 is not a Service Credit and does not limit Customer's remedies.

**Why.** C-06, C-09; snapshot K.

### DPA-R6 — US residency; no Singapore without a signed University decision — P0

**Section:** §8.1; §8.3; new §8.5.

**Proposed insertion:**

> **8.5 Data Residency.** Customer Data and Customer Personal Data at rest shall be stored in the United States. Provider shall not enable any non-U.S. region, including the optional Republic of Singapore configuration, without Customer's prior written decision stated on an Order Form. Cross-border support access, global content-delivery that processes identifiable Customer Data or education records, or telemetry that sends such content outside the United States requires Customer's prior written approval and a documented transfer mechanism. Cloudflare, Inc. global-edge processing of identifiable Customer Data or education records is not authorized unless so approved.

**Why.** Checklist §6.3; snapshot I; C-11.

### DPA-R7 — Assurance package — P0 / P1

**Section:** §6.2.

**Proposed replacement:**

> **6.2** Upon written request, and under NDA if needed, Provider shall make available to Customer (i) its then-current SOC 2 Type II report covering security and, preferably, confidentiality and availability, and (ii) a summary of an independent penetration test completed within the preceding twelve (12) months. Provider shall refresh each on request not more than once per twelve (12) month period, and promptly after a Personal Data Breach. On-site inspections are not required if those materials are current, except where required by Applicable Data Protection Law.

**Why.** Checklist §6.2; snapshot J.

### DPA-R8 — Liability cites the revised cap and carve-outs — P0 — [cross-document with MSA-R8]

**Section:** §12.

**Proposed replacement:**

> **12. LIABILITY** The limitations of liability in Section 11 of the Agreement, as revised to provide a floor of the greater of twelve (12) months' fees paid or payable or US $500,000 and to carve out willful misconduct, gross negligence, confidentiality, indemnities, and data-protection or security failures including forensic, notification, and regulatory costs, apply to this DPA. Service Credits are not the exclusive remedy for a Personal Data Breach, Security Incident, or loss of Customer Data. To the extent Applicable Data Protection Law requires a different result that cannot be waived by contract, that law controls.

**Why.** C-08. As written, DPA §12 incorporates the three-month cap and the "no forensic / notification costs" sentence.

### DPA-R9 — Customer instructions — P1

**Section:** §3.2.

**Proposed change:** Add: "Customer may give reasonable documented instructions consistent with Applicable Data Protection Law and FERPA, including instructions to disable product-analytics processing of education records and identifiable research-workspace content, to restrict processing to United States regions, and to limit Subprocessors. Provider shall not decline an instruction solely because it is not a pre-existing product setting, unless it would require a material architectural change that Provider does not offer to any customer of comparable size."

**Why.** Checklist §5.7.

### DPA-R10 — Precedence — P0 — [cross-document with MSA-R27]

**Section:** DPA preamble.

**Proposed replacement of the conflict sentence:**

> In the event of a conflict between this DPA and the Agreement with respect to the processing of Customer Data, Customer Personal Data, education records, Subprocessors, international transfers, security measures, or Personal Data Breach or Security Incident notice, this DPA controls. This DPA does not limit any protection in the Agreement that is more protective of Customer. The Agreement's intellectual-property licenses, as revised, and the SLA's credit arithmetic, do not override this DPA.

**Why.** C-02.

### DPA-R11 — UK / Swiss addenda; transfers — P2 (unless a University decision requires them)

**Section:** §8.3.

**Proposed change:** Keep the "separate addendum if and when required" structure, but add: "If Customer identifies a transfer that requires a UK International Data Transfer Addendum, a Swiss addendum, or another approved tool, Provider shall execute that addendum within a commercially reasonable time and in any event before the transfer occurs." Do not enable Singapore.

---

## 4.C Service Level Agreement

### SLA-R1 — Credits are exclusive only for ordinary downtime — P0 — [cross-document with MSA-R9]

**Section:** Preamble, first exclusive-remedy paragraph.

**Current text:** Credits are sole and exclusive remedy and entire liability for Uptime failure, unavailability, degradation, latency, support failure, **and for any Security Incident or Personal Data Breach to the extent it manifests as unavailability, degradation, or loss of access**.

**Proposed replacement:**

> The Service Credits described in this SLA are Customer's sole and exclusive remedy, and Provider's entire liability, **solely for failure to meet the Uptime Percentage caused by ordinary unavailability that is not a Security Incident, Personal Data Breach, data-loss or data-corruption event, or a breach of Section 8.2 of the Agreement or of the DPA**. Service Credits are not the exclusive remedy, and are not Provider's entire liability, for any Security Incident, Personal Data Breach, loss or corruption of Customer Data, or any other breach of the Agreement or the DPA. This SLA does not limit any remedy in the Agreement or the DPA.

**Why.** C-03; Checklist §6.5.

### SLA-R2 — Delete exclusive-remedy for security / data issues — P0

**Section:** §5.2.

**Proposed replacement:**

> **5.2 Remedies.** If a Security Incident, Personal Data Breach, data loss, or data corruption results in unavailability or in a failure of Customer to access Customer Data, Customer's remedies include the remedies in the Agreement and the DPA, in addition to any Service Credit that may be available under Section 4. Provider shall, upon request, provide a root-cause analysis. Nothing in this Section 5 limits Provider's liability for forensic, notification, credit-monitoring, restoration, or regulatory costs to the extent those costs are carved out of Section 11 of the Agreement as revised.

### SLA-R3 — Security-incident notice: 72 hours from awareness; not in lieu of DPA — P0 — [cross-document with DPA-R5]

**Section:** §1.4; §5.1.

**Proposed replacement:**

> **1.4** "**Security Incident**" means any unauthorized access to, or unauthorized acquisition, use, disclosure, loss, alteration, or destruction of, Customer Data or Customer Personal Data, including an incident at a Subprocessor, that affects or is reasonably likely to affect Customer's tenant. Provider's determination, confirmation, or classification is not a precondition to notice.

> **5.1 Notice.** Provider shall notify Customer of a Security Incident in accordance with DPA Section 10, without undue delay and in any event within seventy-two (72) hours after becoming aware. Notice under this Section 5 is in addition to, and not in lieu of, notice under the DPA. Provider has no obligation under this SLA to notify Customer of unsuccessful or attempted attacks that do not meet the Security Incident definition, or of incidents affecting only other customers and not Customer Data.

### SLA-R4 — Maintenance notice and cap — P1

**Section:** §3(a).

**Proposed replacement:**

> **(a) Scheduled Maintenance.** Unavailability for Scheduled Maintenance announced at least seventy-two (72) hours in advance, performed during a Customer-designated or mutually agreed window, and not exceeding eight (8) hours in any calendar month in the aggregate. Notice that is late or incomplete does not convert uncapped maintenance into Excused Downtime. Emergency Maintenance under subsection (b) remains excused if Provider reasonably determines it is necessary to protect security or integrity, with notice as soon as reasonably practicable.

### SLA-R5 — Uptime and credit scale — P1

**Section:** §2.1; §4.1–4.2; §4.4.

**Proposed replacement (opening ask):** Target monthly Uptime Percentage of 99.9%. Credit scale: <99.9% ≥99.5% = 10%; <99.5% ≥99.0% = 25%; <99.0% = 50%; monthly cap 100% of the Monthly Subscription Fee. Delete SLA §4.4's "not a material breach" / "no termination right" sentence, or qualify it: "Failure to meet the Uptime Percentage is not by itself a material breach, provided that chronic failure (Uptime Percentage below 99.0% in any three (3) months of a six (6) month period, or below 98.0% in any month) is a material breach entitling Customer to terminate and to a refund of prepaid unused Fees."

**Fallback I will still accept:** 99.5% target, but credit cap not less than 25% of the monthly fee for a severe outage (Checklist §10.4), plus the chronic-failure termination right, plus SLA-R1.

### SLA-R6 — Severity-1 path — P1

**Section:** §6.1–6.3.

**Proposed change:** Add a severity-1 path with same-day (calendar) first response, not limited to 9–5 Pacific email. Customer's good-faith severity classification controls unless Provider reasonably reclassifies with a written explanation. A research-deadline coincidence is a relevant factor, not an automatic disqualifier.

### SLA-R7 — Precedence — P0 — [cross-document]

**Section:** SLA preamble, second paragraph.

**Proposed replacement:**

> If this SLA conflicts with the Agreement or the DPA, the Agreement's preamble as revised controls, except that this SLA controls solely the calculation of Uptime Percentage and the issuance of Service Credits for ordinary unavailability. This SLA does not replace DPA Section 10 notice, DPA Section 6 security measures, or any DPA or Agreement remedy for a Security Incident, Personal Data Breach, or loss of Customer Data.

---

## 4.D Order Form (not in the file — required inserts)

The Order Form is not in the packet. The following must appear on it or in a University rider. I am not inventing commercial numbers.

- Customer legal name: **Coastal Commonwealth University**. Not a department, not a research group, not a PI.
- Seats: 20 researcher seats; 5 named collaborator guest seats, limited to project workspaces designated by the laboratory director.
- Initial term: twelve months; **no auto-renewal** (MSA-R17).
- Fees: academic catalog rate consistent with ~US $60,000 first-year, exclusive of taxes; exemption certificate path (MSA §5.4).
- **US-only data at rest.** Singapore / non-U.S. regions not enabled.
- Mixpanel / product analytics **not authorized** for education records or identifiable research-workspace content.
- University PO number and any required public-procurement certifications are effective terms (MSA-R16).
- Security / privacy / FERPA notice contacts, including a 24-hour reachable security contact for DPA §10.
- No publicity use of CCU name or marks without University Communications approval.
- Any Third-Party model endpoint the laboratory intends to enable, listed and brought under DPA §7.


*Redline priorities, University Cloud-AI Vendor Review Kit. Synthetic matter only. Not legal advice.*
