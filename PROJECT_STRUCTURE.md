# SENTINEL Workforce Systems™ - Project Structure

## Overview
Static demonstration interface designed for CFOs, General Counsel, Risk Officers, and regulators.
**This is not a functional product.** It is an explanatory system with no backend, no data processing, and no user accounts.

---

## Folder Structure

```
sentinel-demo/
├── public/
│   └── (static assets)
├── src/
│   ├── app/
│   │   ├── layout.tsx                    # Root layout with navigation
│   │   ├── page.tsx                      # Landing page
│   │   ├── governance-overview/
│   │   │   └── page.tsx                  # Section 1: Governance Overview
│   │   ├── risk-surfaces/
│   │   │   └── page.tsx                  # Section 2: Risk Surfaces
│   │   ├── sell-sequence/
│   │   │   └── page.tsx                  # Section 3: Sell Sequence
│   │   ├── governance-artifacts/
│   │   │   └── page.tsx                  # Section 4: Governance Artifacts
│   │   ├── research-alignment/
│   │   │   └── page.tsx                  # Section 5: Research & Institutional Alignment
│   │   └── what-this-is-not/
│   │       └── page.tsx                  # Section 6: What This Is Not
│   ├── components/
│   │   ├── Navigation.tsx                # Main navigation component
│   │   ├── PageHeader.tsx                # Reusable page header
│   │   └── Disclaimer.tsx                # "Illustrative / Representative" notice
│   └── styles/
│       └── globals.css                   # Conservative, institutional styling
├── next.config.js                         # Next.js configuration (static export)
├── package.json
└── tsconfig.json
```

---

## Section Purposes

### 1. Governance Overview
**Purpose:** Establish the institutional context and governance framework.

Explains what workforce risk governance means in the context of:
- Fiduciary duty
- Regulatory compliance
- Board-level oversight
- Enterprise risk management

**Tone:** Formal, framework-oriented, non-promotional.

---

### 2. Risk Surfaces
**Purpose:** Identify categories of workforce-related institutional risk.

Representative categories (illustrative only):
- Regulatory compliance risk
- Litigation and liability exposure
- Operational continuity risk
- Reputational harm
- Financial misstatement risk

**Does NOT include:**
- Real metrics
- Scoring systems
- Predictive analytics

---

### 3. Sell Sequence (Expertise → Risk Audit → Governance Core)
**Purpose:** Demonstrate the logical progression of governance implementation.

Three-stage conceptual flow:
1. **Expertise:** Domain knowledge and regulatory awareness
2. **Risk Audit:** Identification and documentation of exposure
3. **Governance Core:** Ongoing oversight and accountability structures

**Does NOT suggest:**
- Automated solutions
- Turnkey implementation
- Guaranteed outcomes

---

### 4. Governance Artifacts
**Purpose:** Show representative documentation types used in governance practice.

Examples (redacted, illustrative):
- Board reporting templates
- Risk assessment frameworks
- Policy documentation structures
- Audit trail formats

**All examples labeled:** "Illustrative / Representative"

**Does NOT include:**
- Real company data
- Actual assessments
- Live documents

---

### 5. Research & Institutional Alignment
**Purpose:** Ground the system in established governance literature and standards.

References to:
- Corporate governance frameworks (COSO, ISO)
- Regulatory guidance
- Academic research on workforce risk
- Industry standards

**Does NOT claim:**
- Proprietary methodologies
- Novel frameworks
- Certification or endorsement

---

### 6. What This Is Not
**Purpose:** Explicitly state limitations and prevent misinterpretation.

Clear disclaimers:
- Not a software product
- Not a data analytics platform
- Not a compliance tool
- Not a substitute for legal/audit counsel
- Not claiming to predict, prevent, or solve risks

**Tone:** Direct, protective, unambiguous.

---

## Design Principles

### Visual Tone
- Grayscale or muted blue palette
- Generous whitespace
- Clear typography (system fonts)
- No animations or transitions
- No images of people or workplaces
- No charts or visualizations

### Content Tone
- Institutional
- Conservative
- Descriptive, not prescriptive
- Audit-safe language
- No superlatives
- No claims of efficacy

### Technical Approach
- Static site generation (Next.js with `output: 'export'`)
- No JavaScript interactivity beyond navigation
- No forms or inputs
- No external API calls
- No tracking or analytics
- Self-contained HTML/CSS/JS bundle

---

## Deployment
- Static files only
- Can be served from any web server
- No server-side rendering
- No environment variables
- No build-time data fetching
