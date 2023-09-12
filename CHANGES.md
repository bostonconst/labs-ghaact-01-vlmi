# CHANGES.md

## create an github-action

feat: init an github action

```bash
mkdir -p .github/workflows/
touch .github/workflows/01-action.yml
```

Empty workflow file runs but fails (any branch name) with message

```txt
Annotations
1 error
Error: .github#L1
No event triggers defined in `on`
```
