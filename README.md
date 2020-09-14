![Test Status](https://github.com/ElodieFZ/tests_CI/workflows/tests/badge.svg)
[![Coverage Status](https://coveralls.io/repos/github/ElodieFZ/tests_CI/badge.svg?branch=github_workflow)](https://coveralls.io/github/ElodieFZ/tests_CI?branch=github_workflow)

# Test via command line

Package must be added to PYTHON_PATH beforehand
For example, if in a conda environment,

```bash
ln -sf /home/elodief/Work/my_repos/tests_CI/my_module /home/elodief/Soft/anaconda3/envs/senda/lib/python3.8/site-packages
```

To run the test, run one of the following commands from the package root directory:

```bash
python3 test/test_examples.py
python -m unittest
nosetests
pytest
```

# Coverage via command line

```bash
coverage run -m pytest
coverage report
```

# Coverage via github Actions

# 1. Added the coveralls token (one per repository, see https://coveralls.io/github/ElodieFZ) to the Github repo (Settings/Secrets, name COVERALLS_REPO_TOKEN)

