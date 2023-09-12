# CHANGES.md

## create an github-action

feat: init an github action

```bash
mkdir -p .github/workflows/
touch .github/workflows/01-action.yml
```

Empty workflow file runs on push, but fails (any branch name) with message

```txt
Annotations
1 error
Error: .github#L1
No event triggers defined in `on`
```

## sequence of workflow

```txt
this will be github-actions-workflow session wit you

~~~

We need several files for demonstrate ability of github-actions-workflow (GHAW)

FYI: current branch is `workflows-01`

1) workflow launches on every push
workflow-every.yml
set environment variable : env_workflow_every_timestamp=$(date + %Y-%m-%d--%H-%M-%S--%N)


2) workflow launches manualy from gui
workflow-manual.yml
set environment variable : env_workflow_manual_timestamp=$(date + %Y-%m-%d--%H-%M-%S--%N)

3) workflow called by workflow-every.yml OR workflow-manual.yml
workflow-called.yml
print name of calling workflow


4) not shure, workflow or a yaml file that can be as a template, for executing reusable commands. It can be a part to be included in some workflow, for example 1 and 2 .
just echoes current time

```

feat: add chuncked workflows

```bash
touch .github/workflows/workflow-every.yml
touch .github/workflows/workflow-manual.yml
touch .github/workflows/workflow-called.yml
touch .github/workflows/commands-template.yml


```