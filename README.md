# InterAI Summer 2026 INFOSEC Fieldbook

Public defensive security fieldbook for the InterAI Summer 2026 class repos.

This repo gives students a safe, practical way to review public GitHub projects for common security, privacy, dependency, and software-delivery risks. Class repo targets come from the Notes column in the public catalog:

- [CLASS_GITHUB_CATALOG.md](https://github.com/yagaC64/InterAI_summer2026/blob/main/CLASS_GITHUB_CATALOG.md)

## Scope

This is a teaching repo, not a compliance certification, penetration test, incident report repository, or permission slip to attack systems.

Use this fieldbook only with:

- public class repos listed in the catalog
- your own repo
- repos where you have explicit permission to review and propose changes

Do not publish secrets, private names, emails, tokens, credentials, local paths, private incident details, exploit chains, or anything copied from private notes.

## Reference Frameworks

Primary teaching baseline:

- [NIST SP 800-218, Secure Software Development Framework (SSDF) v1.1](https://csrc.nist.gov/pubs/sp/800/218/final)
- [NIST Cybersecurity Framework (CSF) 2.0](https://www.nist.gov/cyberframework)
- [OWASP Top 10 2025](https://owasp.org/www-project-top-ten/)
- [CIS Controls v8.1](https://www.cisecurity.org/controls/v8-1)
- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final), selected controls only when useful for vocabulary

This repo uses those references as learning guides. It does not claim formal compliance.

## How We Will Use This In Class

Pick a public class repo from the catalog and perform a lightweight defensive review:

1. Confirm the repo has a clear purpose and safe public content.
2. Check whether the app can be built or understood from the README.
3. Look for accidental secrets, private data, unsafe examples, or risky defaults.
4. Review dependency and GitHub hygiene.
5. Identify basic web/app risks using OWASP language.
6. Write findings as respectful issues or pull requests.
7. Prefer small fixes over giant rewrite energy.

## Student-Safe Review Rule

Findings should be specific, kind, and useful.

Good:

- "This README should mention how to run the app locally."
- "This token-looking value should be removed and rotated if real."
- "This dependency file should be committed so installs are reproducible."

Bad:

- public shaming
- private identity mapping
- exploit instructions
- dumping scanner noise with no explanation

## Repo Layout

- [docs/standards-map.md](docs/standards-map.md) - short map from class review tasks to NIST, OWASP, and CIS references
- [docs/review-process.md](docs/review-process.md) - step-by-step class review workflow
- [docs/evidence-handling.md](docs/evidence-handling.md) - public-safe evidence rules
- [templates/repo-review.md](templates/repo-review.md) - student-safe review template
- [templates/finding.md](templates/finding.md) - finding format for issues or PR notes
- [exercises/](exercises/) - short defensive review exercises

## Safety Bumper

If you find something that looks like a real password, token, private key, or personal data, do not paste it into an issue. Report it privately to the instructor or repo owner with the minimum path/context needed to find it.

## License

This fieldbook is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE).

You may share and adapt the original docs, templates, and exercises in this repo, including for classroom, public, or commercial use, as long as you give attribution, link to the license, and indicate if changes were made.

Suggested attribution:

```text
InterAI Summer 2026 INFOSEC Fieldbook by yagaC64, licensed under CC BY 4.0.
```

## Maintainer Notes

This public fieldbook is intentionally separate from private INFOSEC records. Private reports, evidence packs, incident notes, and protected artifacts do not belong here.
