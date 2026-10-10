---
name: commit-message
description: Write a Conventional Commits message for the staged changes, using the diff for what changed and the conversation for why. Use when the user asks to write, draft, or suggest a commit message.
license: MIT
metadata:
  author: trevor-lambert
  version: "1.0.0"
---

# Commit message

Write a commit message for the staged changes. Print it. Don't run `git commit`.

## Process

1. **Prepare.** Read [the writing rules](references/writing.md).
2. **Gather.** Run `git diff --staged` for what changed. If nothing is staged, use `git diff` and say so in the output. Read the conversation for why the change was made, which the diff can't show. Don't invent reasons.
3. **Subject.** Write `type(scope): subject`.
   - type: `feat`, `fix`, `refactor`, `perf`, `docs`, `test`, `build`, `ci`, `chore`, `style`, or `revert`. Pick the one that matches the main change.
   - scope: optional. Use the module, package, or area the change touches, if one stands out.
   - subject: imperative, lowercase start, no trailing period, 72 characters max for the whole line.
   - Breaking change: add `!` after the type or scope.
4. **Body.** Optional. Skip it when the subject says enough. Otherwise, after a blank line, explain why the change was made and anything a reviewer can't see in the diff: the problem, a non-obvious decision, a side effect. Don't list the files or narrate the diff. Wrap lines at 72 characters.
5. **Footer.** Only when it applies, after a blank line:
   - `BREAKING CHANGE: <what breaks and how to migrate>`
   - `Refs: <ticket key>` if the conversation or branch name has a ticket key.
   - Never add AI attribution or `Co-Authored-By` lines.
6. **Split check.** If the staged changes do unrelated things, say so in one line and suggest how to split them. Still write the best single message.
7. **Check.** Go through the writing rules one by one against the message and fix every violation.
8. **Output.** Print the message in one fenced code block. Nothing else, except the one-line notes from steps 2 and 6 when they apply.
