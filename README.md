# GitHub Required Review Check

This is a fork from [Action Required Review](https://github.com/Automattic/action-required-review), it adds the ability to use `pr-opened-by` in the requirements specification.

## Example

```yaml
requirements: |
  - paths: unmatched
    teams:
      - maintenance
      - pr-opened-by:
        - devops
```

This means the matched paths have to be either reviewed by the `maintanance` group or the PR was oppened by `devops`.

Read more about the usage in [Action Required Review](https://github.com/Automattic/action-required-review).
