# Autonomous Run

Use this workflow when the user asks the agent to continue until a result is reached or expects to review the work later.

## Contract

Define a finish condition that can be observed, such as a test suite passing, a reproducible interaction succeeding, or a finite set of callers being migrated. Record the initial scope and do not expand it merely because adjacent work is attractive.

Break the run into units that each end with a check. Preserve useful intermediate state with focused commits only when commits are already within scope. Keep a short decision record for consequential choices, rejected approaches, and unresolved risks.

## Persistence without recklessness

- Continue through reversible local obstacles by diagnosing them and trying a materially different approach.
- Do not repeat the same failed action indefinitely. One equivalent retry is enough to classify a failure as persistent.
- Do not infer authority to message people, merge, deploy, publish, delete, purchase, or change production data from a request to “keep going.”
- Keep parallel workers isolated and assign one writer to each file, branch, or worktree.
- Reconcile worker results against the current repository state before accepting them.

## Stop conditions

Stop successfully only when the observable finish condition is met and the final state has been inspected. Stop for the user when completion requires a product choice, missing credential, unavailable external system, or new authority outside the original request.

The final report should distinguish completed, verified work from attempted, blocked, or intentionally deferred work.
