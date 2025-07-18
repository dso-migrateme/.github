# .github

This repository used for:
- Workflow templates (repo must be named `.github`)
- Required workflows (required workflow files  must be located in `.github/workflows` folder)

GitHub has strict naming requirements for Workflow templates and Required workflow files and this is a good compromise to maintain both features in one place. It is expected that this repo structure will be located in every GitHub Oragnisation where Shift-Left will be rolled out.

## Workflow templates
Workflow templates support also branch name interpolation and the template can be defined as follows:
```
  push:
    branches: [ $default-branch ]
  pull_request:
    branches: [ $default-branch ]
```
`$default-branch` is interpolated at the time of including workflow template in the target repository.

## Required workflows

Required workflows will reference this repository to inject the appropriate workflows into the subject repository.