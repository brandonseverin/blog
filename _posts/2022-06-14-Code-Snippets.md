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

#### plot legend position

```python
import matplotlib.pyplot as plt

plt.legend(loc='upper right')
```


## Libre Office - Impress

#### Create an image with rounded corners
- Overlay a rectangle with rounded corners over the image. 
- select the image and the rectangle
- right-click -> shapes -> Intersect
