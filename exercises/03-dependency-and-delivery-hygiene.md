# Exercise 03: Dependency And Delivery Hygiene

Goal: learn how dependency and delivery basics affect security.

## Look For

- missing dependency manifests
- missing lockfiles when the ecosystem normally uses them
- unclear run/build instructions
- committed build output or dependency folders
- packages that appear unused or stale
- public deploy links that do not match the repo state

## Useful Questions

1. Can someone reproduce the project locally?
2. Are dependencies declared in a standard file?
3. Is there a clear command to run or build?
4. Does the repo include generated files that make review harder?
5. Is the suggested fix small enough for a class pull request?

## Output

Open a small issue or pull request that improves setup clarity, dependency declaration, or cleanup. Keep it boring and useful. Boring useful work ships.
