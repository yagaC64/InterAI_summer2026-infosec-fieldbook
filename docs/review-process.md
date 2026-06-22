# Review Process

Use this workflow for a public class repo listed in the Notes column of the class catalog.

Catalog:

- https://github.com/yagaC64/InterAI_summer2026/blob/main/CLASS_GITHUB_CATALOG.md

## 1. Pick A Target

Choose a repo from the catalog Notes column. Stay inside public class material or your own repo.

Record:

- repo URL
- reviewer GitHub handle
- review date
- whether you opened an issue, pull request, or private instructor note

## 2. Confirm Public-Safe Scope

Before reviewing, confirm:

- the repo is public
- the repo belongs to a class participant or instructor-approved target
- you are not reviewing private accounts, private files, or unrelated infrastructure

If the scope is unclear, stop and ask the instructor.

## 3. Read First

Read the README and visible project files before running tools.

Ask:

- What does the project claim to do?
- How should it run?
- What language/framework does it use?
- Does it appear to be a static site, web app, game, API, notebook, or other project?

## 4. Check For Public Content Safety

Look for obvious public-repo problems:

- real names or emails that do not need to be public
- API keys, passwords, tokens, private keys, or `.env` files
- local machine paths
- screenshots that expose private data
- generated files that should not be committed

Do not quote secrets. Report suspected secrets privately.

## 5. Check Build And Dependency Hygiene

Look for:

- dependency manifests such as `package.json`, `requirements.txt`, `pyproject.toml`, or lockfiles
- setup instructions
- build or run commands
- pinned or reproducible dependency state
- obvious stale or abandoned packages

For class reviews, explain dependency concerns simply. Do not bury classmates in raw scanner output.

## 6. Check Basic App Security

Use the project type to guide review:

- Static page: unsafe scripts, external embeds, hidden private data, broken links
- Web app/game: input handling, unsafe DOM use, exposed configuration
- API/backend: auth, environment variables, error handling, data exposure
- Notebook/data project: private data, tokens, generated outputs, unsafe downloads

Use OWASP language when it helps, but keep findings understandable.

## 7. Write Findings Respectfully

Each finding should include:

- short summary
- evidence without leaking private data
- impact
- suggested fix
- optional framework note

Use [templates/finding.md](../templates/finding.md).

## 8. Prefer Small Pull Requests

Good pull requests:

- fix one clear issue
- avoid unrelated formatting churn
- explain the change
- preserve project style

Do not rewrite a classmate's project just because you can. That is not mentorship; that is ego with a keyboard.

## 9. Escalate Sensitive Issues Privately

Use a private instructor note when:

- a real secret may be exposed
- personal data appears in the repo
- a finding could embarrass a student if posted publicly
- you are unsure whether the issue is safe to publish

## 10. Close The Loop

When done, record:

- what was reviewed
- what was opened publicly
- what was sent privately
- what remains unresolved
