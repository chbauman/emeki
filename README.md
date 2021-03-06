# Emeki

This is my first python package published on PyPI.

## Installation

Install as follows.

```
$ pip install emeki
```

After a successful installation, it can be run from
the command line:

```
$ emeki
```

## Python command line tool project creation

Emeki includes a command line tool for setting up a 
project as a base for the implementation of a python command line tool
that can be installed via `pip`. Use the flag `--init_pro`
to run it:

```
$ emeki --init_pro
```

It will ask for the name of the author, the name of the 
project and a directory, where the files will be put.
The files include the base structure of a python project
including documentation with Sphinx and testing functionality.
The main commands to run this project are collected in a PowerShell
script `make.ps1`. Unfortunately there is not yet an Unix version available.

## Python library

Alternatively, it can be used as a python library. It mainly provides
some functionality for coping with the file system and for
testing. 

```python
from emeki.util import str2bool

b = str2bool("true")
print(b)
```

## TODO

Some changes that are planned to be implemented in the future:

- Fix deprecation warning for project creation
- Inlcude PyPI username specification during setup (and password saving?)

[![CircleCI](https://circleci.com/gh/chbauman/emeki.svg?style=svg)](https://circleci.com/gh/chbauman/emeki)
