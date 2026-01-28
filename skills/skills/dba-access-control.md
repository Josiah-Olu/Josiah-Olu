# dba-access-control

**Description:** Generate least-privilege access patterns, permission review scripts, and audit-friendly documentation for SQL Server.

**Summary:** Access control + audit helper

---

## Inputs (copy/paste)
- Requested access in business terms
- Auth pattern (SQL login vs AD group)
- Existing role memberships/permissions output (sanitized) if available

## Output
- Recommended role model
- Diagnostics scripts (read-only)
- PROPOSED CHANGE scripts (requires review)
- Verification + audit notes

## Safety
Avoid broad grants (db_owner) unless explicitly requested and risks are acknowledged.
