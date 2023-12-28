# `actions-github`

This repository provides easy-to-use [composite actions] for managing a Github
repository in [Github workflows]. All actions wrap the [octokit api] via
[`actions/github-script`][github-script].

## Available Actions

Below are the list of available actions, with links to documentation:

* [`git/add`](docs/git-add.md)
* [`git/commit`](docs/git-commit.md)
* [`git/push`](docs/git-push.md)
* [`issues/add-assignees`](docs/issues-add-assignees.md)
* [`issues/add-labels`](docs/issues-add-labels.md)
* [`issues/close`](docs/issues-close.md)
* [`issues/create`](docs/issues-create.md)
* [`issues/create-comment`](docs/issues-create-comment.md)
* [`issues/create-or-comment`](docs/issues-create-or-comment.md)
* [`issues/delete-comment`](docs/issues-delete-comment.md)
* [`issues/get`](docs/issues-get.md)
* [`issues/lock`](docs/issues-lock.md)
* [`issues/remove-assignee`](docs/issues-remove-assignee.md)
* [`issues/remove-label`](docs/issues-remove-label.md)
* [`issues/set-labels`](docs/issues-set-labels.md)
* [`issues/unlock`](docs/issues-unlock.md)
* [`issues/update`](docs/issues-update.md)
* [`issues/update-comment`](docs/issues-update-comment.md)
* [`pulls/add-assignees`](docs/pulls-add-assignees.md)
* [`pulls/add-labels`](docs/pulls-add-labels.md)
* [`pulls/close`](docs/pulls-close.md)
* [`pulls/create-comment`](docs/pulls-create-comment.md)
* [`pulls/get`](docs/pulls-get.md)
* [`releases/create`](docs/releases-create.md)
* [`releases/delete`](docs/releases-delete.md)
* [`releases/delete-asset`](docs/releases-delete-asset.md)
* [`releases/upload-asset`](docs/releases-upload-asset.md)

## License

Except where otherwise specified, this project is dual-licensed under both the
[Apache-2] and [MIT] licenses.

[Apache-2]: https://opensource.org/license/apache-2-0/
[MIT]: http://opensource.org/licenses/MIT/
[composite actions]: https://docs.github.com/en/actions/creating-actions/creating-a-composite-action
[octokit api]: https://octokit.github.io/rest.js/v20
[Github workflows]: https://docs.github.com/en/actions/using-workflows
[github-script]: https://github.com/actions/github-script
