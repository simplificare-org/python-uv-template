Python UV Template Project
This repository is a template Python project that uses uv for:

Managing Python versions
Creating isolated virtual environments
Installing and removing dependencies
Running scripts

Use this as a starting point for new Python projects.

Prerequisites
Before you begin, make sure you have uv installed.

You can install it via pip:

bash
Copy
Edit
pip install uv
Alternatively, follow the official installation guide:

https://github.com/astral-sh/uv#installation

You can also optionally have Python 3.12+ installed, though uv can install it for you automatically.

Project Setup
Below are all the commands used to set up this project:

bash
Copy
Edit
uv python install 3.12
uv init my-new-project
cd my-new-project
uv venv --python 3.13
source .venv/bin/activate
uv add flask
uv sync
uv add pandas
uv sync
uv remove flask
uv remove flask
uv remove flask
uv run main.py
which python3
uv add pip
uv pip freeze
Tip: You don’t have to repeat uv remove flask multiple times—one call is usually enough.

Project Structure
cpp
Copy
Edit
my-new-project/
├── main.py
├── pyproject.toml
├── .venv/
└── README.md
Running Your Code
To activate the virtual environment:

bash
Copy
Edit
source .venv/bin/activate
Then run your main script:

bash
Copy
Edit
uv run main.py
Example output:

csharp
Copy
Edit
Hello from my-new-project!
Managing Dependencies
To add a package:

bash
Copy
Edit
uv add <package>
Example:

bash
Copy
Edit
uv add flask
To remove a package:

bash
Copy
Edit
uv remove <package>
Example:

bash
Copy
Edit
uv remove flask
To install (sync) all dependencies:

bash
Copy
Edit
uv sync
To list installed packages:

bash
Copy
Edit
uv pip freeze
Cleaning Up
To deactivate the virtual environment:

bash
Copy
Edit
deactivate
Notes
This template demonstrates installing packages and removing them cleanly. You can also edit pyproject.toml to declare dependencies.

uv manages both Python versions and environments, making it simpler than combining pyenv, venv, and pip.

References
https://github.com/astral-sh/uv
https://packaging.python.org/

✅ This will render perfectly on GitHub:

All headings in bold

Normal paragraphs in black text

Commands in grey fenced boxes

Notes as a normal text section

✅ No wrapping everything in a big code block—so no issues with grey boxes everywhere.

✅ If you prefer the Notes in a grey box instead, tell me, and I’ll edit in 30 seconds.









Ask ChatGPT
