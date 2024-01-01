# project [![skeleton](https://img.shields.io/badge/bf2dfcf-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/bf2dfcf)
[![Package version](https://img.shields.io/pypi/v/project?label=PyPI)](https://pypi.org/project/project/)
[![Supported Python versions](https://img.shields.io/pypi/pyversions/project.svg?logo=python&label=Python)](https://pypi.org/project/project/)

[![Tests](https://github.com/bswck/project/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/project/actions/workflows/test.yml)
[![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/project.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/project)
[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
[![License](https://img.shields.io/github/license/bswck/project.svg?label=License)](https://github.com/bswck/project/blob/HEAD/LICENSE)
[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)

Automatically detect backends & initialize virtual environments for your Python repo clones.

> [!Warning]
> This project is currently in the **Work in Progress** state.
>
> Hit the `👁 Watch` button to know when it's ready to be tried out!

# Idea
- `project clone [URL]` → clone and install a Python project
- `project install` → install a Python project
- `project env` → display info on the installed environment
- `project config [OPTION] [del|set [VAL]]` → configure `pyproject.toml`
- `project test` → run the detected test suite
- `project lint` → run the detected linting suite
- `project audit` → `project lint; project test`

# Installation



You might simply install it with pip:

```shell
pip install project
```

If you use [Poetry](https://python-poetry.org/), then run:

```shell
poetry add project
```

## For contributors

<!--
This section was generated from bswck/skeleton@bf2dfcf.
Instead of changing this particular file, you might want to alter the template:
https://github.com/bswck/skeleton/tree/bf2dfcf/project/README.md.jinja
-->

> [!Note]
> If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).



1.  Fork the [project repository](https://github.com/bswck/project) on GitHub.

1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
    Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
    You might use [pipx](https://github.com/pypa/pipx#readme) to install it globally (recommended):

    ```shell
    pipx install poetry
    ```

    <sub>If you encounter any problems, refer to [the official documentation](https://python-poetry.org/docs/#installation) for the most up-to-date installation instructions.</sub>

    Be sure to have Python 3.8 installed—if you use [pyenv](https://github.com/pyenv/pyenv#readme), simply run:

    ```shell
    pyenv install 3.8
    ```

1.  Clone your fork locally and install dependencies.

    ```shell
    git clone https://github.com/your-username/project path/to/project
    cd path/to/project
    poetry env use $(cat .python-version)
    poetry install
    ```

    Next up, simply activate the virtual environment and install pre-commit hooks:

    ```shell
    poetry shell
    pre-commit install --hook-type pre-commit --hook-type pre-push
    ```

For more information on how to contribute, check out [CONTRIBUTING.md](https://github.com/bswck/project/blob/HEAD/CONTRIBUTING.md).<br/>
Always happy to accept contributions! ❤️


# Legal info
© Copyright by Bartosz Sławecki ([@bswck](https://github.com/bswck)).
<br />This software is licensed under the terms of [MIT License](https://github.com/bswck/project/blob/HEAD/LICENSE).
