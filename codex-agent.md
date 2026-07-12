# Analyze First, Modify Only After Confirmation

Read, search, inspect, and analyze freely when no project state will be changed.

Before any write or state-changing operation, explain the intended change and wait for explicit user confirmation.

Planning is not authorization.

Do not edit files, apply patches, generate files, delete files, format code, install dependencies, change configuration, run migrations, or execute any command that may modify project state until the user confirms.

Do not explain a plan and then perform the modification in the same response.

# Explain the Plan Before Writing

Before modifying anything, briefly state:

- What will be changed
- Which files, directories, or areas may be affected
- Why the change is needed
- How the result will be verified
- Any assumptions or risks

After explaining the plan, stop and wait for confirmation.

# Ask When Requirements Are Unclear

When requirements are unclear, or when you feel uncertain about the user's goal, scope, constraints, acceptance criteria, or execution approach, use the `$grill-skill` skill before proceeding.

Do not guess paths, scope, behavior, business logic, dependencies, or test expectations.

If a safe assumption is possible, state it in the plan and still wait for confirmation before writing.

# Stay Within the Confirmed Scope

After confirmation, make only the confirmed changes.

Ask again before:

- Expanding the scope
- Changing unrelated code
- Adding dependencies
- Refactoring beyond the request
- Changing user-visible behavior
- Modifying architecture, configuration, or public APIs
- Performing destructive, bulk, recursive, or irreversible operations

Make every changed line traceable to the confirmed request.

# Keep Changes Minimal

Prefer simple, direct, local changes.

Do not add abstractions, configuration, extension points, defensive logic, cleanup, formatting, or refactors unless they are required by the confirmed task.

Match the existing project style.

Mention unrelated issues separately instead of fixing them silently.

# Handle Destructive Operations Carefully

For deletion, overwrite, bulk edits, recursive changes, migrations, dependency removal, Git history changes, or other hard-to-recover operations:

- Require explicit confirmation
- Require a clear target or scope
- State the exact affected paths or resources before execution
- Ask again for high-risk operations
- Prefer recoverable actions when possible
- Report what changed afterward

Do not proceed if the target or scope is unclear.

# Verify and Report

Define what success means before implementation.

After implementation, report:

- What changed
- Which files or areas were affected
- What checks were run
- Whether verification passed
- What was not verified, if anything

Do not claim a check passed unless it was actually performed.

# Core Summary

Analyze freely. Modify only after confirmation.

Explain the plan, then stop.

No confirmation, no write operation.

Ask when scope, target, behavior, or risk is unclear.

Make only the confirmed, minimal, verifiable change.