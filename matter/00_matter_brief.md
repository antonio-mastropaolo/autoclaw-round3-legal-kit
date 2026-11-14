# Matter Brief — School of Computing Evaluation of AgentForge Cloud

**Coastal Commonwealth University — Office of University Counsel**
**Confidential — Attorney-Client Privileged / Attorney Work Product (fictional)**

| Field | Detail |
| :--- | :--- |
| Matter no. | CCU-OUC-2026-1147 (synthetic) |
| Intake date | 12 November 2026 |
| Requesting unit | School of Computing |
| Assigned counsel | Simone Alvarez, Associate University Counsel (fictional) |
| Business owner | Prof. Julian Hartwell, Principal Investigator (fictional) |
| Procurement lead | Thomas Reeve, Director of Strategic Sourcing (fictional) |
| Authorizing official (anticipated) | Dr. Priya Nandakumar, Vice President for Research (fictional) |
| Target PO date | 26 November 2026 (fourteen (14) calendar days from intake) |
| Classification | Synthetic demo packet — not a real matter; not legal advice |

---

## 1. Purpose of this Intake

Counsel is asked to review the vendor's standard paper — Master Subscription Agreement v3.0, Data Processing Addendum, and Service Level Agreement — and to advise whether Coastal Commonwealth University ("**CCU**" or the "**University**") may proceed to a purchase order for AgentForge Cloud seats for the School of Computing, and on what conditions. The laboratory needs a cleared path to purchase within fourteen (14) days. This brief states the commercial goal, the data that will be placed on the service, the University's must-haves, and the questions counsel should resolve before signature.

This intake does not authorize signature. No commitment has been made to AgentForge Inc.

---

## 2. Parties

**Customer / Institution.** Coastal Commonwealth University, a public institution of higher education organized under the laws of the Commonwealth of Virginia, with its principal campus at 100 Tidewater Green, Harbor Point, Virginia 23510 (fictional address). The contracting party must be the University, not the laboratory and not any individual investigator.

**Sponsoring unit.** The School of Computing, a degree-granting academic unit. The work is conducted by Prof. Hartwell's research group, which studies multi-agent systems, human-AI collaboration, and research-workflow automation, and collaborates with investigators at other institutions under data-use and visiting-researcher arrangements. **Note the structural point:** the group is not a legal entity — the contracting party is the University (above), and the group is merely the requesting unit.

**Provider.** AgentForge Inc., a Delaware corporation with a stated principal place of business at 880 Ember Wharf, Suite 14, San Francisco, California 94107 (fictional), offering a multi-tenant cloud service branded "**AgentForge Cloud**."

**Paper under review.** AgentForge Cloud Master Subscription Agreement, Version 3.0 (1 November 2026); Data Processing Addendum; Service Level Agreement. The University's internal requirements are stated in the CCU Cloud AI-Agent Procurement Checklist (Office of University Counsel / Procurement, fictional playbook).

---

## 3. Commercial Goal

The School of Computing seeks to subscribe to AgentForge Cloud for a twelve-month initial term, as follows:

- **Twenty (20) researcher seats** for CCU faculty, staff, postdoctoral researchers, and enrolled graduate and undergraduate research assistants assigned to the group's projects; and
- **Five (5) collaborator guest seats** for named investigators at other institutions who participate in the group's projects under existing collaboration agreements, with access limited to project workspaces designated by the laboratory director.

Approximate first-year spend, at the vendor's quoted academic catalog rate, is Sixty Thousand United States Dollars (US $60,000), exclusive of taxes, overage, and optional professional-services hours. Seats will be used to draft and iterate research code and notes, run agent workflows against laboratory repositories, and coordinate tasking among researchers and guests. The service will not be used for clinical care, for the University's official student-information system, or as the system of record for sponsored-award financials.

A purchase order is requested by **26 November 2026**, to align with a sponsored-project milestone and with seat provisioning before the spring research cycle. Counsel's mark-up, issue list, and recommended conditions of award are needed in time for negotiation within that window.

---

## 4. Data Types and Regulatory Overlay

The laboratory has described the following categories of content that would be uploaded, prompted, stored, or generated on the service:

| Category | Expected? | Notes for counsel |
| :--- | :--- | :--- |
| Source code, scripts, configuration, and technical documentation | Yes | May include unpublished methods and code that the University intends to own or later release under an open-source license of its choosing. |
| Research notes, experiment logs, literature summaries, and draft papers | Yes | May include pre-publication results and collaborator contributions. |
| Protected health information / HIPAA | **No** | Not in scope. The laboratory has confirmed that clinical or covered-component data will not be placed on the service. If that changes, this matter must be reopened. |
| Student education records (FERPA) | **Possibly** | Guest and researcher seats may be used by or with respect to enrolled students (for example, research-assistant work product, grades or evaluations incidental to a supervised project, or identifiable student-authored code). Treat as **FERPA-sensitive**. The vendor paper must be capable of supporting a school-official or other authorized FERPA use, with appropriate use, disclosure, and subprocessors limits. |
| Government-funded research data; export-controlled technical data | Not anticipated as a primary use, but not excluded by lab practice | Confirm export and publication-restriction handling. |
| Personal data of faculty, staff, students, and external collaborators (accounts, usage logs, workspace content) | Yes | Subject to the DPA and to University privacy policy. |

Counsel should assume that "Customer Data" will include both personal data and non-personal research intellectual property, and should not allow a drafting gap between those categories to authorize model training or secondary use.

---

## 5. Must-Haves (Do-Not-Proceed Without)

The following positions are required by the University's AI-procurement playbook and by the group's intended use. Material deviation should be treated as a block or as a condition of award, not as a business concession for the laboratory to waive.

1. **Intellectual property.** The University owns prompts, inputs, and outputs created by or for CCU users, and all Customer Data. Any license to the Provider is limited to providing the service to CCU. No broad license for service improvement that swallows research IP.
2. **No training on Customer Data.** The Provider shall not use Customer Data, prompts, or outputs to train, fine-tune, or otherwise improve foundation models or the Provider's models, whether or not the content is classified as "personal data."
3. **Exit and handover.** Upon termination or expiry, CCU must have a commercially reasonable transition period (not less than ninety (90) days, and preferably one hundred eighty (180) days) to export Customer Data in a usable format, followed by certified deletion. Deletion shall not cut off a required handover.
4. **Security.** Written security commitments (not merely a cross-reference), including SOC 2 Type II and a penetration-test summary on request, US data residency, encryption in transit and at rest, and a hard breach-notice period. Service credits shall not be the sole remedy for security failure or for downtime that causes research loss.
5. **Liability cap.** A meaningful cap: not less than twelve (12) months' fees paid or payable under the applicable Order, or Five Hundred Thousand United States Dollars (US $500,000), whichever is greater, with customary carve-outs (including data-protection and confidentiality breaches, indemnities, and willful misconduct / gross negligence). Insurance evidence consistent with University vendor requirements.
6. **Subprocessor transparency.** A current list, advance notice of material changes, and the right to object. Analytics tools that are unnecessary for a research workload should be flagged (particularly if they would receive education-records or research content).
7. **Publicity and branding.** No use of the University's name, marks, or logos without prior written approval of University Communications (or as required by law).
8. **Institutional terms.** Choice of law and venue acceptable to a Virginia public institution (Virginia law, or silent / negotiated; no exclusive out-of-state venue that waives sovereign-immunity or venue protections). Assignment, audit, auto-renewal, and termination rights must be workable for public procurement.

---

## 6. Timeline and Deliverables Requested of Counsel

| Date | Action |
| :--- | :--- |
| 12 November 2026 | Intake opened; vendor paper received. |
| 18 November 2026 | Counsel issue list, cross-document contradiction map, and recommended redlines. |
| 19–24 November 2026 | Negotiation window with AgentForge (business and legal). |
| 26 November 2026 | Target PO date, subject to clearance. |

Please return: (a) a risk memo with source cites to the MSA, DPA, SLA, and the CCU checklist; (b) Word-ready redlines or a clause-by-clause mark-up; (c) a contradiction map across the three vendor documents; and (d) a short list of P0 conditions of award versus items that may be accepted or deferred.

---

## 7. Contacts (Fictional)

- Prof. Julian Hartwell, Principal Investigator — j.hartwell@ccu-example.edu
- Simone Alvarez, Associate University Counsel — s.alvarez@ccu-example.edu
- Thomas Reeve, Strategic Sourcing — t.reeve@ccu-example.edu
- AgentForge account lead (vendor): Mara Ellison, Academic Programs — m.ellison@agentforge-example.com

---

*This brief is a synthetic counseling aid prepared for an AutoClaw Round 3 demonstration. It is not legal advice and does not create an attorney-client relationship with any real person or institution.*
