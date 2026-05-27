# DESLICER AI DATA LIFECYCLE AND HANDLING SCHEDULE

<img src="../media/logo.png" alt="Deslicer logo" width="300" />

Last Updated: May 27, 2026

This Deslicer AI Data Lifecycle and Handling Schedule ("**Schedule**") supplements the Specific Terms for Deslicer AI and is incorporated by reference into the Agreement for customers using Deslicer AI. It provides a consolidated description of how Deslicer handles customer data in connection with Deslicer AI, including where data is stored, who can access it, and when it is retained or deleted.

This Schedule is intended to be read together with:

- the [Deslicer General Terms](../general-terms/deslicer-general-terms.md);
- the [Specific Terms for Deslicer Offerings](deslicer-specific-terms.md), including sections 3, 10, 12, and 12A;
- the [Deslicer Data Processing Agreement (DPA)](../dpa/deslicer-emea-apac-dpa.md); and
- the [Deslicer Privacy Policy](../privacy/privacy-policy.md).

In case of conflict, the order of precedence set out in the Agreement applies. For data protection matters, the DPA prevails to the extent required by applicable Data Protection Laws.

---

## 1. Purpose and Scope

This Schedule applies solely to **Deslicer AI** delivered as a SaaS offering (and any supporting on-premises components where specified in the Order).

This Schedule describes:

- the categories of data processed through Deslicer AI;
- where such data is stored and processed;
- who may access it;
- retention and deletion practices during and after the subscription Term; and
- customer controls available for export and deletion.

This Schedule does **not** replace or modify:

- **Customer Content** obligations in General Terms section 4.3;
- **Personal Data** processor obligations in the DPA;
- **Training Data** retention in Specific Terms section 12; or
- license and intellectual property terms in the General Terms, Specific Terms, or applicable EULA.

### 1.1 What customers should expect — at a glance

This section 1.1 is a summary of how Deslicer handles data in connection with Deslicer AI, provided as a reading aid for the parties. In the event of any inconsistency between this summary and the detailed provisions, the detailed provisions prevail. The binding provisions governing the matters summarized in this section are set out in section 5 of this Schedule, Specific Terms sections 12A and 12B, General Terms section 4.3, and the DPA.

| Data type | Where it lives | During subscription | After subscription ends |
|-----------|----------------|---------------------|--------------------------|
| **Customer Content** (artifacts and files you upload to the service) | SaaS Service | Available; you can retrieve and remove at any time | 30-day retrieval window, then deletion (General Terms section 4.3) |
| **AI Service Data** (Inputs, Outputs, agent conversation history) | SaaS Service; AI subprocessors for inference (Deslicer-Provided AI) or your endpoint (BYO AI) | Retained on a commercially reasonable, best-efforts basis; may be removed, truncated, or made unavailable during maintenance, upgrades, or housekeeping; in-product controls where available | Deleted as part of service decommissioning; no separate retrieval window unless agreed in the Order |
| **Service-Operational Data** (Collected Configuration Data and Configuration Change Records — internal service data) | Deslicer-managed systems | Used internally by Deslicer to operate Deslicer AI; configuration snapshots are retained for a reasonable period reflecting how often each monitored item changes; older snapshots may be purged automatically | Deleted no later than the Customer Content deletion date under General Terms section 4.3, without a separate retrieval window; **Configuration Change Records are not exposed for customer export** |
| **Personal Data** | As above, by category | Processed under the DPA on Customer's documented instructions | Returned or deleted per DPA section 9 at Customer's choice |
| **Access and Audit Logs** | Deslicer internal systems | Retained as required for security, compliance, and dispute resolution | Retained for periods required by applicable law; not offered for customer export |

**What customers can do (controls).** Subject to product capabilities, customers can: export Customer Content during the subscription and within the 30-day retrieval window after termination; export agent conversation history through any in-product tools provided or manually preserve it (for example, by copying from the user interface) before maintenance or termination; configure BYO AI to route inference data to a Customer-controlled AI endpoint; and manage in-product access controls. See section 6 of this Schedule.

**What Deslicer does not warrant.** Deslicer does not warrant uninterrupted availability, completeness, or recoverability of AI Service Data or Service-Operational Data. Except for Personal Data Processed on Customer's behalf under the DPA, Deslicer is not liable for loss, corruption, or unavailability of such data, subject to Specific Terms section 14 and General Terms sections 17.5 and 18.

**Consumer tier — important difference.** The retrieval and retention behavior described in this Schedule reflects the **enterprise** Deslicer AI offering governed by the General Terms, Specific Terms, and DPA. For individuals using Deslicer AI on a **consumer plan** under the [Deslicer Consumer Terms](../general-terms/deslicer-consumer-terms.md), there is **no separate post-termination retrieval window** for Customer Content or AI Service Data, and the 30-day retrieval window referenced in the table above (and in General Terms section 4.3) does not apply. Consumers should export anything they wish to keep before closing their account. The full consumer-side rules are set out in Consumer Terms section 10.6.

---

## 2. Data Categories

The following table summarizes the main data categories relevant to Deslicer AI. Personal Data may appear within several categories depending on Customer configuration and use.

| Category | Description | Primary Governing Document |
| -------- | ----------- | -------------------------- |
| **Customer Content** | Stored customer artifacts and data submitted through SaaS Services (configurations, files, and similar materials uploaded by Customer), excluding AI interaction history and Service-Operational Data | General Terms section 4.3 |
| **AI Service Data** | Inputs, Outputs, **agent conversation history**, context data, and related materials generated through use of Deslicer AI (as defined in Specific Terms section 3). Agent conversation history is operational in nature and is not guaranteed to persist for the full subscription Term. | Specific Terms sections 3, 10, and 12A; this Schedule |
| **Service-Operational Data** | Internal Deslicer service data for Deslicer AI, consisting of (i) **Collected Configuration Data** — processed and normalized configuration snapshots derived from monitored items in Customer environments; and (ii) **Configuration Change Records** — historical records of detected or applied configuration changes, drift events, and related processing metadata used by Deslicer AI features. Service-Operational Data is **not Customer Content** and **not AI Service Data**, and is not offered as a customer-exportable archive. | Specific Terms section 12B; this Schedule |
| **Personal Data** | Personal Data embedded in Customer Content, AI Service Data, Service-Operational Data, or other data Processed on Customer's behalf | DPA; Specific Terms sections 12A and 12B where applicable |
| **Training Data** | Aggregated, de-identified service analytics and synthetic or non-customer datasets used for Research and Development Purposes | Specific Terms section 12 |
| **Usage Data** | Data generated from usage, configuration, deployment, access, and performance of Deslicer AI, excluding Customer Content | General Terms section 12 |
| **Account and Administrative Data** | Account, billing, support, security, audit, and compliance records for which Deslicer may act as an independent controller. Includes **Access and Audit Logs** retained in Deslicer internal systems for periods required by applicable law. | DPA scope clarifications; Privacy Policy |

**Important distinctions:**

- **Customer Content**, **AI Service Data**, and **Service-Operational Data** are separate categories. Customer Content covers what Customer uploads to the service. AI Service Data covers Inputs, Outputs, and agent conversation history — which is operational in nature and may be removed during maintenance. Service-Operational Data covers internal processing data the service maintains to operate Deslicer AI and is not exposed for customer export.
- **Training Data** does not include Customer Content or Personal Data.
- Where **Personal Data** is Processed as part of any of the above, the DPA also applies in addition to this Schedule.

---

## 3. Where Data Lives

Deslicer AI is hosted primarily in **EU-based infrastructure**, with subprocessors engaged as described in the [Deslicer Subprocessor List](../privacy/subprocessors.md).

| Data Category | Primary Storage / Processing Location | Primary Subprocessors (indicative) |
| ------------- | ------------------------------------- | ---------------------------------- |
| Customer Content | EU (primary) | Hetzner Online GmbH; Amazon Web Services (EU regions); Supabase, Inc. |
| AI Service Data (live service) | EU (primary) | Hetzner Online GmbH; Amazon Web Services (EU regions); Supabase, Inc. |
| AI Service Data (Deslicer-Provided AI Service) | EU (primary) for Deslicer systems; AI inference may involve US/global regions via AI subprocessors | Google Gemini; OpenAI; Anthropic (as configured) |
| AI Service Data (BYO AI configuration) | EU (primary) for Deslicer-managed components; Inputs/Outputs sent to Customer's AI endpoint are processed under Customer's provider terms | Customer's own AI provider (not a Deslicer subprocessor) |
| Service-Operational Data (Collected Configuration Data and Configuration Change Records) | EU (primary) | Hetzner Online GmbH; Amazon Web Services (EU regions); Supabase, Inc. (Deslicer-managed) |
| Personal Data | As above, depending on category | As listed in the Subprocessor List |
| Training Data | EU (primary) | Deslicer-controlled systems; no Customer Content or Personal Data |
| Usage Data | EU (primary); analytics subprocessors may process in US/EU | PostHog, Inc.; Sentry (Functional Software, Inc.) |
| Account and Administrative Data (including Access and Audit Logs) | EU (primary) | Hetzner; AWS; Microsoft 365; Resend, Inc. |

Region-specific hosting or deployment restrictions must be expressly stated in the applicable Order Form. The current subprocessor list and processing locations are maintained at [https://github.com/deslicer/legal/blob/main/privacy/subprocessors.md](https://github.com/deslicer/legal/blob/main/privacy/subprocessors.md).

---

## 4. Who Can Access Data

Access to customer data is limited by role and purpose:

| Access Tier | Who | Purpose | Data Categories Typically Accessed |
| ----------- | --- | ------- | ---------------------------------- |
| **Customer administrators and authorized users** | Customer personnel with assigned roles | Configure, operate, and use Deslicer AI | Customer Content, AI Service Data, Outputs |
| **Deslicer support personnel** | Deslicer staff with a need to know | Provide support, troubleshoot, and resolve incidents | As necessary for the support request; subject to confidentiality obligations |
| **Deslicer automated systems** | Service components operating Deslicer AI | Provide, secure, monitor, and maintain the service | All categories as required for service operation |
| **AI subprocessors (Deslicer-Provided AI Service only)** | Third-party LLM providers under contract | Generate Outputs based on Inputs | AI Service Data sent for inference only; subject to DPA and subprocessor terms |
| **Deslicer security and compliance functions** | Limited personnel and processes | Security monitoring, incident response, audit, and legal compliance | Logs, metadata, and data as required; may include Account and Administrative Data |

Deslicer's technical and organizational measures are described in General Terms section 7, DPA Annex 2, and any applicable security exhibits.

---

## 5. Lifecycle and Retention

### 5.1 Customer Content

| Phase | Treatment |
| ----- | --------- |
| **During Term** | Available in the SaaS Service; Customer may retrieve and remove at any time |
| **Post-termination retrieval** | Available for retrieval for **30 days** after subscription termination |
| **Deletion** | After the 30-day window, remaining Customer Content deleted **without undue delay**, unless legally prohibited |
| **Backups** | Deletion may be satisfied through standard decommissioning; backup overwrite per DPA section 9.2 |

Customer Content return and deletion is governed by General Terms section 4.3. Customer Content excludes AI Service Data and Service-Operational Data.

### 5.1b Collected Configuration Data

| Phase | Treatment |
| ----- | --------- |
| **During Term** | Retained for a commercially reasonable period reflecting the change frequency of each monitored item. Older snapshots may be purged automatically by Deslicer. |
| **Post-termination** | Deleted no later than the Customer Content deletion date under General Terms section 4.3 (i.e., once the 30-day Customer Content retrieval window ends), subject to applicable legal retention. Where Deslicer offers export tooling for Collected Configuration Data, the timing of such export will be aligned with the Customer Content retrieval window; otherwise no separate retrieval window applies. |
| **No warranty** | Deslicer does not warrant the persistence, completeness, or recoverability of any specific configuration snapshot or set of snapshots. |

### 5.1c Configuration Change Records

| Phase | Treatment |
| ----- | --------- |
| **During Term** | Maintained as internal service technology to support configuration intelligence, drift detection, and related Deslicer AI capabilities. **Not accessible to Customer for export.** Some change information may be surfaced view-only in the user interface; that does not create an export, return, or archive obligation. |
| **Post-termination** | Deleted no later than the Customer Content deletion date under General Terms section 4.3 (i.e., once the 30-day Customer Content retrieval window ends), without any separate retrieval or export window for change records. |
| **Customer expectation** | If Customer requires an independent record of configuration changes for its own audit or compliance purposes, Customer should maintain that record outside Deslicer. |

### 5.2 AI Service Data

| Phase | Treatment |
| ----- | --------- |
| **During Term** | Deslicer uses commercially reasonable efforts to retain AI Service Data, including agent conversation history, subject to: (i) manual or automated maintenance, cleanup, upgrades, migrations, or housekeeping activities, which may delete, truncate, or make AI Service Data unavailable (intentionally or unintentionally); (ii) in-product deletion controls where available in the Documentation; (iii) storage limits and product capabilities documented in the Documentation; and (iv) BYO AI routing data outside Deslicer's retention model. |
| **Post-termination** | AI Service Data is deleted as part of service decommissioning. Deslicer does not guarantee a post-termination retrieval window for AI Service Data unless expressly stated in the applicable Order and supported by available export tooling. |
| **End-user export responsibility** | Preserving agent conversation history, Inputs, and Outputs that the user wishes to keep is the **end user's responsibility**. Where in-product export tools are provided, users should use them. Where export tools are not available for a particular view or data type, users may **manually extract** content — for example, by copying from the user interface — before maintenance, termination, or deletion. Deslicer is not obligated to provide export tooling for every type or view of AI Service Data. |
| **Backups and logs** | Deletion obligations may be satisfied through standard decommissioning processes consistent with DPA section 9.2. AI Service Data may persist in backups and system logs for a limited period consistent with Deslicer's backup retention policies, after which the data is overwritten or deleted in the ordinary course of business. |
| **BYO AI configuration** | Inputs and Outputs sent to Customer's own AI endpoint are subject to Customer's provider relationship and are outside Deslicer's retention model for AI inference data. |
| **Personal Data carve-out** | Where AI Service Data includes Personal Data Processed on Customer's behalf, all retention and deletion remain subject to the DPA. Maintenance, cleanup, and decommissioning activities do not override Deslicer's Personal Data return, deletion, or breach-notification obligations under the DPA and applicable Data Protection Laws. Unintentional loss of Personal Data through such activities is handled under DPA section 9 (return and deletion) and DPA section 8 (Personal Data breach notification) where applicable. |
| **Order Form override** | Retention windows may be varied in a signed Order Form, **provided that** such variation does not weaken Deslicer's Personal Data return and deletion obligations under DPA Article 28(3)(g) and DPA section 9. |

Binding commitments for AI Service Data retention and deletion are set out in Specific Terms section 12A.

### 5.3 Personal Data

Personal Data Processed on Customer's behalf is retained for the duration of the Agreement and applicable Order, and thereafter handled in accordance with DPA section 9 (delete or return at Customer's choice, subject to legal retention and independent controller carve-outs).

Where Personal Data is embedded in AI Service Data, deletion of AI Service Data under section 12A and this Schedule is without prejudice to DPA section 9 obligations for Personal Data.

### 5.4 Training Data

Training Data is retained for up to **one (1) year** following its creation or last use for Research and Development Purposes, unless otherwise required by applicable law. Training Data does not include Customer Content or Personal Data.

Binding commitments for Training Data are set out in Specific Terms section 12.

### 5.5 Usage Data

Usage Data is retained as necessary to operate, maintain, secure, and improve Deslicer AI, and in accordance with General Terms section 12 and the Privacy Policy. Usage Data does not include Customer Content.

### 5.6 Account and Administrative Data (including Access and Audit Logs)

| Phase | Treatment |
| ----- | --------- |
| **Storage** | Deslicer internal systems. Access and Audit Logs are not customer-facing export surfaces unless expressly documented. |
| **Retention** | Retained for periods required by applicable law and Deslicer's legitimate compliance, security, and dispute-resolution needs. Where Deslicer acts as an independent controller for such records (for example, for tax, accounting, dispute resolution, or security purposes), those periods may exceed the subscription Term. |
| **Not customer-exportable** | Access and Audit Logs are not treated as Customer Content, AI Service Data, or Service-Operational Data for the purpose of customer export, return, or retrieval, and are not offered as a customer-facing archive. |
| **Personal Data in logs** | Where logs contain Personal Data, retention and deletion remain subject to the DPA and the backup carve-out in DPA section 9.2. |

---

## 6. Customer Controls

Customer may, subject to product capabilities and Documentation:

- **Export and retrieve Customer Content** during the Term and within the 30-day post-termination retrieval window under General Terms section 4.3;
- **Export agent conversation history and other AI Service Data** using in-product export tools where provided, or **manually preserve** such content (for example, by copying from the user interface) before termination or maintenance cleanup, in each case as an end-user responsibility;
- **Delete** AI Service Data through in-product controls where available;
- **Configure BYO AI** so that AI inference is performed by Customer's own provider rather than Deslicer-managed AI subprocessors;
- **Manage access** through role-based access controls in Customer's environment and Deslicer AI administration settings;
- **Request assistance** with migration or export of Customer Content (and of Collected Configuration Data where export is offered by Deslicer); Deslicer may charge a mutually agreed fee for extended migration support beyond standard export capabilities.

Customer remains responsible for maintaining independent records, backups, and archival copies of Customer Content, AI Service Data, and configuration history where required for Customer's business or regulatory needs. **Configuration Change Records are internal Deslicer service technology and are not available for customer export.**

---

## 7. Process for Return or Deletion at Termination

When a Deslicer AI subscription terminates or expires:

1. **Notice.** Termination takes effect in accordance with the Agreement and applicable Order Form.
2. **Customer Content retrieval window.** Customer may retrieve Customer Content during the 30-day post-termination retrieval window under General Terms section 4.3.
3. **AI Service Data.** Deslicer does not maintain a separate post-termination retrieval window for AI Service Data unless expressly stated in the applicable Order. Customer should export — using in-product tools where provided — or manually preserve any agent conversation history and other AI Service Data it wishes to keep before termination.
4. **Service-Operational Data.** Collected Configuration Data and Configuration Change Records are deleted no later than the Customer Content deletion date under General Terms section 4.3, without a separate retrieval window. Where Deslicer offers export tooling for Collected Configuration Data, its timing is aligned with the Customer Content retrieval window.
5. **Customer action.** Customer should export or manually preserve required data before the Customer Content retrieval window expires. Customer may request migration assistance subject to availability and applicable fees.
6. **Deletion.** After the Customer Content retrieval window, Deslicer deletes remaining Customer Content, AI Service Data, and Service-Operational Data without undue delay, subject to legal retention requirements and the backup decommissioning approach in DPA section 9.2.
7. **Personal Data.** Personal Data is deleted or returned in accordance with DPA section 9 at Customer's choice, subject to the same backup and legal retention carve-outs. Unintentional loss of Personal Data through maintenance activities is handled under DPA section 9 (return and deletion) and DPA section 8 (Personal Data breach notification) where applicable.
8. **Access and Audit Logs.** Access and Audit Logs in Deslicer internal systems are not returned or deleted as part of the customer termination process. They are retained for periods required by applicable law and Deslicer's legitimate compliance, security, and dispute-resolution needs.
9. **Confirmation.** Upon reasonable written request, Deslicer may provide written confirmation that deletion has been initiated or completed, subject to confidentiality and security limitations.

---

## 8. Cross-References

| Topic | Document | Section |
| ----- | -------- | ------- |
| Customer Content return and deletion | [General Terms](../general-terms/deslicer-general-terms.md) | 4.3 |
| AI Service Data use and processing | [Specific Terms](deslicer-specific-terms.md) | 3, 10 |
| AI Service Data retention and deletion (binding) | [Specific Terms](deslicer-specific-terms.md) | 12A |
| Service-Operational Data (binding) | [Specific Terms](deslicer-specific-terms.md) | 12B |
| Training Data retention | [Specific Terms](deslicer-specific-terms.md) | 12 |
| Personal Data return and deletion | [DPA](../dpa/deslicer-emea-apac-dpa.md) | 9 |
| Subprocessors and processing locations | [Subprocessor List](../privacy/subprocessors.md) | — |
| Privacy summary | [Privacy Policy](../privacy/privacy-policy.md) | 9, 11 |

---

*© 2026 Deslicer AB. All rights reserved.*
