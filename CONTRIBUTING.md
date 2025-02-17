## User experiences, bugs, and feature requests

If you are using `sbi` to infer the parameters of a simulator, we would be delighted to
know how it worked for you. If it didn't work according to plan, please open up an issue
and tell us more about your use case: the dimensionality of the input parameters and of
the output, as well as the setup you used to run inference (i.e. number of simulations,
number of rounds,...).

To report bugs and suggest features (including better documentation), please equally
head over to [issues on GitHub](https://github.com/sbi-dev/sbi/issues).

## Code contributions

Contributions to the `sbi` package are welcome!
In general, we use pull requests to make changes to `sbi`. So, if you are planning to
make a contribution, please fork, create a feature branch and then make a PR from
your feature branch to the upstream `sbi` ([details](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)).
To give credits to contributors, we consider adding contributors who repeatedly and substantially contributed to `sbi` to the list of authors of the package at the end of every year.
Additionally, we mention all contributors in the releases.

### Development environment

Clone [the repo](https://github.com/sbi-dev/sbi) and install all the dependencies using
the `environment.yml` file to create a conda environment: `conda env create -f
environment.yml`. If you already have an `sbi` environment and want to refresh
dependencies, just run `conda env update -f environment.yml --prune`.

Alternatively, you can install via `setup.py` using `pip install -e ".[dev]"` (the dev
flag installs development and testing dependencies).

### Style conventions

For docstrings and comments, we use [Google
Style](http://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings).

Code needs to pass through the following tools, which are installed alongside `sbi`:

**[black](https://github.com/psf/black)**: Automatic code formatting for Python. You can
run black manually from the console using `black .` in the top directory of the
repository, which will format all files.

**[isort](https://github.com/timothycrosley/isort)**: Used to consistently order
imports. You can run isort manually from the console using `isort` in the top
directory.

**[pyright](https://github.com/Microsoft/pyright)**: Used for static type checking.

`black` and `isort` and `pyright` are checked as part of our CI actions. If these
checks fail please make sure you have installed the latest versions for each of them
and run them locally.

## Online documentation

Most of [the documentation](http://sbi-dev.github.io/sbi) is written in markdown ([basic
markdown guide](https://guides.github.com/features/mastering-markdown/)).

You can directly fix mistakes and suggest clearer formulations in markdown files simply
by initiating a PR on through GitHub. Click on [documentation
file](https://github.com/sbi-dev/sbi/tree/master/docs/docs) and look for the little pencil at top right.
