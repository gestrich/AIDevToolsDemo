---
description: Files should not contain FIXME comments left in submitted code.
category: code-quality
new_code_lines_only: true
max_comments_per_file: 3
violation_regex: "FIXME"
violation_message: "FIXME comments should be resolved or converted to tracked issues before merging."
applies_to:
  file_patterns: ["*.txt", "*.md", "*.swift", "*.py", "*.js", "*.ts"]
---

# No FIXME Comments

Code submitted in pull requests should not contain `FIXME` comments. These indicate unfinished work and should either be resolved before merging or converted to tracked issues.

## Requirements

Remove or resolve any `FIXME` comments before merging:

```
# ❌ Bad: FIXME left in submitted code
FIXME: this needs to be cleaned up

# ✅ Good: resolved or tracked elsewhere
# See issue #42 for cleanup plan
```

## GitHub Comment

`FIXME` comments should be resolved or converted to tracked issues before merging.
