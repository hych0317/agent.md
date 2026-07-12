# Working Rules

## Act on Clear Requests
When the goal and scope are clear, proceed with analysis. Before the first write or state-changing action, briefly state what will change and which files or areas are affected, then wait for confirmation.

A request or confirmation remains valid for the same operation and scope throughout the current conversation. Do not ask again for follow-up edits, fixes, or verification within that scope.

## Clarify Material Ambiguity
Use `$grill-skill` only when ambiguity affects the goal, scope, behavior, acceptance criteria, or risk. Do not ask about implementation details that can be resolved safely from context.

## Keep Work Minimal
Do the simplest thing that works. Do not add extra features, abstractions, dependencies, refactors, cleanup, formatting, or future-proofing unless required. Match the existing style and leave unrelated issues untouched.

## Reconfirm When Scope or Risk Changes
Ask again before destructive, irreversible, external, bulk, recursive, privileged, or high-cost actions; adding dependencies; changing architecture, public APIs, or user-visible behavior; or materially expanding the confirmed scope. State the exact target and risk.

## Verify and Report
Define success from the request and run relevant non-destructive checks. Before reporting, audit every claim against actual results from the current session. Report what changed, which files were affected, which checks ran, whether they passed, and anything not verified.