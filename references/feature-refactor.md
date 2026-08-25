# Feature or Refactor

Use this workflow for new behavior, changed behavior, migrations, and behavior-preserving structural changes.

## Define the shape

State the user-visible outcome and the important data shape. Identify where external data enters, where state lives, and which existing callers or consumers must remain compatible.

Inspect current patterns before designing a new one. Prefer the project's established architecture when it supports the requirement cleanly.

## Choose a design

Prefer the design with fewer concepts, less shared mutable state, and a shorter path from input to outcome. Avoid adding a wrapper, service, option, or compatibility layer for a single use unless it encodes a real boundary.

When two approaches have materially different consequences and observation can decide, build the cheapest disposable probe or benchmark. Do not ask the user to settle a technical fact that the system can reveal.

## Implement and prove

Implement a narrow end-to-end slice before expanding across callers. Keep each migration step in a verifiable state. When feasible, migrate callers and remove the obsolete internal API in the same change rather than maintaining two paths indefinitely.

Verify:

- the requested user-visible behavior;
- the invariant that must not regress;
- affected tests and static checks;
- the final diff and repository state.

For a pure refactor, demonstrate behavior preservation with existing tests or a before-and-after observable comparison.
