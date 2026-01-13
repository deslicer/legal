# EU AI Act Compliance Review Template

<img src="../media/logo.png" alt="Deslicer logo" style="max-width:25%; height:auto;" />

**Document Type:** Internal Compliance Review Template
**Last Updated:** January 7, 2026
**Review Frequency:** Quarterly or upon major product changes

---

## Purpose

This template provides a structured framework for periodic review of Deslicer AI's classification and compliance under the EU AI Act (Regulation (EU) 2024/1689). Regular reviews ensure that:

- Our AI system classification remains accurate as the product and regulatory landscape evolve
- Transparency obligations are consistently met
- Customer-facing terms remain aligned with regulatory requirements
- Technical guardrails are appropriate for intended use cases

---

## Review Schedule

**Mandatory Reviews:**

- Quarterly (Q1, Q2, Q3, Q4)
- Before any major product release that changes AI functionality
- When significant regulatory guidance is published (EU Commission, national authorities)
- After customer deployment patterns reveal new use cases

**Review Team:**

- Legal/Compliance Lead
- Product Manager (Deslicer AI)
- Engineering Lead (AI/ML)
- Customer Success (for deployment scenario insights)

---

## Section 1: AI System Classification

### 1.1 Current Classification

**Documented Classification:** Limited-risk AI system under EU AI Act Article 50

**Basis for Classification:**

- [ ] System is designed for configuration management and operational insights
- [ ] Primary use case is technical analysis and optimization, not decision-making affecting individuals
- [ ] Does not fall within high-risk categories defined in Annex III
- [ ] Requires transparency disclosures but not full conformity assessment

**Date of Last Classification Review:** _______________

**Reviewed by:** _______________

### 1.2 Classification Criteria Checklist

**Question 1: Does Deslicer AI meet the definition of "AI system" under Article 3(1)?**

- [ ] Yes - Uses machine learning and generates outputs (recommendations, analyses)
- [ ] No - System is purely rule-based (would exclude from AI Act)

**If Yes, proceed to Question 2.**

**Question 2: Is Deslicer AI a general-purpose AI model (GPAI) under Article 3?**

- [ ] No - Deslicer AI uses third-party GPAIs but is itself a specialized application
- [ ] Yes - Would trigger different obligations

**Current Assessment:** Deslicer AI is an AI system but not a GPAI.

**Question 3: Does Deslicer AI fall within prohibited AI practices (Article 5)?**

Review each prohibited practice:

- [ ] Social scoring by public authorities: **No** - Not designed for this purpose
- [ ] Manipulation or deception: **No** - Transparent AI disclosure provided
- [ ] Exploitation of vulnerabilities: **No** - Technical configuration tool
- [ ] Biometric categorization (sensitive characteristics): **No** - No biometric processing
- [ ] Real-time remote biometric identification in public spaces: **No** - No biometric processing
- [ ] Emotion recognition in workplace/education: **No** - No emotion detection
- [ ] Untargeted scraping of facial images: **No** - No facial recognition

**Assessment:** Deslicer AI does not engage in prohibited practices.

**Question 4: Is Deslicer AI a high-risk AI system under Annex III?**

Review each Annex III category:

**Category 1: Biometrics**

- [ ] Biometric identification/categorization: **No**

**Category 2: Critical Infrastructure**

- [ ] Management/operation of critical infrastructure (water, gas, electricity, etc.): **Potential Risk**
  - Deslicer AI may be used to manage observability infrastructure for critical infrastructure operators
  - However, Deslicer AI itself is not managing the critical infrastructure directly
  - Assessment: **Not high-risk** when used for its intended purpose (log/observability management)
  - **Action:** Monitor customer deployments; flag if customers use for direct critical infrastructure control

**Category 3: Education/Vocational Training**

- [ ] Determining access to educational institutions: **No**
- [ ] Assessing learning outcomes: **No**

**Category 4: Employment**

- [ ] Recruitment, selection, promotion decisions: **No**
- [ ] Task allocation, monitoring, evaluation of workers: **Potential Risk**
  - If customers use Deslicer AI to monitor employee system usage or performance
  - Assessment: **Not designed for this purpose**; prohibited without separate agreement
  - **Action:** Terms explicitly exclude high-risk use; confirm technical restrictions

**Category 5: Essential Services and Benefits**

- [ ] Credit scoring, insurance pricing: **No**
- [ ] Emergency response dispatch: **No**
- [ ] Access to essential services: **No**

**Category 6: Law Enforcement**

- [ ] Risk assessment for criminal offenses: **No**
- [ ] Polygraph/emotion detection: **No**
- [ ] Deep fake detection: **No**

**Category 7: Migration and Border Control**

- [ ] Assessing security risks: **No**

**Category 8: Justice and Democracy**

- [ ] Assisting judicial authorities: **No**
- [ ] Influencing democratic processes: **No**

**Overall Annex III Assessment:** Deslicer AI is **not designed or intended** for any Annex III high-risk use case. Terms explicitly prohibit such use without separate agreement.

**Question 5: If not high-risk, what transparency obligations apply?**

- [x] Article 50: Limited-risk systems (AI systems that interact with natural persons)
- [x] Article 52: Transparency when using AI systems
  - Users must be informed they are interacting with AI
  - Generated content must be disclosed as AI-generated when shared with third parties

**Current Compliance Status:**

- [ ] Specific Terms section 2A provides Article 52 transparency notice
- [ ] Terms require human validation before production use
- [ ] Terms require disclosure when AI-generated content affects third parties

---

## Section 2: Intended Use Case Documentation

### 2.1 Primary Intended Use Cases

Document the intended use cases as described in customer-facing terms and marketing:

**Use Case 1: Configuration Discovery and Normalization**

- Description: Automated discovery and normalization of log management/observability configurations
- Risk Level: Minimal
- Human Oversight: Configuration review before application
- Personal Data Processing: May include technical identifiers, user IDs in logs

**Use Case 2: Configuration Intelligence and Deviation Analysis**

- Description: Analysis of configuration patterns, baseline comparison, optimization recommendations
- Risk Level: Limited
- Human Oversight: Recommendations reviewed by technical staff before implementation
- Personal Data Processing: Configuration metadata, change history with user identifiers

**Use Case 3: Policy Validation and Compliance**

- Description: Assessment of configurations against policies and best practices
- Risk Level: Limited
- Human Oversight: Policy violations reviewed and remediated by technical staff
- Personal Data Processing: Audit logs, compliance reports with user identifiers

**Use Case 4: Operational Insights and Optimization**

- Description: Generation of insights and recommendations for cost/performance optimization
- Risk Level: Limited
- Human Oversight: Insights used by technical and management staff; not automated
- Personal Data Processing: Usage data, performance metrics, may include user activity patterns

**Use Case 5: Change Automation Support**

- Description: Semi-automated or fully automated generation of change proposals
- Risk Level: Limited-Medium
- Human Oversight: Approval workflows required before production deployment
- Personal Data Processing: Change requests, approval records with user identifiers

### 2.2 Use Cases Explicitly Excluded

Document use cases that are **not** intended and are prohibited or restricted:

- [ ] High-risk employment decisions (hiring, firing, promotion) without separate agreement
- [ ] Direct control of critical infrastructure without separate agreement
- [ ] Credit scoring, insurance underwriting, or financial risk assessment without separate agreement
- [ ] Law enforcement applications without separate agreement
- [ ] Medical diagnosis or treatment recommendations (prohibited entirely)
- [ ] Biometric identification or categorization (prohibited entirely)

**Documented in:** Specific Terms section 2A, AI Acceptable Use Policy Annex A

---

## Section 3: Customer Deployment Scenario Analysis

### 3.1 Actual Customer Deployments (Review Quarterly)

**Review Date:** _______________

**Question: Have customers deployed Deslicer AI for any use cases not explicitly documented as intended use?**

- [ ] Yes - Document below
- [ ] No
- [ ] Unknown - Requires customer outreach

**If Yes, document:**

| Customer/Segment | Use Case | Risk Assessment | Action Required |
|------------------|----------|-----------------|-----------------|
| [Redacted] | [Description] | [Low/Limited/High] | [None/Monitor/Restrict/Separate Agreement] |

### 3.2 Customer Inquiries About High-Risk Use

**Question: Have customers inquired about using Deslicer AI for high-risk applications?**

- [ ] Yes - Document below
- [ ] No

**If Yes, document:**

| Date | Customer | Requested Use Case | Response | Follow-up Required |
|------|----------|-------------------|----------|-------------------|
| | | | | |

---

## Section 4: Transparency Obligations Compliance Check

### 4.1 Article 52 Transparency Requirements

**Requirement 1: Users informed they are interacting with AI**

- [ ] Compliant - Specific Terms section 2A provides clear notice
- [ ] Review needed

**Requirement 2: AI-generated outputs identified as such**

- [ ] Compliant - Terms require disclosure when shared with third parties
- [ ] Review needed

**Requirement 3: Human oversight requirements communicated**

- [ ] Compliant - Terms require human validation before production use
- [ ] Review needed

**Requirement 4: Limitations and risks disclosed**

- [ ] Compliant - Terms disclose hallucination risk, inaccuracy, bias potential
- [ ] Review needed

### 4.2 Documentation and Record-Keeping

**Question: Do we maintain adequate documentation to demonstrate compliance?**

- [ ] Yes - Document location: _______________
- [ ] Needs improvement

**Required Documentation:**

- [ ] Technical documentation describing AI system architecture
- [ ] Training data sources and characteristics
- [ ] Testing and validation results
- [ ] Risk assessments and mitigation measures
- [ ] Customer-facing transparency disclosures

---

## Section 5: Technical Guardrails Assessment

### 5.1 Current Technical Safeguards

Review technical measures in place to prevent high-risk misuse:

**Safeguard 1: Approval Workflows**

- [ ] In place - Customers can configure approval gates for production changes
- [ ] Status: _______________

**Safeguard 2: Human-in-the-Loop Controls**

- [ ] In place - System does not automatically apply changes without explicit approval
- [ ] Status: _______________

**Safeguard 3: Usage Monitoring**

- [ ] In place - System logs all AI interactions for audit
- [ ] Status: _______________

**Safeguard 4: High-Risk Detection**

- [ ] Not yet implemented - Consider automated detection of high-risk deployment patterns
- [ ] Status: _______________

### 5.2 Recommended Enhancements

Based on this review, are additional technical guardrails recommended?

**Enhancement 1: High-Risk Use Case Warnings**

- Description: Display warnings when usage patterns suggest high-risk deployment
- Priority: [ ] High [ ] Medium [ ] Low
- Feasibility: [ ] High [ ] Medium [ ] Low
- Recommendation: _______________

**Enhancement 2: Contractual Compliance Checks**

- Description: Technical checks to ensure separate agreements are in place before enabling high-risk features
- Priority: [ ] High [ ] Medium [ ] Low
- Feasibility: [ ] High [ ] Medium [ ] Low
- Recommendation: _______________

**Enhancement 3: Enhanced Audit Logging**

- Description: More detailed logging of AI decision points for regulatory compliance
- Priority: [ ] High [ ] Medium [ ] Low
- Feasibility: [ ] High [ ] Medium [ ] Low
- Recommendation: _______________

---

## Section 6: Regulatory Guidance Evolution Tracking

### 6.1 EU Commission Guidance

**Latest Guidance Reviewed:**

- Date: _______________
- Source: _______________
- Impact on Deslicer AI: [ ] None [ ] Minor [ ] Significant
- Action Required: _______________

**Relevant Commission Documents:**

- [ ] General Purpose AI Code of Practice (Article 56)
- [ ] Guidelines on classification of high-risk AI systems
- [ ] FAQ documents from EU Commission
- [ ] Implementing acts and delegated regulations

### 6.2 National Authority Guidance

**Member State Guidance Reviewed:**

**Sweden (Integritetsskyddsmyndigheten - IMY):**

- Date Reviewed: _______________
- Relevant Guidance: _______________
- Impact: _______________

**Other Relevant Jurisdictions:**

- [ ] Germany (BfDI, Bundesnetzagentur)
- [ ] France (CNIL)
- [ ] Netherlands (AP)
- [ ] Ireland (DPC) - if customers with EU HQ in Ireland

**Impact Assessment:** _______________

### 6.3 Industry Standards and Best Practices

**Standards Reviewed:**

- [ ] ISO/IEC 42001 (AI Management System)
- [ ] ISO/IEC 23894 (Risk Management for AI)
- [ ] NIST AI Risk Management Framework (for US customers)
- [ ] Industry-specific guidance (if applicable)

**Adoption Recommendations:** _______________

---

## Section 7: Customer-Facing Terms Alignment

### 7.1 Review of Specific Terms Section 2A

**Question: Does section 2A accurately reflect current system capabilities and classification?**

- [ ] Yes - No changes needed
- [ ] No - Updates required

**If updates required, document:**

| Current Language | Proposed Update | Reason |
|-----------------|-----------------|--------|
| | | |

### 7.2 Review of AI Acceptable Use Policy (Annex A)

**Question: Does Annex A adequately restrict prohibited and high-risk uses?**

- [ ] Yes - No changes needed
- [ ] No - Updates required

**If updates required, document:**

| Current Language | Proposed Update | Reason |
|-----------------|-----------------|--------|
| | | |

### 7.3 Review of DPA AI Service Data Provisions

**Question: Does the DPA adequately address AI-related data processing and GDPR compliance?**

- [ ] Yes - No changes needed
- [ ] No - Updates required

**If updates required, document:**

| Section | Current Language | Proposed Update | Reason |
|---------|-----------------|-----------------|--------|
| | | | |

---

## Section 8: Risk Mitigation and Action Items

### 8.1 Identified Risks

Based on this review, document any compliance risks:

**Risk 1:**

- Description: _______________
- Severity: [ ] High [ ] Medium [ ] Low
- Likelihood: [ ] High [ ] Medium [ ] Low
- Mitigation Plan: _______________
- Owner: _______________
- Due Date: _______________

**Risk 2:**

- Description: _______________
- Severity: [ ] High [ ] Medium [ ] Low
- Likelihood: [ ] High [ ] Medium [ ] Low
- Mitigation Plan: _______________
- Owner: _______________
- Due Date: _______________

### 8.2 Action Items

| # | Action Item | Owner | Due Date | Priority | Status |
|---|-------------|-------|----------|----------|--------|
| 1 | | | | [ ] High [ ] Medium [ ] Low | [ ] Open [ ] In Progress [ ] Complete |
| 2 | | | | [ ] High [ ] Medium [ ] Low | [ ] Open [ ] In Progress [ ] Complete |
| 3 | | | | [ ] High [ ] Medium [ ] Low | [ ] Open [ ] In Progress [ ] Complete |

---

## Section 9: Review Conclusion and Sign-Off

### 9.1 Overall Assessment

**Classification Remains Appropriate:**

- [ ] Yes - Limited-risk AI system classification confirmed
- [ ] No - Reclassification required (document reason below)

**Transparency Obligations Met:**

- [ ] Yes - All Article 50/52 requirements satisfied
- [ ] No - Gaps identified (document below)

**Technical Safeguards Adequate:**

- [ ] Yes - Current safeguards appropriate for intended use
- [ ] No - Enhancements required (documented in Section 5.2)

**Customer-Facing Terms Accurate:**

- [ ] Yes - Terms reflect current system and regulatory requirements
- [ ] No - Updates required (documented in Section 7)

**Overall Compliance Status:**

- [ ] Compliant - No significant issues identified
- [ ] Compliant with minor improvements recommended
- [ ] Non-compliant - Immediate action required

### 9.2 Recommendations for Next Review

**Priority Areas for Next Review:**

1. _______________
2. _______________
3. _______________

**Regulatory Developments to Monitor:**

1. _______________
2. _______________
3. _______________

### 9.3 Sign-Off

**Review Completed by:**

Legal/Compliance Lead: _______________ Date: _______________

Product Manager: _______________ Date: _______________

Engineering Lead: _______________ Date: _______________

**Next Scheduled Review:** _______________

---

## Appendix A: Regulatory Reference Links

**EU AI Act Core Documents:**

- Regulation (EU) 2024/1689: https://eur-lex.europa.eu/eli/reg/2024/1689
- European Commission AI Act Hub: https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai

**Classification Guidance:**

- High-Risk AI Systems: Annex III of Regulation (EU) 2024/1689
- Prohibited AI Practices: Article 5 of Regulation (EU) 2024/1689
- Transparency Obligations: Articles 50-52 of Regulation (EU) 2024/1689

**National Authorities:**

- Sweden IMY: https://www.imy.se/
- European Data Protection Board: https://edpb.europa.eu/

---

## Appendix B: Version History

| Version | Date | Changes | Reviewer |
|---------|------|---------|----------|
| 1.0 | 2025-11-16 | Initial template created | Legal team |
| | | | |

---

*© 2026 Deslicer AB. Internal compliance document.*
