# Test for [jupyter-book/jupyter-book#1501](https://github.com/jupyter-book/jupyter-book/issues/1501)

This repo tests whether [jupyter-book/jupyter-book#1501](https://github.com/jupyter-book/jupyter-book/issues/1501) is caused by an upstream bug.

## How to run?

Easiest to work with [`uv`](https://docs.astral.sh/uv/). There are two ways ('tests') to build the documentation.

### `jupyter-book`

```shell
uv venv
source .venv/bin/activate
uv pip install jupyter-book pandas
jb build docs
```

### `sphinx-build`

```shell
uv venv
source .venv/bin/activate
uv pip install myst-nb pandas
sphinx-build docs docs/_build/html
```
