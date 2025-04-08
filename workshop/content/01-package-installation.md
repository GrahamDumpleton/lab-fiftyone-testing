---
title: Package Installation
---

To install and use the `fiftyone` package we will create a virtual environment.
We will use `uv` to do this, although you can use other Python packaging tools
as well.

```terminal:execute
command: uv venv --python 3.12
```

If this was a traditional virtual environment we would activate the virtual
environment and then install any required Python packages, but because we are
using `uv` to create it, we will avoid that and instead use the `uv pip` command
to install packages.

```terminal:execute
command: uv pip install fiftyone
```
