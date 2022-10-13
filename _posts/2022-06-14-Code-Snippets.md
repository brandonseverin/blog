---
title: "Code Snippets"
tags: [notes]
toc: true
layout: post
---

## Python

### Anaconda

#### cloning an environment

```python
conda create --name myclone --clone myenv
```

### General

#### Compatible type hints across various versions
Place the following at the top of the module

```python
from __future__ import annotations
```
See this [stack overflow link here](https://stackoverflow.com/questions/63939138/is-there-a-way-to-use-python-3-9-type-hinting-in-its-previous-versions) for more details and the [python docs](https://docs.python.org/3/library/__future__.html)
