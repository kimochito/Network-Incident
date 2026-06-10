# Network Incident Log

A centralized repository for tracking, diagnosing, and resolving network-related infrastructure incidents. This log serves as an administrative audit trail, documenting root-cause analyses, ISP tickets, hardware failures, and perimeter security bottlenecks.

## 📂 Repository Structure

All succeeding network incidents are logged chronologically as independent Markdown files inside this repository. 
*   **Naming Convention:** File names follow the `YYYY-MM-DD.md` format (e.g., `2026-06-10.md`).
*   **Archiving:** Each file contains a localized topology map, console test outputs, and a final resolution state.

---

## 📋 Active / Recent Incident Logs

| Date | Incident Summary | Primary Node / Vendor | Status | Log File |
| :--- | :--- | :--- | :--- | :--- |
| **2026-06-10** | Outbound Latency & 40-60% Packet Loss to Cloud Services | Palo Alto / Globe Business | 🔄 Investigating | [`2026-06-10.md`](./2026-06-10.md) |

---

## 🛠️ Daily Incident Log Template

Copy and paste this template whenever creating a new daily `YYYY-MM-DD.md` incident file to maintain formatting consistency across the repository:

```markdown
# Network Incident Report: [Brief Title Here]

**Date:** YYYY-MM-DD  
**Status:** [🟢 Resolved | 🟡 Monitoring | 🔴 Critical / Active]  
**Impact Level:** [Low | Medium | High | Site-Wide Outage]  
**Affected Nodes/Sites:** [e.g., Rawis Branch Local LAN / Wan Handoff]  

---

## 1. Incident Description
*Provide a concise summary of the symptoms, user complaints, and initial discovery timeline.*

## 2. Diagnostics & Test Data
*Paste technical evidence gathered during troubleshooting (Command outputs, logs, metrics).*

### Test A: Layer 3 Ping / Traceroute Verification
\`\`\`bash
# Paste raw console outputs here
\`\`\`

### Test B: Transport Layer (`curl` / Application Performance)
\`\`\`bash
# Paste application error codes or connection handshake headers here
\`\`\`

## 3. Root Cause Analysis (RCA)
*Detail the technical mechanism causing the breakdown (e.g., ISP fiber cut, hardware freeze, expired licenses, configuration drift).*

## 4. Remediation & Action Plan
*   [ ] **Short-Term Workaround:** *Temporary fix to restore user productivity.*
*   [ ] **Long-Term Prevention:** *Permanent fix required to prevent recurrence.*
\`\`\`
```


I can provide the scripts to streamline your daily admin workflows.
