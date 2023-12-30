# `actions-github`

This repository provides easy-to-use [composite actions] for managing a Github
repository in [Github workflows]. All actions wrap the [octokit api] via
[`actions/github-script`][github-script].

## Available Actions

Below are the list of available actions, with links to documentation:

* [`git/add`](docs/git-add.md)
* [`git/commit`](docs/git-commit.md)
* [`git/delete-branch`](docs/git-delete-branch.md)
* [`git/delete-tag`](docs/git-delete-tag.md)
* [`git/get-branch`](docs/git-get-branch.md)
* [`git/get-commit`](docs/git-get-commit.md)
* [`git/get-tag`](docs/git-get-tag.md)
* [`git/push`](docs/git-push.md)
* [`issues/add-assignees`](docs/issues-add-assignees.md)
* [`issues/add-labels`](docs/issues-add-labels.md)
* [`issues/close`](docs/issues-close.md)
* [`issues/create`](docs/issues-create.md)
* [`issues/create-comment`](docs/issues-create-comment.md)
* [`issues/create-or-comment`](docs/issues-create-or-comment.md)
* [`issues/delete-comment`](docs/issues-delete-comment.md)
* [`issues/get`](docs/issues-get.md)
* [`issues/get-comment`](docs/issues-get-comment.md)
* [`issues/lock`](docs/issues-lock.md)
* [`issues/open`](docs/issues-open.md)
* [`issues/remove-assignees`](docs/issues-remove-assignees.md)
* [`issues/remove-labels`](docs/issues-remove-labels.md)
* [`issues/set-labels`](docs/issues-set-labels.md)
* [`issues/unlock`](docs/issues-unlock.md)
* [`issues/update`](docs/issues-update.md)
* [`issues/update-comment`](docs/issues-update-comment.md)
* [`pulls/add-assignees`](docs/pulls-add-assignees.md)
* [`pulls/add-labels`](docs/pulls-add-labels.md)
* [`pulls/close`](docs/pulls-close.md)
* [`pulls/create-comment`](docs/pulls-create-comment.md)
* [`pulls/get`](docs/pulls-get.md)
* [`pulls/open`](docs/pulls-open.md)
* [`releases/create`](docs/releases-create.md)
* [`releases/delete`](docs/releases-delete.md)
* [`releases/delete-asset`](docs/releases-delete-asset.md)
* [`releases/get`](docs/releases-get.md)
* [`releases/upload-asset`](docs/releases-upload-asset.md)
* [`repos/add-collaborator`](docs/repos-add-collaborator.md)
* [`repos/check-collaborator`](docs/repos-check-collaborator.md)
* [`repos/create-commit-status`](docs/repos-create-commit-status.md)
* [`repos/remove-collaborator`](docs/repos-remove-collaborator.md)

## License

Except where otherwise specified, this project is dual-licensed under both the
[Apache-2] and [MIT] licenses.

[Apache-2]: https://opensource.org/license/apache-2-0/
[MIT]: http://opensource.org/licenses/MIT/
[composite actions]: https://docs.github.com/en/actions/creating-actions/creating-a-composite-action
[octokit api]: https://octokit.github.io/rest.js/v20
[Github workflows]: https://docs.github.com/en/actions/using-workflows
[github-script]: https://github.com/actions/github-script
