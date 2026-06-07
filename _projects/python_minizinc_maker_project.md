---
layout: page
title: Python MiniZinc Maker
description: Generate MiniZinc models programmatically from Python
img: assets/img/projects/python-minizinc-maker/banner.jpg
importance: 1
category: work
related_publications: false
---
* GitHub Repository: [https://github.com/Arthod/python-minizinc-maker]()
* PyPI Package: [https://pypi.org/project/pymzm/]()

Python MiniZinc Maker is an open-source library that allows developers to build pure [MiniZinc](https://www.minizinc.org/) models directly from Python code. Instead of manually writing `.mzn` files, users can define variables, constraints, objectives, and global constraints using a Python API and automatically generate valid MiniZinc models. The project bridges the gap between Python applications and constraint programming workflows powered by MiniZinc.

The library was designed to make optimization and constraint modeling more accessible for Python developers while preserving the flexibility and solver-independence offered by MiniZinc. MiniZinc itself is a high-level constraint modeling language that supports a wide range of optimization and satisfaction problems across multiple solver backends.

## Example Usage

A model can be created entirely from Python by defining variables, constraints, and optimization goals. The generated output is a standard MiniZinc model that can be solved using any MiniZinc-compatible solver.

We give below a 

```python
import pymzm
model = pymzm.Model()

n = 8
q = model.add_variables("q", range(n), val_min=0, val_max=n-1)

model.add_constraint(pymzm.Constraint.alldifferent(q))
model.add_constraint(pymzm.Constraint.alldifferent([q[i] + i for i in range(n)]))
model.add_constraint(pymzm.Constraint.alldifferent([q[i] - i for i in range(n)]))

model.set_solve_criteria("satisfy")
model.generate()

import minizinc
gecode = minizinc.Solver.lookup("gecode")
result = minizinc.Instance(gecode, model).solve(all_solutions=False)
# queen on column i is in row results[0, f"q_{j}"]
```
