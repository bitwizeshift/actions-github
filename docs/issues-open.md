# Open issue

<!-- These docs are generated by a tool -->

A composite action for opening a previously closed issue.
This requires `issues: write` permissions in order to work correctly.

## Inputs

| Name | Description | Default |
|------|-------------|---------|
| `github-token` | The default token to use for this Git operation. If unspecified, this will default to `github.token`.  | `"${{ github.token }}"` |
| `issue-number` | The issue number to comment on | `"0"` |
| `owner` | The repository owner. If unspecified, this will default to the owner of the current repository.  | `""` |
| `repo` | The name of the repository. If unspecified, this will default to the current repository.  | `""` |
| `retries` | The number of times to attempt to retry if this fails.  | `"0"` |
| `retry-exempt-status-codes` | A list of error-codes that are exempt from being retried.  | `"400,401,403,404,422"` |

## Outputs

`issues/open` does not have any outputs at this time

## Example

Here is a very basic example of how to use the `issues/open` composite action
in a project (placeholders are used in place of real inputs):

```yaml
run:
  example-job:
    # ... 
    steps:
      # ... 
      - name: Open issue
        uses: bitwizeshift/actions-github/issues/open@v1
        with:
          # Optional inputs
          github-token: GITHUB_TOKEN
          issue-number: ISSUE_NUMBER
          owner: OWNER
          repo: REPO
          retries: RETRIES
          retry-exempt-status-codes: RETRY_EXEMPT_STATUS_CODES
```