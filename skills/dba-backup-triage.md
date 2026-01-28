# dba-backup-triage

**Description:** Triage failed SQL Server backups (including Ola Hallengren jobs) using copy/paste evidence.

**Summary:** Backup failures triage

---

## Inputs (copy/paste)
- SQL Agent job name + step output (failing step)
- Error message text (from job output / error log snippet)
- Backup destination type (local disk vs UNC)
- Free space snapshot for the target volume/share
- If Ola: whether CommandLog rows exist for the failure window (paste if possible)

## Output
- Ranked root-cause hypotheses
- Evidence plan (exact queries/checks)
- Remediation options (lowest risk first)
- Verification steps

## Provide read-only queries
- msdb backup history (backupset)
- job history (msdb sysjobhistory/sysjobs)
