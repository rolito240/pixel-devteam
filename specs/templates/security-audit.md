# Spec Template: Security Audit

## Project: [NOMBRE]
## Date: [FECHA]
## Scope: [full|partial|specific]

## Description
[Descripcion del alcance de la auditoria]

## Checklist OWASP Top 10
- [ ] A01: Broken Access Control
- [ ] A02: Cryptographic Failures
- [ ] A03: Injection
- [ ] A04: Insecure Design
- [ ] A05: Security Misconfiguration
- [ ] A06: Vulnerable Components
- [ ] A07: Auth Failures
- [ ] A08: Data Integrity Failures
- [ ] A09: Logging Failures
- [ ] A10: SSRF

## Additional Checks
- [ ] Hardcoded secrets
- [ ] Dependency vulnerabilities (npm audit / pip audit)
- [ ] CORS configuration
- [ ] Rate limiting

## Deliverables
- [ ] Executive summary
- [ ] Detailed findings with severity
- [ ] Remediation recommendations
- [ ] Re-test verification
