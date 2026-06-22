# Exercise 02: Secret And Privacy Hygiene

Goal: learn how to recognize sensitive material without republishing it.

## Look For

- `.env` files
- token-looking strings
- private keys or certificates
- hardcoded passwords
- personal emails, phone numbers, addresses, or IDs
- screenshots that expose accounts, dashboards, terminals, grades, or private messages
- local paths that reveal unnecessary machine/user details

## Public-Safe Reporting

If you suspect a real secret, do not quote it.

Use wording like:

```text
I found a credential-like value in a committed configuration file. I am not quoting it publicly. Please remove it and rotate it if real.
```

## Output

Use [templates/finding.md](../templates/finding.md), but keep sensitive details out of the public version.

## Reflection

Answer:

1. What made the evidence sensitive?
2. What could be safely shared?
3. What should be sent privately?
4. What fix would prevent recurrence?
