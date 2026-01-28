# dba-monitoring

**Description:** Interpret Redgate Activity Monitor highlights and summarize actionable DBA next steps.

**Summary:** Monitoring summary + triage

---

## Inputs (copy/paste)
- Redgate Activity Monitor highlights (top waits, CPU/IO, blocking)
- Time window and whether it is ongoing
- Any top queries surfaced (if available)

## Output (required structure)
1) Summary
2) Assumptions
3) Evidence to collect (T-SQL DMVs; read-only)
4) Likely causes (ranked)
5) Remediation options (safe first)
6) Verification checklist
7) SQL 2012–2022 compatibility notes

## Provide read-only evidence queries
- Active requests + wait types (sys.dm_exec_requests + sys.dm_exec_sessions)
- Blocking chain (blocking_session_id)
- Wait stats snapshot (sys.dm_os_wait_stats)
