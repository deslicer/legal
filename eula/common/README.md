# EULA Common Modules

<img src="../../media/logo.png" alt="Deslicer logo" width="300" />

**Last Updated:** January 7, 2026

---

## Overview

This directory contains common modules used across all Deslicer End User License Agreements (EULAs). The common module approach:

- **Reduces duplication:** Standard warranty and liability language is defined once
- **Ensures consistency:** All EULAs reference the same standard provisions
- **Simplifies updates:** Changes to standard language are made in one place
- **Improves maintainability:** Product-specific EULAs focus on unique provisions

---

## Available Modules

### standard-disclaimers.md

Contains 9 standardized modules:

1. **Module 1:** AS-IS Warranty Disclaimer (Commercial)
2. **Module 2:** AS-IS Warranty Disclaimer (OSS)
3. **Module 3:** Implied Warranty Disclaimer (Extended)
4. **Module 4:** Limitation of Liability (Commercial - 12 Month Cap)
5. **Module 5:** Limitation of Liability (OSS - EUR 100 Cap)
6. **Module 6:** Force Majeure
7. **Module 7:** Governing Law (Swedish Law)
8. **Module 8:** No Warranty for Accuracy, Fitness, or Uninterrupted Service
9. **Module 9:** No Liability for Deployment Outcomes

---

## How Common Modules Are Used in EULAs

### Module Selection

**Commercial Offerings (Deslicer AI, DevOps, Automation Platform):**
- Module 1 (AS-IS Disclaimer - Commercial)
- Module 4 (Liability Cap - Commercial)
- Module 6 (Force Majeure) - via General Terms reference
- Module 7 (Governing Law) - via General Terms reference
- Module 8 (AI/Technical) - if AI-powered
- Module 9 (Deployment) - if DevOps/Automation

**OSS Projects (AI Sidekick, MCP for Splunk, CCA for Splunk):**
- Module 2 (AS-IS Disclaimer - OSS)
- Module 5 (Liability Cap - OSS)
- Module 6 (Force Majeure) - if needed
- Module 7 (Governing Law)
- Module 8 (AI/Technical) - if AI-powered

### Reference Pattern in EULAs

**Pattern for Commercial EULAs:**

```markdown
## X. Warranties, Disclaimers and Limitation of Liability

### X.1 Warranties

Deslicer's warranties are set out in section 17 of the General Terms and in the Specific Terms for [Offering Name]. In particular, Deslicer warrants that it will not materially decrease the overall functionality of the SaaS Service during the Term, as stated in section 17.3 of the General Terms.

### X.2 [Product-Specific] Disclaimers

As further described in the Specific Terms for [Offering Name]:

- [Product-specific disclaimer 1]
- [Product-specific disclaimer 2]
- [Product-specific disclaimer 3]

For standard warranty disclaimers and limitations applicable to all Deslicer Offerings, see the [Standard EULA Disclaimers](https://github.com/deslicer/legal/blob/main/eula/common/standard-disclaimers.md) (Modules 1, 4, and [others as applicable]).

### X.3 Limitation of Liability

Section 18 (Limitation of Liability) of the General Terms applies in full to your use of [Offering Name]. Nothing in this EULA expands Deslicer's liability beyond what is agreed in the General Terms.
```

**Pattern for OSS EULAs:**

```markdown
## 2. No Warranty

To the maximum extent permitted by applicable law and in addition to any disclaimers in the Open Source License:

- The Software is provided **"AS IS"** and **"AS AVAILABLE"**; and
- Deslicer and its Affiliates disclaim all warranties, whether express, implied, statutory or otherwise, including any implied warranties of merchantability, satisfactory quality, fitness for a particular purpose, non‑infringement, or quiet enjoyment.

Without limiting the foregoing, Deslicer does not warrant that the Software will be error‑free, uninterrupted, secure, or compatible with all [platform] environments.

For detailed standard disclaimers, see [Module 2](https://github.com/deslicer/legal/blob/main/eula/common/standard-disclaimers.md#module-2-as-is-warranty-disclaimer-oss-variant) of the Standard EULA Disclaimers.

## 3. Limitation of Liability

To the maximum extent permitted by applicable law:

- Deslicer's and its Affiliates' **aggregate liability** arising out of or related to the Software will not exceed **EUR 100**; and
- Deslicer and its Affiliates will **not** be liable for any indirect, incidental, consequential, special, punitive or exemplary damages.

If you are also a customer under the Deslicer General Terms, section 18 (Limitation of Liability) of the General Terms will apply instead of the EUR 100 cap.

For detailed limitations, see [Module 5](https://github.com/deslicer/legal/blob/main/eula/common/standard-disclaimers.md#module-5-limitation-of-liability-oss---eur-100-cap) of the Standard EULA Disclaimers.
```

### Product-Specific vs. Standard Content

**Product EULAs focus on:**
- Product-specific operational risks (e.g., "AI may hallucinate")
- Technology-specific disclaimers (e.g., "Not designed for medical use")
- Integration-specific risks (e.g., "Relies on third-party APIs")
- Deployment-specific warnings (e.g., "Test before production")

**Common modules provide:**
- Generic implied warranty disclaimers (Module 3)
- Standard liability caps (Modules 4 and 5)
- Force majeure provisions (Module 6)
- Governing law (Module 7)

---

## Example Usage

### Commercial EULA Pattern

```markdown
## X. Warranties, Disclaimers and Limitation of Liability

### X.1 Warranties

Deslicer's warranties are set out in section 17 of the General Terms. In particular, the SaaS Service will perform materially in accordance with the Documentation.

### X.2 Product-Specific Disclaimers

In addition to standard disclaimers (see Module 1 of the Standard EULA Disclaimers):

- [Offering Name] may generate recommendations that require validation before implementation
- Automated changes may cause service interruption if not properly configured
- Customer is responsible for testing in non-production environments

### X.3 Limitation of Liability

Section 18 (Limitation of Liability) of the General Terms applies in full to [Offering Name]. See also Module 4 of the Standard EULA Disclaimers for detailed provisions.
```

---

## Contact

For questions about EULA modules or licensing:

**Email:** legal@deslicer.com
**Subject:** "EULA Question"

---

*© 2026 Deslicer AB. All rights reserved.*
