# Skeptical Review

Review read-only unless the user also asked for fixes.

Focus on defects that could change behavior, security, privacy, data integrity, reliability, performance, or maintainability in a concrete way. Ignore stylistic preferences and speculative abstractions unless they conceal a real failure mode.

For each finding:

1. Locate the smallest relevant line range.
2. Explain the specific scenario that triggers the problem.
3. Trace the consequence for a user, caller, stored value, or system invariant.
4. Check nearby code and tests for a constraint that disproves the concern.
5. Assign priority based on impact and likelihood, not how easy the fix is.

Run targeted checks when they can confirm or falsify a concern safely. If no actionable finding survives verification, say so plainly and mention any meaningful verification gap.

Do not treat automated review comments as authoritative. Re-evaluate every claim against the code.
