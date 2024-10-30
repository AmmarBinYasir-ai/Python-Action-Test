<h1 align="center">🧪 Python Calculator Project with GitHub Actions</h1>

<p align="center">
   <b>A CI/CD Python project with a calculator app and GitHub Actions workflow for automated testing of basic arithmetic operations.</b>
</p>

---

## Table of Contents
- [Project Architecture](#project-architecture)
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Testing Code](#testing-code)
- [Contributing](#contributing)
- [Commands](#commands)

---

## Project Architecture

<p align="center">
<img src="projectarchitectureimage.png" alt="Project Architecture">
</p>

**This project's GitHub Actions workflow** involves several key components:
- **Code Checkout**: Fetches the latest code from the GitHub repository.
- **Python Setup**: Installs a specified version of Python to ensure consistent runtime.
- **Dependency Installation**: Installs project dependencies listed in `requirements.txt`.
- **Testing**: Executes tests with `pytest` to validate functionality.

This architecture supports a seamless CI/CD pipeline, automatically verifying code quality and functionality upon each code push to `main`.

---

## Overview

This repository contains:
- A **Calculator class** that provides methods for basic arithmetic operations: addition, subtraction, multiplication, and division.
- **Unit tests** to ensure each calculator function operates correctly.
- A **GitHub Actions workflow** to automate dependency installation and testing on each code update to `main`.

---

## Prerequisites

- Ensure **Python 3.x** is installed on your local machine.
- Have a **GitHub account** and a repository set up for this project.

---

## Installation

Follow these steps to set up the project:

1. **Clone the repository** and navigate into the project folder.
2. **Create a virtual environment** and activate it.
3. **Install dependencies** from `requirements.txt`.

---

## Usage

Once installed, you can use the `Calculator` class to perform:
- **Addition**
- **Subtraction**
- **Multiplication**
- **Division** (with handling for division by zero)

The functionality of the class is validated through the unit tests included in this repository.

---

## Testing Code

Unit tests are provided in the `test_calculator.py` file to verify the functionality of each method in the `Calculator` class.  
The `test_calculator.py` file is attached in the repository for reference.

---

## Contributing

Feel free to open issues or submit pull requests for additional features, improvements, or new test cases.

---

## Commands

```bash
# Clone the repository and navigate into it
git clone https://github.com/AmmarBinYasir-ai/Python-Action-Test.git
cd Python-Action-Test

# Create a virtual environment
python3 -m venv .env
source .env/bin/activate  # For Linux/macOS
# .\.env\Scripts\activate   # For Windows

# Install dependencies
pip install -r requirements.txt

# Run tests locally
pytest

# To push code changes and trigger the GitHub Actions workflow
git add .
git commit -m "Initial commit with calculator app and CI workflow"
git push -u origin main
