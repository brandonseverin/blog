---
title: "Code Snippets"
tags: [notes]
toc: true
layout: post
---

## Python

### Anaconda

#### Create an environment spec file (operating system specific)

```bash
conda list --explicit > spec_file.txt
```

#### cloning an environment

```bash
conda create --name myclone --clone myenv
```
#### removing an environment

```bash
conda remove --name myenv --all
```



### General

#### Compatible type hints across various versions
Place the following at the top of the module

```python
from __future__ import annotations
```
See this [stack overflow link here](https://stackoverflow.com/questions/63939138/is-there-a-way-to-use-python-3-9-type-hinting-in-its-previous-versions) for more details and the [python docs](https://docs.python.org/3/library/__future__.html)

#### Greek letters
Python has support for unicode fonts, [source](https://pythonforundergradengineers.com/unicode-characters-in-python.html)
```python
>>> print('Omega: \u03A9')
Omega: Ω
>>> print('Delta: \u0394')
Delta: Δ
>>> print('sigma: \u03C3')
sigma: σ
>>> print('mu: \u03BC')
mu: μ
>>> print('epsilon: \u03B5')
epsilon: ε
>>> print('degree: \u00B0')
degree: °
>>> print('6i\u0302 + 4j\u0302-2k\u0302')
6î + 4ĵ-2k̂
```

#### Automatically reload modules in jupyter notebook
```python
# reload modules if there is a change
%load_ext autoreload
%autoreload 2
```
Place in top cell where modules are imported - useful for rapid testing and development of a python package


#### plot legend position

```python
import matplotlib.pyplot as plt

plt.legend(loc='upper right')
```

## Git

### Commit messages
The commit type can include the following:

- `feat` – a new feature is introduced with the changes
- `fix` – a bug fix has occurred
- `chore` – changes that do not relate to a fix or feature and don't modify src or test files (for example updating dependencies)
- `refactor` – refactored code that neither fixes a bug nor adds a feature
- `docs` – updates to documentation such as a the README or other markdown files
- `style` – changes that do not affect the meaning of the code, likely related to code formatting such as white-space, missing semi-colons, and so on.
- `test` – including new or correcting previous tests
- `perf` – performance improvements
- `ci` – continuous integration related
- `build` – changes that affect the build system or external dependencies
- `revert` – reverts a previous commit 

Example:

```bash
feat: improve performance with lazy load implementation for images
```

Source: [free code camp: how-to-write-better-git-commit-messages](https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/)

## Libre Office - Impress

#### Create an image with rounded corners
- Overlay a rectangle with rounded corners over the image. 
- select the image and the rectangle
- right-click -> shapes -> Intersect

## LaTex
*Large and archaic but for some reason people love it*
Installation on local machine:

https://www.tug.org/texlive/

Best off download the largest package, don't bother with basictex or tiny tex. Just get the full TexLive and MacTex
