# Quantitative Risk Assessment Research: ALE/ARO for CyberSafe SMB Audits

## Overview
**Date research initiated:** approx. January 2025  
**Last updated:** February 05, 2026  
**Status:** Early implementation planning – templates & calculator POC pending

This document captures focused research and planning from Grok conversations on integrating **Annual Loss Expectancy (ALE)** and **Annual Rate of Occurrence (ARO)** calculations into CyberSafe SMB service offerings. The goal is to add credible, dollar-based risk quantification to reports (especially Pro tier) to increase perceived value, improve upsell conversion, and differentiate from generic checklist services.

## Business Rationale
- SMB owners respond strongly to financial impact (“You could lose ~$8,400/year to ransomware”) vs. abstract severity levels.
- Strengthens justification for $250 Pro package (report + 2h consult + 3mo monitoring).
- Creates natural upsell path to ongoing $12–$19/mo monitoring (“Reduce expected loss by 60–80%”).
- Aligns with NIST CSF / ISO 27001 / SOC 2 concepts without misleading certification claims.

## Core Concepts Implemented
- **Single Loss Expectancy (SLE)** = Asset Value × Exposure Factor  
- **Annual Loss Expectancy (ALE)** = SLE × Annual Rate of Occurrence (ARO)  
- Target 4–6 key SMB-relevant threats: ransomware, phishing/BEC, data breach (customer records), payment card compromise, operational downtime.

### Simplified SMB Approach
- Use **industry benchmarks** (Verizon DBIR, FBI IC3, Advisen, etc.) for baseline ARO and Exposure Factor ranges.
- Adjust ARO up/down based on audit posture (e.g., no 2FA → +50% phishing ARO).
- Asset Value derived from client-provided inputs: annual revenue, daily revenue, customer record count, tolerable downtime hours.
- Keep fully lightweight – no expensive tools or invasive scans required.

## Tiered Integration Plan
- **Basic ($40)**: Qualitative only (severity counts, recommendations).
- **Premium ($100)**: Aggregated ALE range (“Total expected annual cyber loss: $4,200–$12,000”).
- **Pro ($250)**: Detailed ALE table per threat + charts + prioritized dollar-impact recommendations.

## Low-Cost Asset Footprint Quantification Methods
### Manual / Guided (Premium/Pro baseline)
- One-page Google Sheets/Docs template filled during consult or pre-submission.
- Categories: servers/workstations, laptops/phones, POS/payment systems, cloud services (M365, Google Workspace, QuickBooks), routers, IoT/smart devices.
- Client provides count, age, primary use → used to estimate Asset Value.

### Optional Lightweight Automated (Pro upsell value-add)
- **Nmap** (free): Basic network discovery (IP devices, OS, open ports) – guided run from client laptop or during consult (with permission).
- **Spiceworks Inventory** (free ad-supported): Agentless network scan for hardware/software.
- **Snipe-IT** (free self-hosted): Manual entry + Nmap import.
- **Open-AudIT** (free tier): Lightweight Windows scanner.

All methods emphasize privacy: client controls data sharing; no persistent agents or cloud upload required unless they choose.

## Planned Deliverables (POC Phase)
1. Google Sheets ALE Calculator Template  
   - Inputs: revenue, records, downtime tolerance  
   - Benchmarks tab (pre-filled ranges by industry/threat)  
   - Auto-adjust ARO via audit score modifiers  
   - Output: per-threat ALE table + total range + chart

2. Asset Inventory Template (Google Sheets/Docs)  
   - Categorized prompts for common SMB types (retail, trades, services)

3. Updated Pro Report Section  
   - “Quantitative Risk Summary” table  
   - “Tech Footprint Overview” summary

## Challenges & Mitigations
- Benchmark accuracy for diverse SMBs → Use conservative mid-range values + clear disclaimers.
- Client comfort with numbers → Frame as “estimated industry-informed range” not precise forecast.
- Manual effort per report → Automate via Sheets formulas + Apps Script (future).

## Next Actions
- [ ] Build & test ALE calculator prototype in Google Sheets (4–6 hrs)
- [ ] Draft asset inventory template (2–3 hrs)
- [ ] Document Nmap/Spiceworks one-pager guidance for consults (2 hrs)
- [ ] Integrate into Pro report template & pilot on next 2–3 clients
- [ ] Add disclaimer language re: estimates & non-certification

## Related Repo Locations
- Main documentation: `/docs/`
- Report templates: `/templates/`
- Future automation: `/scripts/` (Google Apps Script or Python helpers)

This research directly supports enhancing the Pro package value proposition and should be revisited after first client pilots for refinement.
