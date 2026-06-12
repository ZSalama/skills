---
name: score-last-commit
description: Review changes since the last commit and score the diff for code quality.
---

# Review Uncommitted Changes

Review the code changes made since the last commit and give a concise quality assessment.

## Scorecard

Score each category from 1–10, where 1 is poor and 10 is excellent.

| Category                 | What to judge                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------- |
| Maintainability          | How easy this code will be to change for future features.                                         |
| Comments                 | Whether comments are useful, accurate, and appropriately sparse.                                  |
| Function/Variable Naming | Whether names are descriptive, project-appropriate, and self-documenting without being bloated.   |
| Clarity                  | How easily a human or machine can understand the code as written.                                 |
| Verbosity                | Whether the code is concise and avoids unnecessary custom logic or boilerplate.                   |
| Engineering              | Whether the solution is simple, elegant, robust, and not over-engineered.                         |
| Senior Developer Energy  | Whether a strong senior developer would approve of the judgment, taste, and production-readiness. |

## Output

Use this format:

```md
# Review: Uncommitted Changes

## Summary

Briefly describe what changed and your overall impression.

## Scores

| Category                 | Score | Notes |
| ------------------------ | ----: | ----- |
| Maintainability          |  N/10 | ...   |
| Comments                 |  N/10 | ...   |
| Function/Variable Naming |  N/10 | ...   |
| Clarity                  |  N/10 | ...   |
| Verbosity                |  N/10 | ...   |
| Engineering              |  N/10 | ...   |
| Senior Developer Energy  |  N/10 | ...   |

## Main Issues

- List the most important issues, with file/function references where useful.

## Recommended Fixes

1. Highest-priority fix.
2. Next fix.
3. Optional polish.

## Verdict

Choose one:

- Ready to commit
- Ready after minor cleanup
- Needs revision
- High-risk / needs deeper review

End with a brief explanation.
```

Be direct. Avoid nitpicks unless they materially affect readability, maintainability, correctness, or production quality.
