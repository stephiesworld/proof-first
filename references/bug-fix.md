# Bug Fix

Use this workflow for a defect, regression, crash, incorrect output, or unexplained runtime behavior.

1. Reproduce the symptom on the closest practical surface to the real failure. Record the input, observed output, and environment details that matter.
2. Trace the execution path from the symptom to the first incorrect assumption or state transition. Distinguish the root cause from downstream damage.
3. Add a failing automated test first when it can reproduce the behavior without brittle mocks or an artificial setup. Otherwise keep a repeatable runtime reproduction.
4. Make the smallest change at the root cause. Avoid guards that merely hide the symptom unless graceful degradation is itself the requirement.
5. Rerun the original reproduction, relevant regression tests, and the project's normal static checks.
6. Inspect the final diff for accidental scope growth, generated artifacts, debug code, and unrelated formatting.

If the defect cannot be reproduced, do not guess and declare it fixed. Report what was attempted, what was observed, the leading hypothesis, and the missing evidence needed to proceed.
