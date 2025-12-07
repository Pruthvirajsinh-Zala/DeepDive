# DeepDive

A small, personal workspace containing exploratory code and a Jupyter Notebook (`code.ipynb`). This repository is intended for experiments, learning, and prototyping.

## Contents

- `code.ipynb` — main Jupyter Notebook (analysis / experiments).


## Goals

- Provide a lightweight, reproducible environment for running the notebook locally.
- Make it easy for collaborators to get started.

## Requirements

- Python 3.8+ (3.10 or later recommended)
- Jupyter or VS Code with the Jupyter extension
- pip (or conda) for installing dependencies


## Quick start (Windows PowerShell)

1. Clone the repository:

   git clone <repo-url>
   cd DeepDive

2. (Recommended) Create and activate a virtual environment with venv:

   python -m venv .venv
   .\.venv\Scripts\Activate.ps1

   Or with conda:

   conda create -n deepdive python=3.10
   conda activate deepdive

3. Install Jupyter and any project dependencies (if a `requirements.txt` exists):

   pip install --upgrade pip
   pip install jupyter
   pip install -r requirements.txt  # optional

4. Open the notebook in your browser:

   jupyter notebook

   Then open `code.ipynb` from the notebook UI.

   Alternatively, open this folder in VS Code and use the built-in notebook support.

## Generate dependencies from the notebook

1. Extract imports (quick method): open `code.ipynb` and look for top-level `import` statements.
2. Install the discovered packages into your environment and run `pip freeze > requirements.txt`.


## License

This project is licensed under the MIT License — see the included `LICENSE` file for the full text.

If you prefer a different license (Apache-2.0, GPL-3.0, etc.), tell me and I will replace the `LICENSE` file.


## Environment & secrets

- The notebook contains a placeholder `GEMINI_API_KEY = "YOUR_API_KEY_HERE"`. Instead of committing keys, set an environment variable in PowerShell while testing:

```powershell
$env:GEMINI_API_KEY = "your_api_key_here"
```

Or paste your key into the notebook for quick local testing (do not commit).

---
