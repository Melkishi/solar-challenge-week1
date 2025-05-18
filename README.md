
# Solar Challenge Week 1 - Environment Setup

This repository contains the initial setup for the Solar Challenge Week 1 project. Below are instructions to reproduce the development environment.

## Prerequisites
- Git
- Python 3.8+
- GitHub account

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/melkishi/solar-challenge-week1.git
cd solar-challenge-week1
```

### 2. Create and Activate Virtual Environment

#### Using venv:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

#### Using conda:
```bash
conda create -n solar-challenge python=3.8
conda activate solar-challenge
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Development Workflow
1. Make changes in your branch
2. Commit changes with descriptive messages
3. Push to GitHub
4. Create a Pull Request to merge into main

## Project Structure
```
├── .vscode/                # VS Code settings
├── .github/workflows/       # CI/CD workflows
├── src/                    # Source code
├── notebooks/              # Jupyter notebooks
├── tests/                  # Test files
├── scripts/                # Utility scripts
├── .gitignore              # Files to ignore
├── requirements.txt        # Dependencies
└── README.md               # Project documentation
```

## CI/CD Pipeline
The GitHub Actions workflow will automatically:
1. Run `pip install -r requirements.txt` on push
2. Verify Python version compatibility