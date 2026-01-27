# invenio-subjects-mesh-common

*Common features surrounding MeSH subject terms for InvenioRDM*

<a href="https://pypi.org/project/invenio-subjects-mesh-common/">
  <img src="https://img.shields.io/pypi/v/invenio-subjects-mesh-common.svg">
</a>

This groups common MeSH features and lets downstream distribution packages (e.g., invenio-subjects-mesh-lite)
provide vocabulary fixtures with targeted filtering. This distribution package is meant to be
a dependency to those downstream distribution packages.


## Installation

```bash
pip install invenio-subjects-mesh-common
```


## Development

Install the project in editable mode with `dev` dependencies in an isolated virtualenv. We recommend using `uv`:

```bash
uv pip install -e .[dev]
# or if using pipenv
pipenv run pip install -e .[dev]
```

Run tests:

```bash
uv run invoke test
# or shorter
uv run inv test
# or if using pipenv
pipenv run inv test
```

Test compatibility with the pre-release version of InvenioRDM (invenio-app-rdm):

```bash
uv run --extra dev_pre --prerelease=allow inv test
```

Check manifest:

```bash
uv run inv check-manifest
# or if using pipenv
pipenv run inv check-manifest
```

Clean out artefacts:

```bash
uv run inv clean
# or if using pipenv
pipenv run inv clean
```
