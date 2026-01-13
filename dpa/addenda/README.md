# Data Transfer Mechanisms – Addenda for International Transfers

<img src="../../media/logo.png" alt="Deslicer logo" width="300" />

**Last Updated:** January 7, 2026

---

## Purpose

This directory contains templates for international data transfer mechanisms that supplement the Deslicer Data Processing Agreement (EMEA & APAC) to ensure compliance with data protection laws when Personal Data is transferred to countries outside the European Economic Area (EEA) or the United Kingdom that do not benefit from adequacy decisions.

---

## Available Transfer Mechanisms

### 1. European Commission Standard Contractual Clauses (EU SCCs)

**File:** `eu-scc-module-two.md`

**Purpose:** Provides appropriate safeguards for transfers of Personal Data from the EEA to third countries under Article 46(2)(c) GDPR.

**Module:** Module Two (Controller to Processor)

**When Required:**
- Customer is subject to GDPR (either established in the EEA or within territorial scope under Article 3(2) GDPR)
- Deslicer or its Subprocessors process Personal Data in a country outside the EEA that does not have an EU adequacy decision under Article 45 GDPR

**Commission Decision:** Based on Commission Implementing Decision (EU) 2021/914 of 4 June 2021

---

### 2. UK International Data Transfer Addendum (UK IDTA)

**File:** `uk-idta.md`

**Purpose:** Modifies the EU SCCs to comply with UK data protection law for transfers from the UK to third countries.

**When Required:**
- Customer is subject to UK GDPR (either established in the UK or within territorial scope under Article 3(2) UK GDPR)
- Deslicer or its Subprocessors process Personal Data in a country outside the UK that does not have UK adequacy regulations under Section 17A of the Data Protection Act 2018

**UK ICO Approval:** Based on the UK IDTA template laid before Parliament on 2 February 2022

**Important:** The UK IDTA must be used **together** with the EU SCCs. Execute both documents when UK transfers are in scope.

---

## When Do You Need to Execute These Addenda?

### Step 1: Determine if GDPR/UK GDPR Applies to You

**You are subject to GDPR if:**
- Your organisation is established in the EEA, or
- You offer goods/services to individuals in the EEA, or
- You monitor the behaviour of individuals in the EEA

**You are subject to UK GDPR if:**
- Your organisation is established in the UK, or
- You offer goods/services to individuals in the UK, or
- You monitor the behaviour of individuals in the UK

### Step 2: Determine if Personal Data Will Be Transferred to Third Countries

Review the Deslicer subprocessor list at https://github.com/deslicer/legal/blob/main/privacy/subprocessors.md to see where Personal Data may be processed.

**Third Countries:** Any country outside the EEA/UK that does not have adequacy.

**Common third countries in our subprocessor list:** United States (for certain AI/ML and communications subprocessors)

### Step 3: Check for Adequacy Decisions

#### EU Adequacy Countries (as of January 2026)

The European Commission has issued adequacy decisions for:
- Andorra
- Argentina
- Canada (commercial organisations)
- Faroe Islands
- Guernsey
- Isle of Man
- Israel
- Japan
- Jersey
- New Zealand
- Republic of Korea
- Switzerland
- United Kingdom
- Uruguay
- United States (EU-U.S. Data Privacy Framework)

**Check current status:** https://commission.europa.eu/law/law-topic/data-protection/international-dimension-data-protection/adequacy-decisions_en

#### UK Adequacy Countries (as of January 2026)

The UK has issued adequacy regulations for:
- European Economic Area member states
- Gibraltar
- Countries with EU adequacy decisions (as they stood on 31 December 2020)

**Check current status:** https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/international-transfers-after-uk-exit/

### Step 4: Determine Which Addenda to Execute

| Your Situation | Addendum(s) Required |
|---------------|---------------------|
| Subject to GDPR only + transfers to non-adequate third countries | Execute **EU SCCs** only |
| Subject to UK GDPR only + transfers to non-adequate third countries | Execute **EU SCCs + UK IDTA** |
| Subject to both GDPR and UK GDPR + transfers to non-adequate third countries | Execute **EU SCCs + UK IDTA** |
| All processing in EEA/UK or adequate countries | **No addenda required** (DPA alone suffices) |

---

## How to Execute These Addenda

### For EU Standard Contractual Clauses

1. **Download the template:** `eu-scc-module-two.md`

2. **Review the Annexes:** The annexes reference the Deslicer Data Processing Agreement. Review:
   - Annex I.A (Parties) – Your details will be filled in during execution
   - Annex I.B (Description of Transfer) – Pre-filled based on DPA
   - Annex I.C (Competent Supervisory Authority) – Identify your supervisory authority
   - Annex II (Technical and Organizational Measures) – References DPA Annex 2
   - Annex III (List of Sub-processors) – References Deslicer subprocessor list

3. **Complete the Party Details:**
   - Fill in your legal entity name, address, registration number
   - Fill in your contact person details
   - Identify your competent supervisory authority (Annex I.C)

4. **Execute:**
   - Both parties must sign the document
   - Each party retains a fully executed copy

5. **Retain with DPA:**
   - Keep the executed EU SCCs together with your Deslicer DPA
   - Provide a copy to your data protection officer/compliance team

### For UK International Data Transfer Addendum

1. **Execute EU SCCs First:** The UK IDTA must be used together with EU SCCs. Complete and execute the EU SCCs as described above.

2. **Download the UK IDTA template:** `uk-idta.md`

3. **Complete Table 1 (Parties):**
   - Fill in Start Date (typically the execution date)
   - Fill in your legal entity details
   - Fill in contact details

4. **Complete Table 2 (Selected SCCs):**
   - Confirm Module 2 (Controller to Processor) is selected
   - Reference your executed EU SCCs

5. **Review Table 3 (Appendix Information):**
   - Confirm all annexes reference your executed EU SCCs

6. **Review Table 4 (Ending this Addendum):**
   - Default selection allows either party to end if the Approved Addendum changes materially
   - Modify only if negotiated otherwise

7. **Execute:**
   - Both parties must sign the UK IDTA
   - Each party retains a fully executed copy

8. **Retain Together:**
   - Keep the UK IDTA and EU SCCs together
   - Both form part of your data transfer safeguards

---

## Requesting Execution

### Standard Process

1. **Email Deslicer Legal:** Send a request to legal@deslicer.com with subject line: "Request for Data Transfer Addendum Execution"

2. **Include the following information:**
   - Your legal entity name and address
   - Company registration number (if applicable)
   - Contact person for execution
   - Which addendum(s) you need (EU SCCs, UK IDTA, or both)
   - Your competent supervisory authority (for EU SCCs)
   - Preferred execution method (DocuSign, wet signature, etc.)

3. **Review and Execute:**
   - Deslicer will provide pre-filled templates within 5 business days
   - Both parties review and execute
   - Executed copies exchanged

4. **Timeline:**
   - Standard execution: 5-10 business days from initial request
   - Expedited execution: Available upon request for urgent compliance needs

### Alternative: Pre-Signed Addenda (Enterprise Customers Only)

For enterprise customers with volume licenses, Deslicer can provide pre-signed addenda that become effective upon customer counter-signature. Contact legal@deslicer.com to discuss this option.

---

## Regional Deployment Options

If you prefer to minimize or avoid international transfers entirely, Deslicer offers regional deployment options for certain Offerings:

### EEA-Only Deployment

- Deslicer can configure your deployment to use only EEA-based infrastructure and subprocessors
- Eliminates the need for EU SCCs for GDPR compliance
- Subject to technical feasibility and may involve additional costs
- Contact sales@deslicer.com for availability and pricing

### UK-Only Deployment

- Deslicer can configure your deployment to use only UK-based infrastructure and subprocessors
- Eliminates the need for UK IDTA for UK GDPR compliance
- Subject to technical feasibility and may involve additional costs
- Contact sales@deslicer.com for availability and pricing

---

## Subprocessor Notifications and Transfer Updates

When Deslicer adds or replaces subprocessors, the notification process described in the subprocessor list (https://github.com/deslicer/legal/blob/main/privacy/subprocessors.md) applies.

**Impact on Transfer Addenda:**

- **New subprocessor in adequate country:** No impact on your executed addenda
- **New subprocessor in non-adequate country:** Covered by your executed addenda through the onward transfer provisions (Clause 8.8 of EU SCCs)
- **If you object to a new subprocessor:** Follow the objection process in DPA section 4.4

---

## Frequently Asked Questions

### Q: Do I need to execute these addenda if all Deslicer subprocessors are in adequate countries?

**A:** No. If all subprocessors process Personal Data only in the EEA/UK or countries with adequacy decisions, the DPA alone provides sufficient safeguards. However, the subprocessor list may change over time, so many customers execute the addenda proactively.

### Q: What if my company is established outside the EEA/UK?

**A:** You need these addenda only if you are subject to GDPR or UK GDPR under the territorial scope provisions (Article 3(2)). This typically applies if you offer goods/services to individuals in the EEA/UK or monitor their behavior, even if your company is established elsewhere.

### Q: Can we use our own template SCCs instead of Deslicer's?

**A:** The EU SCCs and UK IDTA are standard forms that cannot be substantially modified. However, if your template is based on the same Commission/ICO approved text, we can review it for compatibility. Contact legal@deslicer.com to discuss.

### Q: How often do we need to renew these addenda?

**A:** The addenda remain in effect for as long as the Deslicer DPA is in effect and you make covered transfers. You do not need to renew them annually. However, if there are material changes to the standard clauses (e.g., the European Commission issues new SCCs), you may need to execute updated versions.

### Q: What happens if adequacy status changes?

**A:**
- **If a country gains adequacy:** Your executed addenda remain valid but may not be necessary for that country. You can continue to rely on them or rely on adequacy for new transfers.
- **If a country loses adequacy:** Your executed addenda continue to provide safeguards. Ensure they cover the affected transfers.

### Q: Are there any countries where Deslicer cannot provide adequate safeguards?

**A:** Deslicer will not knowingly process Personal Data in countries where we cannot provide appropriate safeguards under GDPR/UK GDPR. Our subprocessor list reflects locations where we have assessed that appropriate safeguards can be provided. If regulatory guidance or legal developments make transfers to a specific country impracticable, we will work with affected customers to find alternatives.

---

## Contact Information

**For questions about data transfer mechanisms:**
Email: legal@deslicer.com
Subject: Data Transfer Addenda Question

**For requests to execute addenda:**
Email: legal@deslicer.com
Subject: Request for Data Transfer Addendum Execution

**For regional deployment options:**
Email: sales@deslicer.com
Subject: Regional Deployment Inquiry

---

## Related Documents

- **Deslicer Data Processing Agreement (EMEA & APAC):** https://github.com/deslicer/legal/blob/main/dpa/deslicer-emea-apac-dpa.md
- **Subprocessor List:** https://github.com/deslicer/legal/blob/main/privacy/subprocessors.md
- **Deslicer General Terms:** https://github.com/deslicer/legal/blob/main/general-terms/deslicer-general-terms.md

---

*© 2026 Deslicer AB. All rights reserved.*
