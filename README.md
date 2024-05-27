# Readme

## Installation

1. Install Python 3.8 or newer.
2. Install Git 2.27 or newer.
3. To use as a CLI app: 
```sh
pipx install copier
```
4. To use as a library: 
```sh
pip install copier
```
or

```sh
conda install -c conda-forge copier
```

## Quickstart

To generate project from the template:

- On the command-line:

```sh
copier copy path/to/project/template path/to/destination
```

- Or in Python code, programmatically:

```python
from copier import run_copy

# Create a project from a local path
run_copy("path/to/project/template", "path/to/destination")

# Or from a Git URL.
run_copy("https://github.com/copier-org/copier.git", "path/to/destination")

# You can also use "gh:" as a shortcut of "https://github.com/"
run_copy("gh:copier-org/copier.git", "path/to/destination")

# Or "gl:" as a shortcut of "https://gitlab.com/"
run_copy("gl:copier-org/copier.git", "path/to/destination")
```