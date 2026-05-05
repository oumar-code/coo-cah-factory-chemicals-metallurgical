---
name: Regulatory / Certification Action
about: Track a SON NIS certification, NCC Type Approval, NESREA compliance action, or ISO audit action
title: "[REGULATORY] <body> — <certification/action name>"
labels: regulatory, certification, compliance
assignees: ''
---

## Regulatory Action Details

| Field | Value |
|---|---|
| **Regulatory Body** | <!-- SON / NCC / NESREA / ISO / NIPC / Ogun State EPA / Other --> |
| **Certification / Action** | <!-- e.g., "SON NIS 411 certification for CCG-INV-PSW-2kVA" --> |
| **Product SKU(s) affected** | <!-- e.g., CCG-INV-PSW-2K, CCG-INV-PSW-3K --> |
| **Standard / Regulation** | <!-- e.g., NIS 411:2020 / IEC 62040-1/2/3 / NESREA WEEE Regulations 2011 --> |
| **Action Type** | <!-- New Certification / Renewal / Surveillance Audit / Non-Conformity / Complaint --> |
| **Target Completion Date** | <!-- YYYY-MM-DD --> |
| **Responsible Team** | <!-- Quality / Engineering / Legal / Operations --> |
| **External Agency / CAB** | <!-- e.g., Intertek Nigeria / Bureau Veritas / NCC RF lab --> |
| **Date Raised** | <!-- YYYY-MM-DD --> |
| **Priority** | <!-- Critical (blocks sale) / High / Medium / Low --> |

---

## Action Plan

### Pre-Submission Requirements
- [ ] Internal pre-compliance testing completed (load bank, hipot, EMC scan at Coo-Cah RF lab)
- [ ] Technical file compiled (BOM, schematic, design drawings, test reports, user manual)
- [ ] Product samples prepared (typically 3–5 samples required by CAB)
- [ ] Factory inspection readiness confirmed (SON requires factory audit for NIS certification)
- [ ] Application fee payment arranged

### Submission
- [ ] Application submitted via regulatory portal (attach submission confirmation)
- [ ] CAB / test laboratory assigned: ___________________________
- [ ] Application reference number: ___________________________
- [ ] Submission date: ___________________________

### Testing / Assessment
- [ ] CAB documentation review: PASS / FAIL / PENDING
- [ ] CAB factory inspection: PASS / FAIL / PENDING / DATE: ___________
- [ ] Type test at accredited laboratory: PASS / FAIL / PENDING
- [ ] Test report issued: YES / NO / DATE: ___________

### Closure
- [ ] Certificate / approval issued: YES / NO / DATE: ___________
- [ ] Certificate number: ___________________________
- [ ] Certificate valid until: ___________________________
- [ ] SON C-Mark / NCC TAC / NESREA permit applied to product label: YES / NO
- [ ] Annual surveillance scheduled: DATE: ___________________________

---

## Non-Conformities (if any)

| # | NC Description | NC Raised By | Root Cause | Corrective Action | Due Date | Closed? |
|---|---|---|---|---|---|---|
| 1 | | | | | | |
| 2 | | | | | | |

---

## Impact Assessment

| Impact | Detail |
|---|---|
| **Commercial impact** | <!-- e.g., "Cannot ship CCG-INV-PSW-2kVA until SON certificate received; currently 0% external sales on this SKU" --> |
| **Internal supply impact** | <!-- e.g., "Internal supply to sister factories can proceed under 'own use' before SON cert" --> |
| **Revenue at risk** | <!-- ₦ per month blocked --> |
| **Production impact** | <!-- Can production continue pending cert? --> |

---

## Document Updates Required

- [ ] [docs/regulatory.md](../../docs/regulatory.md) updated with new certificate details
- [ ] Product label template updated in MES with certificate number
- [ ] SON C-Mark artwork updated on product label if required
- [ ] Aftersales portal updated with certification information

---

## Related Issues

<!-- Link any related GitHub issues (e.g., design changes required to pass EMC test) -->

- Relates to: #

---
*Regulatory actions follow Coo-Cah Technologies Holdings compliance governance. See master repo [oumar-code/Coo-Kah-Doks](https://github.com/oumar-code/Coo-Kah-Doks) for group-wide regulatory standards and master repo `docs/standards/iso-requirements.md` for ISO audit requirements.*
