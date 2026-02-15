---
name: create-repo-readme
description: Generates a high-quality README.md for a repository, starting with project details and usage instructions.
version: 1.0.0
author: Antigravity
created: 2026-02-15
platforms: [claude-code, github-copilot-cli]
category: documentation
tags: [readme, documentation, project-setup, markdown]
risk: safe
---

# Create Repo README

## Purpose
To automatically generate a comprehensive and well-structured `README.md` file for any software project. This skill ensures that the documentation starts with clear project details and usage instructions, making it easy for users to understand and contribute to the repository.

## When to Use This Skill
Use this skill when:
- You are setting up a new repository and need a standard README.
- You want to improve the documentation of an existing project.
- You need a template that covers installation, usage, and contribution guidelines.

## Instructions
1.  **Analyze Project**: Ask the user for the project name, a brief description, and the main programming languages/frameworks used.
2.  **Generate Sections**: Create a `README.md` with the following structure:
    -   **Project Title & Badges**: Add a clear title and optional status badges (e.g., license, build status).
    -   **Description**: A concise summary of what the project does and why it exists.
    -   **Key Features**: A bulleted list of the main capabilities.
    -   **Installation**: Step-by-step instructions to get the project running locally (e.g., `npm install`, `pip install`).
    -   **Usage**: Examples of how to use the project (code snippets or commands).
    -   **Contributing**: Guidelines for how others can contribute.
    -   **License**: Information about the project's license (e.g., MIT).
    -   **Contact**: How to reach the maintainers.
3.  **Refine**: Ask the user if they want to add specific sections like "Roadmap" or "Acknowledgments".
4.  **Output**: Provide the full Markdown content for the user to copy or save directly to `README.md`.

## Examples
**Input:**
"Project Name: TaskMaster
Description: A simple CLI tool for managing daily tasks.
Tech Stack: Python, Click"

**Output:**
# TaskMaster 📝

A simple and efficient CLI tool for managing your daily tasks directly from the terminal. Built with Python and Click.

## Features ✨
-   Add, update, and delete tasks easily.
-   Mark tasks as complete.
-   List all pending tasks.
-   Persistent storage using JSON.

## Installation 🛠️

Prerequisites: Python 3.8+

```bash
git clone https://github.com/username/TaskMaster.git
cd TaskMaster
pip install -r requirements.txt
```

## Usage 🚀

To add a new task:
```bash
python taskmaster.py add "Buy groceries"
```

To list all tasks:
```bash
python taskmaster.py list
```

## Contributing 🤝
Contributions are welcome! Please open an issue or submit a pull request.

## License 📄
This project is licensed under the MIT License.
