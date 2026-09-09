# Local CI Production Pilot

Public real-use pilot for isolated Switzer Systems local CI.

Security:
- No secrets, client data, private client code, Azure/DB/WordPress credentials.
- Labels are routing only, never authorization.
- Never register a runner without explicit owner approval.
- Never use pull_request_target for PR-controlled code.
- Fail closed if repo/ref/SHA/actor/workflow/runner-group identity is uncertain.
- Initial workloads must be harmless: tests, linting, packaging, synthetic/public-data analysis.
