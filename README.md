# Simplon Projet 1 – Python Toolbox

![CI Status](https://github.com/nicolastchenio/simplon_projet1_mlop/actions/workflows/ci.yml/badge.svg)
![Coverage](https://raw.githubusercontent.com/nicolastchenio/simplon_projet1_toolbox/main/coverage.svg)
![Python](https://img.shields.io/badge/python-3.11-blue)
![Lint](https://img.shields.io/badge/lint-ruff-purple)
![License](https://img.shields.io/badge/license-MIT-green)


## Overview

**Python Toolbox** is a small modular Python project designed to demonstrate good software engineering practices:

- modular Python architecture
- unit testing with Pytest
- code coverage measurement with pytest-cov
- static code analysis with Ruff
- dependency management with uv
- CI/CD integration

The application reads a CSV file describing mathematical operations and executes them using a dedicated business logic module.

This repository is structured to follow professional Python project standards used in modern data and MLOps environments.

---

## Project Structure

```plaintext
.
├── .github/                    
│   ├── workflows/
│   │   └── ci.yml
│   └── CODE_OF_CONDUCT.md
│   └── CONTRIBUTING.md          
├── app/                    
│   ├── modules/           
│   │   ├── __init__.py
│   │   └── mon_module.py
│   ├── main.py            
│   └── moncsv.csv
│   └── __init__.py        
├── tests/                 
│   └── test_main.py
│   └── test_math_csv.py   
├── docs/                      
├── pyproject.toml         
├── uv.lock                    
├── README.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
└── LICENSE

```


---

## Installation

This project uses **uv** for dependency management and environment synchronization.

### 1. Install uv

```
pip install uv
```

### 2. Clone the repository
```
git clone https://github.com/USER/REPO.git

cd REPO
```

### 3. Install dependencies
```
uv sync
```

This command will:

- create the virtual environment
- install all dependencies defined in `pyproject.toml`
- synchronize the environment with the project configuration

---

## Running the Application
```
uv run python -m app.main
```
---

## Running Tests

Execute the test suite with:
```
uv run pytest
```

To run tests with coverage:

```
uv run pytest --cov=app --cov-report=term-missing
```

## Code Quality

This project uses **Ruff** for linting and code quality checks.

Run linting with

```
uv run ruff check .
```


---

## Continuous Integration

The project integrates a CI pipeline that automatically:

- runs tests
- checks code coverage
- performs linting

The CI status badge at the top of this README reflects the latest build status.

---

## Contributing

Contributions are welcome.

Please read the contributing guidelines before submitting a pull request:

See **CONTRIBUTING.md**

---

## Code of Conduct

All contributors must follow the project code of conduct.

See **CODE_OF_CONDUCT.md**

---

## Contributors

Project developed by:

- nicolas tchenio

---

## License

This project is licensed under the **MIT License**.

See the **LICENSE** file for details.