# Demo 2
Testing to make repository locally and remotely.

# New Branch added
Added a new branch addition.


# My Sample Repo - GitHub Actions Demo

This repo demonstrates a minimal Python project with GitHub Actions CI.

## What the workflow does
- Runs on `push` and `pull_request` to `main`.
- Installs dependencies from `requirements.txt`.
- Runs `flake8` linting.
- Runs `pytest` and uploads a junit XML report.

## Run locally
Create a virtual environment and run tests:
```bash
python -m venv .venv
source .venv/bin/activate         # on Windows: .venv\Scripts\activate
pip install -r requirements.txt
pytest
