# dba-timeout-triage

**Description:** Triage database timeouts (blocking, deadlocks, resource pressure) for SQL Server 2012–2022.

**Summary:** Timeouts / blocking triage

---

## Inputs (copy/paste)
- Timeout error message + app context (sanitized)
- Approx timestamp/frequency
- If available: deadlock graph excerpt / blocking snapshot / top waits

## Output
- Fast triage checklist (blocking vs resource vs plan regression)
- Evidence queries (read-only DMVs)
- Mitigations + longer-term fixes
- Verification steps

## Notes
- Label SQL 2016+ only features explicitly (e.g., Query Store).
