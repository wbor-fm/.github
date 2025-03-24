# WBOR Code Style

We aim for consistent, readable code across all WBOR projects.

## Python

- **Formatter:** Use [`black`](https://github.com/psf/black) to format all Python code. We recommend setting up an autoformatter in your editor.
- **Docstrings:** Keep line lengths to **72 characters** max in docstrings, per [PEP 257](https://peps.python.org/pep-0257/).
- **Line length:** Follow `black`'s default line length (88 characters) for general code, except for docstrings as noted.
- **Imports:** Group standard library, third-party, and local imports separately and alphabetize within groups (use [`isort`](https://pycqa.github.io/isort/) for conveniance).

### Module Docstrings

Each Python module (file) should begin with a docstring. Keep them concise: a 2-3 sentence summary is enough to describe what the module does at high level. Module docstrings should focus on explaining the purpose of the module itself, not the internal workings of functions imported from other modules (avoid repeating detailed explanations that are already covered elsewhere). 

If more detailed explanations are needed, put them in a separate documentation file or reference external docs.

For a single author, a docstring might look like:

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
    - 1.0.2 (2025-03-23): Add rate limiting and block certain user 
        agents to reduce bot infiltration <@jdoe, @johnd>
"""
```
