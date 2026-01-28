# dba-job-duration-triage

**Description:** Analyze prolonged SQL Agent job durations; produce a triage and optimization plan.

**Summary:** SQL Agent duration analysis

---

## Inputs (copy/paste)
- Job + step name
- Typical duration vs current duration
- Job history snippet (last 10–30 runs if possible)
- Step command text (sanitized) if T-SQL

## Output
- Regression vs trend assessment
- Evidence queries (read-only)
- Potential causes (blocking, IO, tempdb, stats, external dependencies)
- Remediation options + verification

## Notes
- Do not assume Query Store unless SQL 2016+ and user confirms it is enabled.
