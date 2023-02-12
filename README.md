# An Implementation of Git using Python

## Table of Contents

- [An Implementation of Git using Python](#an-implementation-of-git-using-python)
  - [Table of Contents](#table-of-contents)
  - [General Information](#general-information)
  - [Technologies](#technologies)
  - [Project Objectives](#project-objectives)
  - [Set Up](#set-up)
  - [Commands](#commands)
  - [Underlying Implementation](#underlying-implementation)

## General Information

- In this project, I will try to implement a Git-like version control system called "μgit" from scratch but using Python

- ugit is not exactly Git, but it shares the important ideas of Git. ugit is way shorter and doesn't implement irrelevant features.

## Technologies

- Python
- pip
- git

## Project Objectives

- Built Git from scratch
- Worked with python packaging system
- Set up a virtual environment for development
- Used SHA-1 for implement "the object database"

## Set Up

- Install pip following [instruction](https://pip.pypa.io/en/stable/installation/)
- Clone [this repository](https://github.com/VincentNguyenDuc/DIY-Python-Git.git)
- Within the DIY-Python-Git directory, select the Python interpreter (where pip installed)
- Run:

```bash
pip install .
```

## Commands

```bash
# initialize a ugit repository
ugit init

# print contents from object id
ugit cat-file {object_id}

# commit
ugit commit -m 'message'

# tag
ugit tag {name} {object_id}(optional - use for specific commit / if not available then tag the closet commit)

# List all commits from the chosen commit to the beginning of version history. If not specific object id or refs, then list all commits to the current HEAD
ugit log {object_id / refs}(optional)

# check out
ugit checkout {object_id / refs}
```

## Underlying Implementation
