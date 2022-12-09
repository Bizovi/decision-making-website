# Demo of a python setup

- git
- conda
- pipx
- poetry
- VSCode

```bash
# create a virtual environment with a specific python version
conda create -n cd-chess python=3.10.8 
conda activate cd-chess

# check if tools are installed 
python --version  # Python 3.10.8
which python      # (..)/envs/cd-chess/bin/python
poetry --version  # Poetry (version 1.2.2)
git status        # On branch main ...

# install the dependencies and the package that we built
poetry install    # Installing the current project: chess (0.1.0)
poetry add --dev ipykernel  # in order to use jupyter notebooks

# check that all installed well
pip list | grep chess      # chess 0.1.0
pip list | grep ipykernel  # ipykernel 6.19.2
```