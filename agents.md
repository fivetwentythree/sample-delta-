# Agent guide

## Project context

This repository is currently a starting point: it has no application code,
declared technology stack, build commands, or test suite. Do not assume those
exist. Update this guide as the project takes shape, keeping its instructions
specific, accurate, and easy to follow.

## Working principles

- Understand the request and inspect relevant files before changing anything.
- Make the smallest coherent change that solves the problem, not just its symptoms.
- Follow existing conventions and reuse established patterns.
- Prefer clear names and straightforward code over clever abstractions.
- Keep unrelated refactors, formatting changes, and new dependencies out of scope.
- Ask a focused question when missing information would materially change the result.

## Repository guidance

- Read applicable `AGENTS.md`, `AGENT.md`, and `agents.md` files before editing.
  Follow more specific directory guidance where it applies.
- Treat repository files as the source of truth for project structure and commands.
- When adding the first implementation, document its setup, run, and verification
  commands in a `README.md`.
- Introduce dependencies only when they provide a clear benefit. Use the project's
  chosen package manager and keep its lockfile consistent.
- Do not edit generated files directly when their source or generator is available.

## Making changes

1. Inspect the affected code, its callers, and relevant tests.
2. Choose an approach consistent with the surrounding design.
3. Implement the change with explicit handling for meaningful edge cases.
4. Add or update tests when behavior changes and a test framework is available.
5. Run the relevant checks and review the final diff for unintended changes.

Preserve work already in progress. Do not overwrite another contributor's changes
or revert unrelated edits. If concurrent changes conflict with your work, stop
and resolve the intent before proceeding.

## Verification

- Use documented project commands rather than guessing build or test commands.
- Start with focused checks, then run broader checks when the scope warrants it.
- Verify the requested behavior, not only that code compiles or tests pass.
- If a check fails, distinguish failures caused by your change from pre-existing
  failures or environment limitations.
- Never claim a check passed unless you ran it successfully.
- If no automated checks exist, state that and describe any manual validation.

## Safety and Git

- Never commit secrets, credentials, private keys, or sensitive user data.
- Avoid logging sensitive values; use placeholders in examples.
- Get explicit approval before destructive operations, publishing, deploying,
  rewriting shared history, or pushing to a shared branch.
- Do not create commits or push changes unless requested.
- Keep changes focused and reviewable; do not include temporary files or build output.

## Communication and handoff

Keep updates concise and useful. Explain consequential decisions and surface
blockers early rather than silently guessing.

When finishing, summarize:

- What changed and why.
- Which checks you ran and their results.
- What you could not verify and any remaining limitations or follow-up work.

## Maintaining this guide

Add concrete project conventions and exact commands when they become established.
Remove outdated instructions instead of accumulating contradictory rules. Keep
this file focused on information that helps the next contributor work safely
and effectively.
