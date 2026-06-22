# Evidence Handling

Security evidence has to be useful without becoming a new leak.

## Public-Safe Evidence

Safe evidence usually includes:

- repo-relative paths
- line numbers when they do not expose secrets
- short descriptions of behavior
- screenshots that do not show private data
- dependency names and versions
- links to public GitHub files or pull requests

## Protected Evidence

Keep evidence private when it includes:

- tokens, passwords, private keys, credentials, session IDs, or webhook secrets
- private names, emails, phone numbers, addresses, grades, or identity mapping
- screenshots with private account data
- exploit chains or step-by-step abuse instructions
- NDA, MOU, customer, employer, or incident material

## Secret-Like Values

If a value looks like a real secret:

1. Do not paste it into a public issue.
2. Do not include it in screenshots.
3. Record the repo-relative file path and a safe description.
4. Tell the instructor or repo owner privately.
5. Recommend removal and rotation if the value is real.

Example public-safe wording:

```text
This repo appears to contain a credential-like value in a committed configuration file. I am not quoting it here. Please remove it from history if needed and rotate it if it is real.
```

## Class Evidence Folder

When this fieldbook stores validation reports, use:

- `tests/test_results/` for tracked, sanitized summaries
- `tests/test_results/protected/` for local-only sensitive evidence

Do not commit protected evidence.
