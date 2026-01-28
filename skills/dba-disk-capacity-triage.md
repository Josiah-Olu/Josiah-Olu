# dba-disk-capacity-triage

**Description:** Triage disk space/storage utilization issues for SQL Server on Windows; provide mitigations and prevention.

**Summary:** Disk + capacity triage

---

## Inputs (copy/paste)
- Volume free space snapshot (drive letters/mount points)
- Which SQL files are growing (data/log/tempdb/backups)
- Recent changes (deployments, index maintenance, loads)
- Current file growth settings if available

## Output
- Immediate containment (lowest risk first)
- Evidence plan (where growth is coming from)
- Prevention plan (right-sizing, growth settings, retention)
- Verification steps

## Safety
- Do not recommend shrinking as a default; only discuss with strict conditions + downsides.
