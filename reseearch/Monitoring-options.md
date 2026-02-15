# CyberSafe Business Plan – Expansion Roadmap Recap
**Conversation Date:** ~February 2026  
**Focus:** Evaluating paths to scale CyberSafe from manual/form-based cybersecurity assessments into more automated, recurring-revenue offerings (compliance tooling, monitoring, SIEM/XDR integration).  
**Prepared by:** Your Grok Business Partner & PM

## Core Current State (Reminder)
- **Service Model**: Tiered audits via Google Forms/Sheets → personalized reports + consults
  - Basic: $40 (15 points)
  - Premium: $100 (30 points + 1h consult)
  - Pro: $250 (50 points + 2h consult + 3 months monitoring)
- **Target**: Primarily low-to-mid tech-savvy SMBs (hairdressers, mechanics, etc.) + individuals
- **Tools/Infra**: Carrd site, Google Workspace stack, Zoho Books invoicing, manual report generation
- **Lead Flow**: Free 15-pt audit → score → upsell emails → paid package form → delivery
- **Retention**: Post-consult follow-ups, $12/mo optional monitoring, quarterly re-engagement
- **Differentiation**: Simplified, affordable, framework-aligned (inspired by NIST CSF, ISO 27001, SOC 2) without claiming formal certification

## Key Questions Discussed

### Q1. Expanding into automated compliance tooling (Vanta / Drata / Secureframe style)
**Assessment**: Moderately achievable in 18–36 months, **significant pivot** from service to SaaS. **High cost & risk**, but high upside for mid-market SMBs needing SOC 2 / compliance readiness.

| Aspect              | Summary                                                                 | Verdict                  |
|---------------------|-------------------------------------------------------------------------|--------------------------|
| Practicality        | Possible with phased approach; overkill for core low-tech audience       | Worth pursuing **if** Pro tier traction is strong |
| Cost Impact         | $100k–500k dev + $50k+/yr maintenance; high burn if bootstrapped         | Major financial lift     |
| Market Fit          | Strong for 50–200 employee SMBs; taps $10B+ compliance market            | Good long-term differentiator |
| Roadmap (3 Phases)  | 0–6 mo: Validate + prototype (Zapier/MVP) <br>6–18 mo: Beta build & test <br>18–36 mo: Full SaaS launch | Start small, demand-first |

**Recommendation**: Only pursue aggressively if you see 30–50+ Pro Package customers and clear demand for automation in surveys. Otherwise → defer and focus on monitoring upsells first.

### Q2. DIY / Open-Source Compliance Platform (fork Comp AI or build from scratch)
**Assessment**: More achievable solo/bootstrapped than proprietary SaaS path. Lower cost, higher control, but still **high effort** to maintain and polish.

| Aspect              | Summary                                                                 | Verdict                  |
|---------------------|-------------------------------------------------------------------------|--------------------------|
| Feasibility         | High if forking (e.g. Comp AI); medium-high if greenfield                | Realistic with your skills |
| Cost                | $5k–20k initial (hosting, domains, basic audit); mostly time             | Much leaner than Vanta-like |
| Edge                | “Open & affordable” positioning; community potential                     | Attracts privacy-focused users |
| Risks               | Maintenance burden, security exposure if not hardened                    | Need disciplined updates |

**Recommended Path**:
1. Research/fork open-source base (0–3 mo)
2. MVP: Integrate your 50 AP points + basic evidence collection (3–6 mo)
3. Launch as $50–100/mo add-on to Pro tier
4. Push code to GitHub repo for versioning / credibility

**Verdict**: Strong “next step” if you want automation without massive burn. Prioritize over full Vanta clone.

### Q3. Vertical Integration via Monitoring / SIEM / XDR (Wazuh, Huntress, etc.)
**Assessment**: **Highly practical & aligned** with current Pro tier (already includes 3 months monitoring). Leverages your employer SIEM/SOAR/XDR knowledge. Fastest path to recurring revenue.

| Tool       | Type              | Cost (approx)             | SMB Fit & Recommendation                          |
|------------|-------------------|---------------------------|----------------------------------------------------|
| Wazuh      | Open-source SIEM/XDR | Free core + ~$500–$2k/mo cloud/hosted | Best for cost control & customization → **primary choice** |
| Huntress   | Managed EDR/SIEM  | $5–10/endpoint/mo         | Hands-off, trusted → good upsell for non-technical clients |

**Roadmap**:
1. **0–3 mo**: Pilot Wazuh on 5–10 Pro clients (dark web + endpoint alerts)
2. **3–9 mo**: Bundle as $12–20/mo tier; add Huntress option for premium
3. **9–18 mo**: Scale to standalone product; aim 30% upsell rate from existing base

**Verdict**: **Highest priority near-term expansion**. Turns one-time audits into sticky $12+/mo revenue. Start with Wazuh for margins.

## Overall Prioritization (as of Feb 2026)
1. **Top Priority (Next 6–12 mo)**  
   - Scale current manual/service model (more leads, better conversion, testimonials)  
   - Launch enhanced $12/mo monitoring (Wazuh-based pilot) → prove recurring revenue  
   - Survey Pro customers on automation interest

2. **Mid-Term (12–24 mo)**  
   - Build/fork lightweight open-source compliance & monitoring dashboard  
   - Offer as $50–150/mo upsell tier

3. **Long-Term / Stretch (24+ mo)**  
   - Full automated compliance platform if mid-market traction emerges  
   - Consider Huntress partnership or white-label for managed services

## Next Immediate Actions (Suggested)
- Run quick survey to current/ex-Pro leads: “Would you pay $X/mo for automated monitoring / compliance evidence collection?”
- Set up Wazuh test instance → document in repo
- Update package tiers sheet with clearer monitoring upsell language
- Schedule 30-min review call to align on Q1 priorities

Let me know which of these you want to deep-dive next or if you'd like me to expand any section into a full mini-project plan.
