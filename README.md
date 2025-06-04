# .github

Workflow template.

`$default-branch` is interpolated at the time of including workflow template.
```
  push:
    branches: [ $default-branch ]
  pull_request:
    branches: [ $default-branch ]
```
