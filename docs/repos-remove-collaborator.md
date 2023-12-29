# Remova repository collaborator

<!-- These docs are generated by a tool -->

A composite action that removes a collaborator from the repository.
Requires the `contents: write` permission to work.

## Inputs

| Name | Description | Default |
|------|-------------|---------|
| `username` (*) | The handle for the GitHub user account. | _N/A_ |
| `github-token` | The default token to use for this Git operation. If unspecified, this will default to `github.token`.  | `"${{ github.token }}"` |
| `owner` | The repository owner. If unspecified, this will default to the owner of the current repository.  | `""` |
| `repo` | The name of the repository. If unspecified, this will default to the current repository.  | `""` |
| `retries` | The number of times to attempt to retry if this fails.  | `"0"` |
| `retry-exempt-status-codes` | A list of error-codes that are exempt from being retried.  | `"400,401,403,404,422"` |

**Note:** _(*) marks required inputs_

## Outputs

`repos/remove-collaborator` does not have any outputs at this time

## Example

Here is a very basic example of how to use the `repos/remove-collaborator` composite action
in a project (placeholders are used in place of real inputs):

```yaml
run:
  example-job:
    # ... 
    steps:
      # ... 
      - name: Remova repository collaborator
        uses: bitwizeshift/actions-github/repos/remove-collaborator@v1
        with:
          # Required inputs
          username: USERNAME

          # Optional inputs
          github-token: GITHUB_TOKEN
          owner: OWNER
          repo: REPO
          retries: RETRIES
          retry-exempt-status-codes: RETRY_EXEMPT_STATUS_CODES
```