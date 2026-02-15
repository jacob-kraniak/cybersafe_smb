## CyberSafe Home Grok Workspace Summary (Key Discussions & Decisions)

**Last Updated:** February 2025–2026 (ongoing)  
**Purpose:** Quick reference for business evolution decisions discussed with Grok (business partner / project manager mode).

### 1. Current Business Model Recap
- **Target:** Small businesses (mechanics, hairdressers, etc.) + individuals
- **Core Offering:** Tiered cybersecurity self-assessments via online forms
  - **Basic** ($40): 15-point foundational checklist → personalized report
  - **Premium** ($100): 30 points + 1-hour consult
  - **Pro** ($250): 50 points + 2-hour consult + 3 months monitoring
  - **Ongoing:** $12/month monitoring add-on
- **Lead Flow:** Free 15-question audit (Google Forms) → auto-scored → upsell emails → paid form → report + consult + Zoho Books invoice
- **Tech Stack (MVP):** Carrd site, Google Forms/Sheets/Apps Script, Zoho Books, manual PDF reports from Google Docs templates

### 2. Scaling Beyond Google Forms
**Goal:** Replace consumer-grade Google Forms with a professional, integrated platform  
**Comparison & Decision:**
- **Zoho Forms** vs **Jotform** evaluated (pricing, scalability, integrations)
- **Winner: Zoho Forms**
  - Native integration with Zoho Books (auto-invoicing, customer creation)
  - Unlimited forms on paid plans, high submission volume at lower cost
  - Multi-page/conditional logic perfect for tiered audits (15 → 30 → 50 points)
  - Workflows, PDF generation, approvals, audit logs
  - Starting cost: ~$12/month (Basic plan)
- **Migration Plan:**
  - Import existing questions/logic
  - Build separate forms per tier
  - Automate: submission → scoring → report trigger → invoice in Books
  - Reduce manual work per customer (target: 50% time savings)
- **Next Action:** Prototype free audit form in Zoho Forms; update repo with migration guide

### 3. SMB Certifications & Framework Alignment
**Focus:** Move from "inspired by" language to credible alignment/audit services  
**Key Frameworks Discussed:**

- **NIST CSF** — Most achievable for CyberSafe
  - Voluntary, flexible, no formal certification body required
  - Can offer "NIST CSF Alignment Audits" as $500–$1,000 upsell to Pro package
  - Use existing 50-point mappings (Identify → Protect → Detect → Respond)
  - Start with gap analysis during consults + virtual evidence review
  - No licensing barrier initially; build on personal credentials

- **ISO 27001** — High barrier (requires accredited certification body status)
  - Not realistic short-term; consider future partnership/white-label

- **SOC 2** — Medium-high barrier (requires licensed CPA firm to issue reports)
  - Potential via CPA partnership; longer-term play

**Personal Certification Alignment:**
- Ties directly to Security+ (foundational), CySA+ (analysis/vuln mgmt), eventual CISSP
- Offering NIST-aligned services builds portfolio hours/experience

**Phased Roadmap:**
1. Launch NIST CSF Alignment add-on pilot (3 months)
2. Earn Security+ to strengthen credibility
3. Pilot with 2–5 existing leads
4. Document results → testimonials → marketing

### 4. Open / In-Progress Items
- Finalize Zoho Forms migration & automation flows
- Update legal disclaimers for NIST/ISO/SOC 2 mappings
- Add "NIST Alignment Audit" section to package tiers doc
- Research low-cost CISA/CISSP consultants for co-review if needed
- Track everything in repo: https://github.com/jacob-kraniak/cybersafe_smb

**Guiding Principle:** Build credibility affordably → generate recurring revenue → fund personal certs → enable higher-value services.
