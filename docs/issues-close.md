# Close issue

<!-- These docs are generated by a tool -->

A composite action for closing an issue.
This requires `issues: write` permissions in order to work correctly.

## Inputs

| Name | Description | Default |
|------|-------------|---------|
| `issue-number` | The issue number to comment on | `"0"` |
| `owner` | The repository owner | `""` |
| `repo` | The repository | `""` |
| `retries` | The number of times to try retrying | `"0"` |
| `retry-exempt-status-codes` | The retry exempt status codes | `"400,401,403,404,422"` |
| `state_reason` | The reason for the state-change | `"completed"` |

## Outputs

`issues/close` does not have any outputs at this time

## Example

Here is a very basic example of how to use the `issues/close` composite action
in a project (placeholders are used in place of real inputs):

```yaml
run:
  example-job:
    # ... 
    steps:
      # ... 
      - name: Close issue
        uses: bitwizeshift/actions-github/issues/close@v1
        with:
          # Optional inputs
          issue-number: ISSUE_NUMBER
          owner: OWNER
          repo: REPO
          retries: RETRIES
          retry-exempt-status-codes: RETRY_EXEMPT_STATUS_CODES
          state_reason: STATE_REASON
```