<div align="center">

  <img src="https://github.com/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio/blob/main/.github/assets/repo-banner.png?raw=true" alt="Repository Banner" style="width:100%; max-width:900px;"/>

  <h1>Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio</h1>

  <p>Official hands-on Python code portfolio for advanced machine learning and deep learning courses. Features examples in NLP, Reinforcement Learning, Time Series, PyTorch, and TensorFlow. A comprehensive resource hub for practical AI development.</p>

  <p>
    <a href="https://github.com/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio/actions/workflows/ci.yml"><img src="https://github.com/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio/actions/workflows/ci.yml/badge.svg" alt="Build Status" style="max-width: 100%;"></a>
    <a href="https://codecov.io/gh/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio"><img src="https://codecov.io/gh/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio/branch/main/graph/badge.svg?token=YOUR_CODECOV_TOKEN" alt="Code Coverage" style="max-width: 100%;"></a>
    <img src="https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python&logoColor=white" alt="Python Version" style="max-width: 100%;">
    <img src="https://img.shields.io/badge/PyTorch-2.x-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" style="max-width: 100%;">
    <img src="https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow" style="max-width: 100%;">
    <img src="https://img.shields.io/badge/Lint%2FFormat-Ruff-black?style=flat-square&logo=ruff&logoColor=white" alt="Lint/Format" style="max-width: 100%;">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square" alt="License" style="max-width: 100%;">
    <img src="https://img.shields.io/github/stars/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio?style=flat-square&color=FEDC01&logo=github" alt="GitHub Stars" style="max-width: 100%;">
  </p>

  <p align="center">
    <a href="https://github.com/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio/stargazers">
      <img src="https://img.shields.io/badge/Star%20⭐%20this%20Repo-brightgreen?style=for-the-badge&logo=github" alt="Star this repo">
    </a>
  </p>
</div>

<p align="center">
  A comprehensive hands-on Python code portfolio demonstrating advanced deep learning concepts and implementations across various domains like Natural Language Processing (NLP), Reinforcement Learning, and Time Series Analysis. This repository serves as a practical educational resource and a robust foundation for building AI applications.
</p>

---

## 🚀 Project Overview

This repository is meticulously curated to provide practical, runnable examples of cutting-edge deep learning techniques using PyTorch and TensorFlow. It's designed for students, researchers, and developers looking to deepen their understanding and application of deep learning fundamentals and advanced topics. Each module is self-contained, focusing on a specific domain or technique, and includes clear explanations, datasets (or instructions to acquire them), and model implementations.

## 🧠 Architecture

This project adopts a **Modular Monolith** architecture, organized by deep learning domains. Each domain acts as an independent module with its own models, data handling, and utility functions, promoting clarity, maintainability, and scalability. The `src/common` directory houses shared utilities.


Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   ├── CONTRIBUTING.md
│   ├── ISSUE_TEMPLATE/
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── SECURITY.md
├── src/
│   ├── common/
│   │   ├── data_loaders.py
│   │   └── utils.py
│   ├── nlp/
│   │   ├── attention_models/
│   │   ├── transformers/
│   │   └── ...
│   ├── reinforcement_learning/
│   │   ├── dqn_agents/
│   │   ├── policy_gradient/
│   │   └── ...
│   ├── time_series_analysis/
│   │   ├── lstm_models/
│   │   ├── transformers/
│   │   └── ...
│   └── computer_vision/
│       ├── cnns/
│       ├── gans/
│       └── ...
├── notebooks/
│   ├── nlp_intro.ipynb
│   ├── rl_basics.ipynb
│   └── ...
├── data/
│   ├── small_datasets/
│   └── README.md (Instructions for larger datasets)
├── models/
│   └── README.md (Placeholder for pre-trained models)
├── tests/
│   ├── nlp/
│   ├── reinforcement_learning/
│   └── time_series_analysis/
├── .gitignore
├── pyproject.toml
├── README.md
├── PROPOSED_README.md
├── AGENTS.md
├── badges.yml
└── LICENSE


## 📝 Table of Contents

- [🚀 Project Overview](#--project-overview)
- [🧠 Architecture](#-architecture)
- [📝 Table of Contents](#-table-of-contents)
- [⚙️ Setup and Installation](#%EF%B8%8F-setup-and-installation)
- [💡 Usage Examples](#-usage-examples)
- [🛠️ Development Standards](#%EF%B8%8F-development-standards)
- [🤝 Contributing](#-contributing)
- [🛡️ Security](#%EF%B8%8F-security)
- [📜 License](#-license)
- [🤖 AI Agent Directives](#-ai-agent-directives)

## ⚙️ Setup and Installation

To get this project up and running locally, follow these steps:

1.  **Clone the repository:**

    bash
    git clone https://github.com/chirag127/Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio.git
    cd Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio
    

2.  **Install `uv` (if you don't have it):**

    `uv` is a blazing-fast Python package installer and resolver, replacing `pip` and `pip-tools`.

    bash
    curl -LsSf https://astral.sh/uv/install.sh | sh
    # Or, if you have pipx:
    # pipx install uv
    

3.  **Create a virtual environment and install dependencies:**

    bash
    uv venv
    source .venv/bin/activate
    uv sync
    

4.  **Install Jupyter Kernel (optional, for notebooks):**

    bash
    pip install ipykernel
    python -m ipykernel install --user --name=deep-learning-foundations --display-name "Python (Deep Learning Foundations)"
    

## 💡 Usage Examples

Each module (`src/nlp`, `src/reinforcement_learning`, etc.) contains its own set of examples and instructions. Refer to the `README.md` files within each domain directory and the Jupyter notebooks in the `notebooks/` directory for detailed usage.

**Example: Running an NLP sentiment analysis model**

bash
# Assuming you are in the project root and have activated the virtual environment
python src/nlp/sentiment_analysis/train_model.py
python src/nlp/sentiment_analysis/predict.py --text "This movie was fantastic!"


## 🛠️ Development Standards

This project adheres to stringent development standards to ensure code quality, maintainability, and collaboration.

### Scripts

Run the following commands using `uv run`:

| Command           | Description                                       |
| :---------------- | :------------------------------------------------ |
| `uv run lint`     | Runs Ruff to check and format code automatically. |
| `uv run test`     | Executes all unit and integration tests with Pytest. |
| `uv run coverage` | Runs tests and generates a code coverage report.  |
| `uv run start-nlp`| Example: Runs the NLP example. (Adjust as needed) |

### Principles

-   **SOLID:** Adherence to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion Principles.
-   **DRY (Don't Repeat Yourself):** Reusable code components and abstractions are prioritized.
-   **YAGNI (You Aren't Gonna Need It):** Features are implemented only when necessary, avoiding over-engineering.

## 🤝 Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](.github/CONTRIBUTING.md) for guidelines on how to submit pull requests, report bugs, and suggest features.

## 🛡️ Security

We take security seriously. Please report any vulnerabilities following the guidelines in [SECURITY.md](.github/SECURITY.md).

## 📜 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](LICENSE) License.

---

<details>
<summary><b>🤖 AI Agent Directives (CRITICAL)</b></summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `Deep-Learning-Foundations-Hands-On-Python-Code-Portfolio`, is a Python-based Deep Learning and Machine Learning educational code portfolio.

*   **PRIMARY SCENARIO: DATA / AI / SCRIPTS (Python)**
    *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing).
    *   **Core Libraries:** Predominantly uses **PyTorch 2.x** and **TensorFlow 2.x** for neural network implementations, alongside `scikit-learn`, `numpy`, `pandas`, and `matplotlib` for data manipulation, traditional ML, and visualization.
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for distinct deep learning domains (e.g., `nlp`, `reinforcement_learning`, `time_series_analysis`, `computer_vision`). Each domain module should be self-contained with its data, models, and utility functions.
    *   **Code Quality:** Emphasize clean, well-documented, and reproducible code. All examples should be runnable and clearly explain the underlying deep learning concepts.

*   **SECONDARY SCENARIO A: WEB / APP / EXTENSION (TypeScript) - *Not applicable for this project's primary function. Reference only for potential future web-based extensions.***
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
    *   **State:** Signals (Standardized).
    *   **Lint/Test:** Biome (Speed) + Vitest (Unit) + Playwright (E2E).
    *   **Architecture:** Feature-Sliced Design (FSD).

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go) - *Not applicable for this project's primary function. Reference only for potential future performance-critical components.***
    *   **Stack:** Rust (Cargo) or Go (Modules).
    *   **Lint:** Clippy / GolangCI-Lint.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters).

---

## 4. ARCHITECTURAL & DEVELOPMENT PRINCIPLES
*   **SOLID Principles:** Ensure all code adheres to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **DRY (Don't Repeat Yourself):** Abstract common functionalities into reusable modules.
*   **YAGNI (You Aren't Gonna Need It):** Focus on current requirements, avoid over-engineering.
*   **Modularity:** Break down complex problems into smaller, manageable, and independently testable units.
*   **Reproducibility:** All deep learning examples should be easily runnable, with clear instructions for environment setup and dataset acquisition (if applicable).
*   **Documentation:** Comprehensive inline comments, docstrings, and README sections are paramount. Explain complex algorithms and model choices thoroughly.

---

## 5. VERIFICATION & DEPLOYMENT STRATEGIES
*   **Unit & Integration Testing:**
    *   All core logic and model components **MUST** have robust `pytest` coverage. Aim for 90%+ coverage.
    *   Use `pytest-cov` for coverage reports.
*   **Continuous Integration (CI):**
    *   GitHub Actions workflow (`.github/workflows/ci.yml`) to automatically run linting (`ruff format --check`, `ruff check`), testing (`uv run test`), and coverage reporting on every push and pull request.
*   **Environment Management:**
    *   Utilize `uv` for lockfile generation (`uv lock`) and dependency synchronization (`uv sync`) to ensure consistent environments.
*   **Security Best Practices:**
    *   Regularly update dependencies.
    *   Sanitize all inputs where user interaction or external data sources are involved.
    *   Adhere to best practices for handling sensitive data (though this repo is primarily educational, generalize this principle).

---

## 6. PROJECT STRUCTURE & NAMING CONVENTIONS
*   **Root Directory:** Clean and minimal.
*   **`src/`:** Contains all Python source code.
    *   `src/common/`: Shared utilities, base classes, data loaders.
    *   `src/nlp/`: Natural Language Processing examples.
    *   `src/reinforcement_learning/`: Reinforcement Learning examples.
    *   `src/time_series_analysis/`: Time Series Analysis examples.
    *   `src/computer_vision/`: (If applicable) Computer Vision examples.
*   **`notebooks/`:** Jupyter notebooks for exploration and detailed step-by-step guides.
*   **`data/`:** Placeholder for small datasets or scripts to download larger datasets.
*   **`models/`:** Placeholder for pre-trained models or saved model checkpoints.
*   **`tests/`:** Unit and integration tests, mirroring the `src/` structure.
*   **Naming:**
    *   Modules: `snake_case`.
    *   Classes: `CamelCase`.
    *   Functions/Variables: `snake_case`.

---

## 7. DOCUMENTATION GENERATION
*   Utilize `Sphinx` or similar for comprehensive API documentation if the project evolves into a library.
*   Markdown for general documentation (README, CONTRIBUTING, etc.).
</details>