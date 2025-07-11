# 🐍 Python UV Template Project

This repository is a **template Python project** that uses [uv](https://github.com/astral-sh/uv) for:

✅ Managing Python versions  
✅ Creating isolated virtual environments  
✅ Installing and removing dependencies  
✅ Running scripts  

Use this as a starting point for new Python projects.

---

## 📋 Prerequisites

Before you begin, make sure you have **uv** installed.

You can install it via pip:

```bash
pip install uv
```
Alternatively, follow the official installation guide:
https://github.com/astral-sh/uv#installation

You can also optionally have Python 3.12+ installed, though uv can install it for you automatically.

---

## 🛠️ Project Setup

Below are all the commands used to set up this project:


```bash
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
uv run main.py
which python3
uv add pip
uv pip freeze
```

---

##  📂 Project Structure

```bash
my-new-project/
├── main.py
├── pyproject.toml
├── .venv/
└── README.md

```
---

##   ▶️ Running Your Code

To activate the virtual environment:

```bash
source .venv/bin/activate
```
Then run your main script:

```bash
uv run main.py
```

Example output:

```bash
Hello from my-new-project!
```
---

##  🧩 Managing Dependencies

Add a package:

```bash
uv add <package>

```

Example:

```bash

uv add flask

```

Remove a package:

```bash

uv remove <package>

```

Example:

```bash

uv remove flask

```

Install (sync) all dependencies:

```bash

uv sync

```

List installed packages:

```bash

uv pip freeze

```

---


##  🧹 Cleaning Up

To deactivate the virtual environment:

```bash

deactivate

```
---

##  💡 Notes

This template demonstrates installing and removing packages cleanly.
You can also edit pyproject.toml to declare dependencies.

uv manages both Python versions and environments, making it simpler than combining pyenv, venv, and pip

---

##  💡 References

uv GitHub Repository

Python Packaging Guide
