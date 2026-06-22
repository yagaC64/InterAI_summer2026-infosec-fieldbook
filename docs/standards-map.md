# Standards Map

This map keeps the class review lightweight while giving students professional vocabulary.

## Baseline References

| Reference | Use in this class | Notes |
| --- | --- | --- |
| [NIST SP 800-218 SSDF v1.1](https://csrc.nist.gov/pubs/sp/800/218/final) | Secure development practices | Primary baseline for secure software development language. |
| [NIST CSF 2.0](https://www.nist.gov/cyberframework) | Risk management vocabulary | Use for broad outcomes: Govern, Identify, Protect, Detect, Respond, Recover. |
| [OWASP Top 10 2025](https://owasp.org/www-project-top-ten/) | Web application risk categories | Use to describe common web app problems in plain language. |
| [CIS Controls v8.1](https://www.cisecurity.org/controls/v8-1) | Practical hygiene | Good for basic actions: inventory, access control, secure configuration, vulnerability management. |
| [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) | Selected control vocabulary | Use only when it clarifies a finding. Do not turn class reviews into fake compliance audits. |

NIST SP 800-218 Rev. 1 / SSDF v1.2 is an initial public draft as of this fieldbook's creation, so this repo uses SSDF v1.1 as the stable baseline.

## Class Review Mapping

| Class review task | Plain-language question | Helpful reference language |
| --- | --- | --- |
| Repo purpose | Can a new reviewer understand what this project does? | SSDF: well-defined development practices; CSF: Govern |
| README and setup | Can someone build or run it without guessing? | SSDF: documentation and maintainability |
| Secret hygiene | Are passwords, keys, tokens, or private files exposed? | CIS: data protection; NIST 800-53: IA, AC, SC, SI families |
| Dependency hygiene | Are dependencies declared and reasonably current? | SSDF: vulnerability prevention and remediation; CIS: vulnerability management |
| Web input handling | Does the app trust user input too easily? | OWASP Top 10 |
| Authentication and access | Are admin/user flows protected where they exist? | OWASP Top 10; NIST 800-53: AC and IA vocabulary |
| Logging and evidence | Could a maintainer understand what happened without exposing private data? | CSF: Detect and Respond; NIST 800-53: AU and IR vocabulary |
| Safe contribution flow | Are fixes proposed in small, reviewable changes? | SSDF: secure development process; CSF: Govern |

## What Not To Do

- Do not claim a repo is compliant because a checklist was filled out.
- Do not publish exploit steps.
- Do not scan or attack systems outside explicit class scope.
- Do not paste secrets into issues, comments, screenshots, or pull requests.
- Do not confuse a public teaching review with a formal security assessment.
