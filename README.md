# Python Hello World CI/CD

This repository contains a Python Hello World application with a GitHub Actions CI/CD workflow.

## Application

The application is defined in `app.py` and returns:

```txt
Hello, World!
```

## Tests

Unit tests are located in the `tests/` directory and are run with `pytest`.

## CI/CD Workflow

The workflow is defined in:

```txt
.github/workflows/main.yml
```

The workflow automatically runs whenever code is pushed to the `main` branch.

It contains:

1. **Lint Python code**
   - Installs dependencies from `requirements.txt`
   - Runs `flake8 .`
   - Fails if linting issues are found

2. **Run unit tests**
   - Installs dependencies from `requirements.txt`
   - Runs `pytest`
   - Fails if any test fails

## How to verify

Go to the repository's **Actions** tab and open the latest workflow run. Both jobs should show successful completion.
