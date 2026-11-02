# Security Standards

This document establishes the security policies and defensive controls enforced across all automation repositories.

---

## 1. Webhook Endpoint Defense

1. **HMAC Signature Verification**: All webhook endpoints must verify the incoming cryptographic signature header (`X-Hub-Signature-256` or equivalent) using a shared secret before parsing the payload.
2. **Payload Size Limits**: Strict payload body limits (maximum 1 MB) to prevent denial-of-service memory exhaustion attacks.
3. **Replay Protection**: Timestamps embedded in webhook headers must be checked against the current server time with a maximum allowable drift of 5 minutes.
4. **IP Allow-listing**: Where supported by providers, restrict webhook ingress to known provider IP ranges.

---

## 2. Credential Storage and Secret Sanitization

- Git commits must never include tokens, passwords, private keys, or actual webhook secrets.
- Workflow JSON files (n8n, Postman) must be audited and stripped of credentials before committing.
- In production, credentials must be retrieved from secure secret stores (AWS Secrets Manager, HashiCorp Vault, Kubernetes Secrets).

---

## 3. Output Sanitization & Logging Hygiene

- Sensitive fields (credit card numbers, passwords, authorization tokens, PII) must be masked or redacted before emitting logs.
- Error responses returned to external callers must never leak stack traces, internal IP addresses, or database schema details.
