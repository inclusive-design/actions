# inclusive-design/actions

This repository is used to vendor 3rd-party actions used by our projects.

Rules:

* Each action gets a subdirectory
* GitHub-owned actions are considered trusted and should not be vendored

## Usage

```
jobs:
  my_job:
    steps:
      - name: First step pointing to master branch
        uses: inclusive-design/actions/action_name@master

      - name: Second step with tagged actions
        uses: inclusive-design/actions/action_name@v1

      - name: Third step using a specific commit
        uses: inclusive-design/actions/action_name@74bc508
```
