# Create a git commit

<!-- These docs are generated by a tool -->

A composite action for committing the current staged content.

## Inputs

| Name | Description | Default |
|------|-------------|---------|
| `title` (*) | The title of the commit message | _N/A_ |
| `body` | The body of the commit message | `""` |
| `user-email` | The email of the user to commit as | `"octocat@users.noreply.github.com"` |
| `user-name` | The default user to commit as | `"Octocat"` |

**Note:** _(*) marks required inputs_

## Outputs

| Name | Description |
|------|-------------|
| `sha1` | The SHA1 of the newly created commit |
| `sha1-short` | The short/succinct SHA1 of the newly created commit |

## Example

Here is a very basic example of how to use the `git/commit` composite action
in a project (placeholders are used in place of real inputs):

```yaml
run:
  example-job:
    # ... 
    steps:
      # ... 
      - name: Create a git commit
        id: git-commit # only necessary if using this action's output(s)
        uses: bitwizeshift/actions-github/git/commit@v1
        with:
          # Required inputs
          title: TITLE

          # Optional inputs
          body: BODY
          user-email: USER_EMAIL
          user-name: USER_NAME
      # ... 
      - name: Uses "Create a git commit" Outputs
        uses: example-actions/use-git-commit@v3 # illustrative
        with:
          use-sha1: ${{ steps.git-commit.outputs.sha1 }}
          use-sha1-short: ${{ steps.git-commit.outputs.sha1-short }}
```