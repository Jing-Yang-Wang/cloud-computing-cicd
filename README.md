# cloud-computing-cicd
CI/CD Pipeline Assignment Part 1

# Cloud Computing CI/CD Pipeline (Part 1)

## Project Description

This project demonstrates a Continuous Integration (CI) pipeline using GitHub Actions.

It contains a simple Python calculator, automated unit tests using pytest, and a GitHub Actions workflow that runs tests whenever code is pushed or a pull request is created.

## Project Files

- `calculator.py` — Python calculator with basic arithmetic operations.
- `test_calculator.py` — Automated unit tests.
- `requirements.txt` — Python dependencies.
- `.github/workflows/ci.yml` — GitHub Actions CI workflow.
- `.gitignore` — Files and directories excluded from Git tracking.

## Requirements

- Python 3.11 or compatible version
- pip

## Installation

Clone the repository and navigate into the project directory.

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

## Running Tests

Run the automated tests using:

```bash
python -m pytest -v
```

The project includes five tests covering addition, subtraction, multiplication, division, and division by zero.

## GitHub Actions CI Pipeline

The GitHub Actions workflow automatically runs when:

- Code is pushed to the repository.
- A pull request is opened or updated.

The workflow can also be started manually using the **Run workflow** button under the GitHub Actions tab.

The pipeline:

1. Checks out the repository.
2. Sets up Python 3.11.
3. Installs the required dependencies.
4. Runs the automated tests using pytest.

A successful workflow indicates that all automated tests passed.

## Purpose

The purpose of this assignment is to understand how Continuous Integration helps software teams detect problems early through automated testing.