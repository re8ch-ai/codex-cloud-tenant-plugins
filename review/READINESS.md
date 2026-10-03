# Re8ch public plugin review preparation

Prepared 2026-10-04 from official/main 23f5fda. This is a draft, not a claim of completed review.

Production MCP: https://tools.service.re8ch.com/tenant-native/mcp (443).
Issuer: https://db-rw.re8ch.com/auth/v1.
Resource metadata: https://tools.service.re8ch.com/.well-known/oauth-protected-resource/tenant-native/mcp.

## Import file

chatgpt-app-submission.json contains listing copy, five positive and three negative proposed review cases, plus annotation justifications for the five read-only tools used by those cases. It does not cover all advertised tools. Validate the remaining tool annotations after the authenticated scan; never imply that this subset is a complete tool audit. Expected results are acceptance criteria, not recorded test results.

## Required remaining evidence

- OpenAI draft domain ownership verification at the origin-root /.well-known/openai-apps-challenge path. The draft currently says not verified. Publish the draft-issued public challenge through reviewed GitOps, then click Verify Domain.
- Complete the currently open RE8CH OAuth sign-in so OpenAI can scan tools. Use a dedicated ordinary reviewer tenant with sample data, not the platform administrator account for the public baseline.
- Provision persistent reviewer access and sample resources; keep credentials out of this package and enter them only in the secure dashboard. Verify sign-in, refresh, revoke, tenant isolation, resource planning, and required write/delete confirmations against that account.
- Review every scanned tool’s readOnlyHint/destructiveHint/openWorldHint and security scheme against actual behavior; do not label the generic platform dispatcher read-only.
- Supply/verify owned logo assets, publisher identity, website, privacy policy, support contact, country availability, and a walkthrough video. Do not invent URLs or attestations.
- Execute the five positive and three negative cases and record observed results. The cases here have not yet been run with the reviewer account.
- Review the policy attestations before submitting. Nothing has been submitted or published.

Official references:
https://developers.openai.com/plugins/deploy/submission
https://developers.openai.com/plugins/deploy/app-review
https://developers.openai.com/plugins/schemas/chatgpt-app-submission.v1.json
