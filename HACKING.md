Contributing to redislite
=========================
Redislite development occurs on github at:
https://github.com/yahoo/redislite

All development should occur on a branch from the redislite github repo.

Prior to submitting a pull request, please complete a <a href="https://yahoocla.herokuapp.com/">Yahoo CLA agreement</a>.

General
-------
Running and testing code requires a c compiler and development environment
sufficient to compile redis and python modules.

Testing
-------
Any changes to source code should be tested, both for regression and for
validation of new code.

* Check for [pep8] conformance.
* Check for general python issues with [pylint] or [flake8]
* Working unit tests are required for all code that adds new functionality.

We recommend adding configuring your development forks in Travis CI so you can
ensure your fork will automatically build correctly using the CI pipeline.

CI Pipelines
------------
Any new change branches should build correctly using CI prior to being
submitted for upstream inclusion.

Submitting Code
---------------
To submit your code for inclusion upstream, do the following to ensure your
submission only includes your new changes:

1.  Complete a Yahoo CLA.
2.  Perform a merge from the MASTER branch of the main redislite repository
    into your fork.  This will ensure your pull request only includes your
    changes and will allow you to deal with any upstream changes that affect
    your code.
3.  Clear up all PEP8 issues before submission.  This will ensure your
    changesets only include code changes and not formatting changes.
4.  Clear up or document exceptions for all PyLint/Flake8 issues.  This will
    ensure the evaluation and review of your code does not have common coding
    errors and decrease the human time to evaluate changes.

## Documentation

Please create documentation in the ``doc/`` folder.

Documentation should all be written in [markdown]. Although github does support 
other formats it seems better just to stabilize on one.

## Style

* Please attempt to follow [pep8] for all code submitted.  This helps make
code merges smaller and more managable.
* Please also attempt to run [pylint] all code submitted.  This finds many
common coding errors and helps ensure good code quality.

[pep8]: http://www.python.org/dev/peps/pep-0008/
[pylint]: http://pypi.python.org/pypi/pylint
[markdown]: http://daringfireball.net/projects/markdown/
[rst]: http://docutils.sourceforge.net/docs/user/rst/quickstart.html