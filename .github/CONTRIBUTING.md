# Contributing to Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio

Thank you for considering contributing to the `Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio` repository! We welcome contributions from the community to enhance this resource for advanced machine learning and deep learning education.

## Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct (v2.1). By participating, you are expected to uphold this code. Please report unacceptable behavior to `chirag.iyer.dev@gmail.com`.

## How Can I Contribute?

### 1. Reporting Bugs

If you find a bug, please check if it has already been reported. If not, please create a new issue on GitHub. Provide a clear and concise description of the bug, including:

*   The specific course module or example.
*   Steps to reproduce the bug.
*   Expected behavior vs. actual behavior.
*   Any relevant error messages or traceback.
*   Your Python version and package versions (e.g., PyTorch, TensorFlow).

### 2. Suggesting Enhancements

We are always looking for ways to improve the portfolio. If you have an idea for a new example, a better explanation, or a way to optimize existing code, please open an issue to discuss it. Include:

*   The specific area you want to enhance.
*   Your proposed solution or new feature.
*   The benefits of your suggestion.

### 3. Contributing Code

We encourage pull requests for bug fixes and new features. Please follow these steps:

1.  **Fork the Repository:** Create your own fork of `https://github.com/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio`.
2.  **Clone Your Fork:** `git clone git@github.com:chirag127/<your-username>/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio.git`
3.  **Create a New Branch:** Create a descriptive branch for your changes (e.g., `feature/add-gan-example`, `fix/pytorch-gradient-issue`).
    bash
    git checkout -b your-branch-name
    
4.  **Make Your Changes:** Implement your bug fixes or new features. Ensure your code adheres to the project's coding standards (see below).
5.  **Test Your Changes:** Run the provided tests to ensure your changes haven't introduced regressions.
    bash
    # Install development dependencies
    uv pip install -r requirements-dev.txt
    # Run tests
    pytest
    
6.  **Commit Your Changes:** Use conventional commits for your messages.
    bash
    git commit -m "feat: Add advanced Transformer architecture example"
    # or for a fix
    git commit -m "fix: Resolve NaN loss in RL agent training"
    
7.  **Push to Your Fork:** Push your branch to your fork.
    bash
    git push origin your-branch-name
    
8.  **Open a Pull Request:** Create a pull request against the `main` branch of the original repository (`chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio`). Describe your changes clearly.

#### Coding Standards & Best Practices:

*   **Python Version:** Code should be compatible with **Python 3.10+**.
*   **Dependencies:** Use `uv` for managing dependencies. New dependencies should be added to `pyproject.toml` and installed using `uv sync`.
*   **Linting & Formatting:** Use **Ruff** for linting and formatting. Ensure your code passes Ruff checks before submitting a PR.
    bash
    ruff check .
    ruff format .
    
*   **Testing:** All new code should be accompanied by relevant unit or integration tests using **Pytest**. Aim for comprehensive test coverage.
    bash
    pytest
    
*   **Modularity:** Follow principles of modular design. Aim for reusable components and clear function/class responsibilities.
*   **Documentation:** Add clear docstrings to all public functions, classes, and methods. Update relevant README sections if necessary.

### 4. Improving Documentation

Clear documentation is crucial. If you find typos, unclear explanations, or missing information in the README or other documentation files, please submit a pull request.

## Development Environment Setup

To set up your development environment:

1.  **Clone the repository:**
    bash
    git clone git@github.com:chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio.git
    cd Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio
    
2.  **Install `uv`:** If you don't have `uv` installed, follow the instructions at [https://github.com/astral-sh/uv](https://github.com/astral-sh/uv).
3.  **Install project dependencies (including dev tools):**
    bash
    uv sync requirements.txt requirements-dev.txt
    
    *(Note: This assumes you have `requirements.txt` for runtime and `requirements-dev.txt` for development tools like pytest and ruff. If using `pyproject.toml`, adjust commands accordingly)*

## Project Structure Overview


Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio/
├── notebooks/             # Jupyter notebooks for exploration and demos
├── src/                   # Source code for modules and examples
│   ├── nlp/               # Natural Language Processing modules
│   ├── reinforcement_learning/ # Reinforcement Learning modules
│   ├── time_series/       # Time Series analysis modules
│   ├── common/            # Common utilities and base classes
│   └── __init__.py
├── tests/                 # Pytest test suites
│   ├── test_nlp.py
│   ├── test_reinforcement_learning.py
│   └── ...
├── pyproject.toml         # Project metadata, build system, and tool configurations (uv, ruff, pytest)
├── README.md              # Project overview, setup, and usage instructions
├── LICENSE                # Project license file
└── .gitignore             # Git ignore patterns


## Questions?

If you have any questions about contributing, please open an issue.

We look forward to your contributions!