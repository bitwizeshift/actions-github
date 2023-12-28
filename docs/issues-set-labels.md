# Sets labels on an issue

<!-- These docs are generated by a tool -->

A composite action for setting labels to github issues.
This requires `issues: write` permissions in order to work correctly.

## Inputs

| Name | Description | Default |
|------|-------------|---------|
| `labels` (*) | A list of labels to add, separated by newlines. | _N/A_ |
| `issue-number` | The issue number to comment on | `"0"` |
| `owner` | The repository owner | `""` |
| `repo` | The repository | `""` |
| `retries` | The number of times to try retrying | `"0"` |
| `retry-exempt-status-codes` | The retry exempt status codes | `"400,401,403,404,422"` |

**Note:** _(*) marks required inputs_

## Outputs

`issues/set-labels` does not have any outputs at this time

## Example

Here is a very basic example of how to use the `issues/set-labels` composite action
in a project (placeholders are used in place of real inputs):

```yaml
run:
  example-job:
    # ... 
    steps:
      # ... 
      - name: Sets labels on an issue
        uses: bitwizeshift/actions-github/issues/set-labels@v1
        with:
          # Required inputs
          labels: LABELS

          # Optional inputs
          issue-number: ISSUE_NUMBER
          owner: OWNER
          repo: REPO
          retries: RETRIES
          retry-exempt-status-codes: RETRY_EXEMPT_STATUS_CODES
```