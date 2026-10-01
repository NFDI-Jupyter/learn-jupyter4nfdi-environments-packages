# Managing environments and packages

## Learning objectives

After working through these materials, you will be able to:

- install packages required for an analysis in Jupyter4NFDI without changing a shared environment;
- identify which Python environment a Jupyter notebook is using;
- create a project-specific Python environment;
- install a project environment as a Jupyter kernel;
- diagnose common package and environment problems.

**Prerequisites**

You should already know how to create and navigate a Jupyter Notebook and have some experience using packages in a programming language such as Python or R.


## Whar are environments for

A research analysis rarely uses only the programming language itself. It normally depends on additional software. Different projects can require different packages or different versions of the same package. For example, Project A needs pandas 2.x and Project B needs pandas 1.x

Installing everything into one shared environment can eventually lead to conflicts. Environments allow projects to keep their software requirements separate.
Let's first check which Python your notebook running. Open a Python notebook and run:

```python
import sys
print(sys.executable)
print(sys.version)
```

The first line tells you which Python executable is running the notebook kernel.  It is one of the most useful checks when troubleshooting Jupyter package problems.
