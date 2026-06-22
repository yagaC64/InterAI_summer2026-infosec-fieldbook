# Test Results And Validation Evidence

Use this folder for tracked, sanitized validation summaries.

## Public-Safe Tracked Reports

Tracked reports may include:

- markdown summaries of link checks
- secret-scan pass/fail summaries without secret values
- documentation validation notes
- build/test summaries with no private data

## Protected Local Evidence

Use `tests/test_results/protected/` for local-only evidence that should not be committed.

Examples:

- raw scanner output that may contain secrets
- screenshots with account data
- private notes from a sensitive report
- logs with local machine paths or private values

`tests/test_results/protected/` is ignored by Git.

## Rule

If evidence would embarrass someone, expose private data, or teach abuse instead of defense, keep it out of the public repo.
