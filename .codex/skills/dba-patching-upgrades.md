# dba-patching-upgrades

**Description:** Plan SQL Server patching and upgrades: pre-checks, post-checks, rollback planning, and documentation.

**Summary:** Patching + upgrade planner

---

## Inputs (copy/paste)
- Current SQL version/build + OS version
- Target CU/GDR (if known)
- Maintenance window and rollback expectations
- HA topology

## Output
- Patch/upgrade plan with pre/post checks
- Risk matrix (downtime, compatibility, HA)
- Validation scripts (read-only)
- CAB/ticket-ready narrative
