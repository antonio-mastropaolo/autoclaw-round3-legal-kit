# AGENTFORGE CLOUD
# SERVICE LEVEL AGREEMENT
## Exhibit B to the AgentForge Cloud Master Subscription Agreement
### Version 3.0 — 1 November 2026

*This document is a wholly fictional service level agreement prepared for a synthetic university-counsel exercise. It is not an agreement of any real company, is not legal advice, and should not be signed or reused as operative contract text.*

---

This Service Level Agreement (this "**SLA**") is Exhibit B to the AgentForge Cloud Master Subscription Agreement (the "**Agreement**") between AgentForge Inc. ("**Provider**") and the customer identified in the Agreement ("**Customer**"). Capitalized terms not defined in this SLA have the meanings given in the Agreement.

This SLA describes the availability target for the production AgentForge Cloud Service, the service credits that may be issued if that target is not met, and the support channels available to Customer. **The Service Credits described in this SLA are Customer's sole and exclusive remedy, and Provider's entire liability, for any failure to meet the Uptime Percentage, for any unavailability, degradation, latency, or support failure, and for any Security Incident or Personal Data Breach (as defined in the DPA) to the extent it manifests as unavailability, degradation, or loss of access to the Service or to Customer Data.** This SLA does not expand any remedy that the Agreement characterizes as exclusive, including Section 8.3 of the Agreement.

If this SLA conflicts with the Agreement, the Agreement controls, except that this SLA controls the calculation of Uptime Percentage and the issuance of Service Credits. If this SLA conflicts with the DPA, the order of precedence in the preamble to the Agreement applies.

---

## 1. DEFINITIONS

**1.1** "**Available**" or "**Availability**" means that the production user interface and primary application programming interface of the Service are reachable by a successful HTTP response (status code 200–399) from Provider's monitoring points, excluding the Exclusions.

**1.2** "**Excused Downtime**" means unavailability arising from any Exclusion in Section 3.

**1.3** "**Monthly Subscription Fee**" means the subscription Fees actually paid by Customer for the Service for the calendar month in which the relevant Downtime occurred, prorated on a thirty (30) day basis if the subscription is billed annually. Usage, overage, professional-services, and pass-through Third-Party Service charges are excluded.

**1.4** "**Security Incident**" means a confirmed unauthorized access to the production Service that materially affects Customer's tenant, as determined by Provider.

**1.5** "**Service Credit**" means a credit calculated under Section 4, issuable against future Fees.

**1.6** "**Uptime Percentage**" means, for a calendar month:

> Uptime Percentage = ((Total Minutes in the month − Downtime Minutes) / Total Minutes in the month) × 100

"**Downtime Minutes**" are minutes during which the Service is not Available, after subtracting Excused Downtime. Partial minutes are rounded down. Measurements are made solely from Provider's monitoring system, which is conclusive as between the Parties, absent manifest error.

---

## 2. AVAILABILITY COMMITMENT

**2.1 Target.** Provider will use commercially reasonable efforts to make the production Service Available with a monthly Uptime Percentage of at least **ninety-nine and one-half percent (99.5%)**.

**2.2 Scope.** This commitment applies only to the production instance of the Service in the standard multi-tenant environment. It does not apply to preview, beta, or experimental features; to sandbox or demonstration tenants; to professional services; to Third-Party Services; or to any feature identified in the Documentation as unsupported or unsupported for service-level purposes.

**2.3 No Other Performance Commitments.** Provider makes no commitment in this SLA regarding latency, throughput, token or job-completion time, model quality, Output accuracy, backup-restoration time, or recovery-point or recovery-time objectives. Any figures on those topics in the Documentation are informational only.

---

## 3. EXCLUSIONS FROM UPTIME

The following are Exclusions and shall not count as Downtime Minutes (and shall not give rise to Service Credits):

**(a) Scheduled Maintenance.** Any period of unavailability for maintenance, upgrades, or infrastructure work. **Provider may perform Scheduled Maintenance at any time. Provider will use commercially reasonable efforts to provide advance notice of Scheduled Maintenance when practicable, but is not required to give notice, is not subject to any minimum notice period or any monthly or annual cap on the duration or frequency of Scheduled Maintenance, and shall not be liable if notice is late, incomplete, or not given.**

**(b) Emergency Maintenance.** Maintenance that Provider reasonably determines is necessary to protect the security, stability, or integrity of the Service or of any customer, with or without notice.

**(c) Customer-Side Factors.** Customer's or an Authorized User's acts or omissions; Customer's equipment, network, or connectivity; Customer's configurations, scripts, or integrations; use of the Service other than in accordance with the Documentation; or failure to use supported browsers, libraries, or API versions.

**(d) Third-Party Services and Dependencies.** Failures of Third-Party Services, model providers, identity providers, public internet, DNS, or other infrastructure not operated by Provider.

**(e) Force Majeure.** Any circumstance described in Section 18.2 of the Agreement, and any other event beyond Provider's reasonable control, **including epidemic, labor dispute, governmental action, change in law, shortage of power, failure of a cloud-infrastructure or telecommunications supplier, denial-of-service attack, or widespread internet disturbance, in each case whether or not reasonably foreseeable and whether or not Provider has implemented redundant systems.**

**(f) Suspension; Beta.** Suspensions under Section 3.2 of the Agreement, or unavailability of features excluded under Section 2.2 of this SLA.

**(g) Insignificant Anomalies.** Periods of degraded performance that do not cause the Service to fail the Availability definition in Section 1.1, including elevated error rates on a subset of endpoints or delayed job processing.

---

## 4. SERVICE CREDITS

**4.1 Credit Table.** If the Uptime Percentage for a calendar month falls below 99.5%, and Customer timely submits a credit request in accordance with Section 4.3, Provider will issue a Service Credit equal to the corresponding percentage of the Monthly Subscription Fee:

| Monthly Uptime Percentage | Service Credit |
| :--- | :--- |
| Less than 99.5% but greater than or equal to 99.0% | 3% of the Monthly Subscription Fee |
| Less than 99.0% but greater than or equal to 98.0% | 5% of the Monthly Subscription Fee |
| Less than 98.0% | 10% of the Monthly Subscription Fee |

**4.2 Maximum Credit.** **The aggregate Service Credits issued for any calendar month shall not exceed ten percent (10%) of the Monthly Subscription Fee for that month.** Unused Service Credits do not roll over, are not transferable, and have no cash value. Service Credits are Customer's sole remedy for the events described in the preamble to this SLA and in Section 8.3 of the Agreement.

**4.3 Claim Procedure.** To receive a Service Credit, Customer's administrative contact must submit a written request to support@agentforge-example.com within fifteen (15) days after the end of the calendar month in which the claimed Downtime occurred, including the dates, times, and a reasonable description of the unavailability. Provider will review its monitoring records and will approve or deny the request in its reasonable discretion. Late or incomplete requests are waived. Service Credits, if approved, will be applied to a future invoice within two (2) billing cycles. No refund will be paid in cash, including at termination, except that an unused approved Service Credit existing at the effective date of Provider's termination for convenience may be refunded at Provider's option.

**4.4 No Other Remedies.** Failure to meet the Uptime Percentage is not a material breach of the Agreement and does not entitle Customer to terminate, to withhold Fees, to claim damages, or to require a root-cause report, except as Provider may elect to provide one. **The Parties agree that Service Credits are a reasonable pre-estimate of Customer's loss and are not a penalty.**

---

## 5. SECURITY INCIDENTS AND DATA ISSUES

**5.1 Notice.** If Provider determines that a Security Incident has occurred, **Provider will use commercially reasonable efforts to notify Customer's designated administrative contact within five (5) business days after Provider's determination.** That notice may be combined with, or may be in lieu of, any notice described in the DPA, as Provider reasonably determines. Provider has no obligation under this SLA to notify Customer of unsuccessful or attempted attacks, of incidents affecting only other customers, or of events that Provider classifies as not meeting the Security Incident definition.

**5.2 Exclusive Remedy.** **If a Security Incident, Personal Data Breach, data loss, or data corruption results in unavailability or in a failure of Customer to access Customer Data, Customer's sole remedy is the Service Credit, if any, available under Section 4.** Nothing in this Section 5 requires Provider to pay forensic, notification, credit-monitoring, restoration, or regulatory costs, and nothing in this SLA enlarges the liability terms of Section 11 of the Agreement.

---

## 6. SUPPORT

**6.1 Channel and Hours.** Standard support is provided **by email only, to support@agentforge-example.com, during the hours of 9:00 a.m. to 5:00 p.m., Pacific Time, Monday through Friday, excluding Provider holidays** (as posted on Provider's website or stated in a support notice). Messages received outside those hours are deemed received at the start of the next support day. Provider does not commit to telephone, chat, or on-call coverage under this SLA. Premium or twenty-four-hour support, if any, is available only if purchased on an Order Form.

**6.2 Severity and Response Targets.** Provider will use commercially reasonable efforts to acknowledge email support requests in accordance with the following targets. **These targets are objectives only, are not service levels, and give rise to no Service Credits, no refund, and no termination right if missed.**

| Severity | Indicative meaning | Target first-response |
| :--- | :--- | :--- |
| Severity 1 | The production Service is down or unusable for all of Customer's Authorized Users, with no reasonable workaround. | One (1) support day |
| Severity 2 | A major feature is impaired for a substantial portion of Authorized Users, and a workaround is limited or unavailable. | Two (2) support days |
| Severity 3 | A non-critical issue or a question about use of the Service; a workaround is available, or only a small number of users are affected. | Five (5) support days |

**6.3 Classification.** **Provider has sole discretion to classify the Severity of a request.** A request is not Severity 1 solely because it coincides with a research deadline, a publication date, a grant milestone, or an examination period. Customer shall reasonably cooperate in diagnosing issues, including by providing logs, timestamps, and a reproducible description.

**6.4 Scope of Support.** Support covers the production Service as described in the Documentation. It does not include custom development, data migration, model-prompt engineering, academic-methods advice, export-control classification, or assistance with Third-Party Services, except as Provider may agree in a paid statement of work.

---

## 7. GENERAL

**7.1 Updates.** Provider may update this SLA in accordance with Section 1.12 and Section 18.5 of the Agreement.

**7.2 Interpretation.** Headings are for convenience only. This SLA is not a warranty that the Service will be error-free or that Customer Data will be preserved, and it is subject always to the disclaimers and limitations in the Agreement.

---

*AgentForge Cloud Service Level Agreement, Version 3.0 (1 November 2026). Fictional form for AutoClaw Round 3 demonstration use only. Not legal advice. Not for signature.*
