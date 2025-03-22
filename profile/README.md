# Hello!

[WBOR (91.1 FM)](https://wbor.org) is the noncommercial, community public radio station licensed to Bowdoin College. This is the public repository for our technology operations. Please [contact us](https://wbor.org/contact) if you have any questions or would like to become involved in projects.

# Contributing
We're delighted you want to help contribute to our technical operations. We welcome folks at all levels of experience.

If you'd like to make changes, please follow these steps:
1. Clone the repo that you would like to make changes to your personal GitHub account.
2. Make changes in your local repo.
3. Create a pull request to the main WBOR repo. Someone will review your code and provide feedback if needed.

## Code Style

We aim for consistent, readable code across all WBOR projects.

### Python

- **Formatter:** Use [`black`](https://github.com/psf/black) to format all Python code. We recommend setting up an autoformatter in your editor.
- **Docstrings:** Keep line lengths to **72 characters** max in docstrings, per [PEP 257](https://peps.python.org/pep-0257/).
- **Line length:** Follow `black`'s default line length (88 characters) for general code, except for docstrings as noted.
- **Imports:** Group standard library, third-party, and local imports separately and alphabetize within groups (use [`isort`](https://pycqa.github.io/isort/) for conveniance).

#### Module Docstrings

Each Python module (file) should begin with a docstring. For a single author, this would include:

```python
"""
Module description here.

Author: Jane Doe <@jdoe>
Version: 1.0.1
Last Modified: 2025-03-22

Changelog:
  - 1.0.0 (2025-01-10): Initial version
  - 1.0.1 (2025-03-22): Refactored API interface
"""
```

For multiple authors, create a list, and add authors to the changelog

```python
"""
Module description here.

Authors:
  - Jane Doe <@jdoe>
  - John Doe <@johnd>
Version: 1.0.2
Last Modified: 2025-03-23

Changelog:
  - 1.0.0 (2025-01-10): Initial version <@jdoe>
  - 1.0.1 (2025-03-22): Refactored API interface <@jdoe>
  - 1.0.2 (2025-03-23): Add rate limitng <@jdoe, @johnd>
"""
```
