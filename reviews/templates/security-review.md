# Security Review Template

## Project: [NOMBRE]
## Auditor: security-auditor
## Date: [FECHA]
## Scope: [PR #X | Full codebase | Specific file]

## Executive Summary
[Resumen de 2-3 lineas]

## Findings

### Critical (must fix before merge)
| # | Issue | File | Line | Remediation |
|---|-------|------|------|-------------|
| 1 | [issue] | [file] | [line] | [fix] |

### High (fix within 24h)
| # | Issue | File | Line | Remediation |
|---|-------|------|------|-------------|
| 1 | [issue] | [file] | [line] | [fix] |

### Medium (fix within 1 week)
| # | Issue | File | Line | Remediation |
|---|-------|------|------|-------------|
| 1 | [issue] | [file] | [line] | [fix] |

### Low (informational)
| # | Issue | File | Line | Note |
|---|-------|------|------|------|
| 1 | [issue] | [file] | [line] | [note] |

## Dependency Scan
- npm audit / pip audit results: [CLEAN|X vulnerabilities]

## Verdict
- [ ] PASS - No critical/high findings
- [ ] CONDITIONAL PASS - High findings with remediation plan
- [ ] FAIL - Critical findings must be fixed
