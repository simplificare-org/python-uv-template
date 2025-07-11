# Python UV Template Project

This repository is a **template Python project** that uses [uv](https://github.com/astral-sh/uv) for:

✅ Managing Python versions  
✅ Creating isolated virtual environments  
✅ Installing and removing dependencies  
✅ Running scripts  

Use this as a starting point for new Python projects.

---

## 📋 Prerequisites

Before you begin, make sure you have:

**uv** installed. You can install it via pip:

```bash
pip install uv

Alternatively, follow the official installation guide.

Optionally, have Python 3.12+ installed (though uv can install it for you automatically).

🛠️ Project Setup
Below are all the commands used to set up this project:

# Install Python 3.12
uv python install 3.12

# Initialize a new project
uv init my-new-project

# Change into the project directory
cd my-new-project

# Create a virtual environment using Python 3.13
uv venv --python 3.13

# Activate the virtual environment
source .venv/bin/activate

# Add Flask
uv add flask

# Install dependencies
uv sync

# Add Pandas
uv add pandas

# Sync again to install new dependencies
uv sync

# Remove Flask
uv remove flask

# Remove remaining dependencies
uv remove flask  # Repeated to clean up
uv remove flask  # Safe even if already removed

# Run the main script
uv run main.py

# Check the active Python interpreter
which python3

# Add pip explicitly
uv add pip

# List installed packages
uv pip freeze


✅ Tip: You don’t have to repeat uv remove flask multiple times—one call is usually enough.

📂 Project Structure

my-new-project/
├── main.py
├── pyproject.toml
├── .venv/
└── README.md

▶️ Running Your Code
To activate the virtual environment, run:

source .venv/bin/activate

Then execute your main script:

uv run main.py


Example output:

csharp
Copy
Edit
Hello from my-new-project!

🧩 Managing Dependencies
Add a package:

uv add <package>


Example:

bash
Copy
Edit
uv add flask
Remove a package:

bash
Copy
Edit
uv remove <package>
Example:

bash
Copy
Edit
uv remove flask
Install (sync) all dependencies:

bash
Copy
Edit
uv sync
List installed packages:

bash
Copy
Edit
uv pip freeze
🧹 Cleaning Up
To deactivate the virtual environment, run:

bash
Copy
Edit
deactivate
💡 Notes
This template demonstrates both installing packages and removing them cleanly. You can modify pyproject.toml to define your dependencies declaratively.

uv manages both Python versions and environments, making it simpler than combining pyenv, venv, and pip.

📚 References
uv GitHub Repository

Python Packaging Guide







