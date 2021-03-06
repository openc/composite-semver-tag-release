# Composite semver tag release

[![Push](https://github.com/openc/composite-semver-tag-release/actions/workflows/push.yml/badge.svg)](https://github.com/openc/composite-semver-tag-release/actions/workflows/push.yml)

GitHub composite repository. Used to template the automated creation
of releases and tags via semver.

## Details

The composite runs via hosting a `package.json` in the root of the
repository. This is used on `push` to master along with `conventional commits`
since the last release / tag to update the the release / tag. The action
will also update the `package.json` to the new version.

The action is allowed in master due to using a PAT that is part of the `Allow
specified actors to bypass required pull requests`

## Docs

* [confluence documentation](https://opencorporates.atlassian.net/wiki/spaces/DEV/pages/41091106/GitHub+Composite+playbook+-+template+usage)
* [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
* [action: gh-action-bump-version](https://github.com/phips28/gh-action-bump-version)
