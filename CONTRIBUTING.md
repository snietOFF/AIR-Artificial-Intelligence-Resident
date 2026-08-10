# Contributing to AIR

We welcome bug reports, feature requests, and pull requests. This document explains how you can contribute.

## Bug Reports and Feature Requests

Please submit bug reports and feature requests as GitHub issues. This helps us track and discuss potential solutions.

## Pull Requests

Small changes can be submitted directly as a PR. For larger or significant changes, please open an issue first to discuss your idea. This saves time for both you and the maintainers and helps ensure your contribution can be integrated smoothly.

## Licensing

By contributing to this project, you agree that your contributions will be licensed under the Apache License 2.0, the same license that covers the project.

## Setting up a Development Environment

### Clone the Repository

```bash
git clone https://github.com/snietOFF/AIR-Artificial-Intelligence-Resident.git
cd AIR-Artificial-Intelligence-Resident
```
Create a Virtual Environment

It is recommended to create a virtual environment outside the repository to keep your development environment isolated.
```bash

python3 -m venv /path/to/venv
```
Activate the Virtual Environment

On Linux or macOS:
```bash

source /path/to/venv/bin/activate
```
On Windows:
```bash

/path/to/venv/Scripts/activate
```
Install the Project in Editable Mode

This allows you to make changes to the source code and have them take effect immediately without reinstalling.
```bash

pip install -e .
```
Install Development Dependencies
```bash

pip install -r requirements/requirements-dev.txt
```
You may also install other optional dependencies from the requirements/ directory if needed.
Install Pre-commit Hooks (Optional)

The project uses pre-commit hooks for code formatting and linting. To set them up:
```bash

pre-commit install
```
Now you should have a fully functional development environment. You can start making changes, running tests, and contributing.
Running Tests

Run the test suite with:
```bash

pytest
```
Coding Standards
Python Compatibility

AIR supports Python 3.10 and later. Ensure your code is compatible with these versions.
Code Style

The project follows PEP 8 with a maximum line length of 100 characters. We use isort for import sorting and Black for code formatting. Installing the pre-commit hooks will automatically format your code before each commit.
No Type Hints

The project does not use type hints.
Managing Dependencies

When introducing new dependencies, add them to the appropriate requirements.in file (e.g., requirements.in for main dependencies, requirements-dev.in for development dependencies). Then run:
```bash

pip install pip-tools
./scripts/pip-compile.sh
```
You can also pass arguments, for example:
```bash

./scripts/pip-compile.sh --upgrade
```
Questions?

If you have any questions about contributing, feel free to open an issue on GitHub.
