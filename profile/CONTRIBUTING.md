# Contributing to PyRolL

The following is a set of guidelines for contributing to the PyRolL project, either the PyRolL Core, Documentation, or
Plugin and Extension packages hosted within
the [`pyroll-project` organization on GitHub](https://github.com/pyroll-project). These are mostly guidelines to
facilitate an efficient development workflow, and not necessarily rules. Use your best judgment, and feel free to
propose changes even to this document in a pull request.

## Wait I don't want to read this. I just have a quick question/bugfix!

1. If your question relates to a bug in PyRolL, please briefly search the `issues page`_ and open a new labeled issue if
   you don't see anything related to your question there.
2. You can also contact us on stackoverflow with the tag 'PyRolL'. There we will answer your questions. For bug fixes,
   please open an issue on GitHub, as mentioned before.

## License

PyRolL is released as an open-source project under the BSD 3-Clause License. Code contributions should also be
considered open-source.

## What should I know before I get started?

PyRolL is a modulare framework for rolling processes. 
Before you get started, please get familiar with the underlying concept of the framework.
Check out our tests and if you have questions, feel free to reach out to us.

### The structure of PyRolL

PyRolL is structured in several repositories. 
The center part of PyRolL is the `pyroll-core` repository. 
It contains the calculation core and also defines several hooks. 
If you want to know more about hooks, the concepts of PyRolL, check out our [documentation](https://pyroll.readthedocs.io/en/latest/).


### PyRolL developer meetings

If you are interested in discussing PyRolL's development, we encourage you to participate, write us a mail and 
discuss your contribution to the project.
Otherwise, you can always fork the project and present us your changes and how PyRolL would benefit from them.
Also, there is a user meeting, which is held together with the "Freiberger Kalibreurstag" a second date is currently being explored.


### Reporting bugs

> [!NOTE]
> If you find a closed issue that seems like it is the same
> thing that you're experiencing, open a new issue and include a
> link to the original issue in the body of your new one.

Briefly search the issues page to see if the problem has already been reported. If it has and the issue is still open,
add a comment to the existing issue instead of opening a new one.

Bugs are tracked as GitHub issues. You can create an issue on the PyRolL repository by including the following
information:

- Use a clear and descriptive title for the issue to identify the problem.
- Describe the exact steps you took, so we can reproduce the problem as closely as possible.
- Provide sample code that causes the problem. Include code snippets as Markdown code blocks.
- Include information about the environment (OS, python version, how packages were installed) in which you were running
  PyRolL.
- Explain what you expected to happen, and what happened instead.

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. You can create an issue on the PyRolL repository by including the
following information:

- Use a clear and descriptive title for the issue to identify the suggestion.
- Describe the exact behavior you would expect the suggested feature to produce.
- Provide sample code that you would use to access the feature. If possible, include code for how you think the feature
  could be built into PyRolL's codebase. Include code snippets as Markdown code blocks.

## Your first code contribution

Unsure where to begin contributing to PyRolL? You can start by looking through these good-first-issue and help-wanted
issues:

- Good first issues - issues which should only require a few lines of code, and a test or two.
- Help wanted issues - issues which should be a bit more involved than beginner issues.

## Pull requests

The process described here has several goals:

* Maintain PyRolL's quality
* Fix problems that are important to users
* Engage the community in working toward the best possible tools
* Enable a sustainable system for PyRolL's maintainers to review contributions

Please follow these steps to have your contribution considered by the maintainers:

* Keep the changes in your pull request as focused as possible - only address one issue per pull request wherever
  possible.
* Follow the `Styleguides`_
* Assign the appropriate label (see `Issue and pull request labels`_) to your pull request. If you are fixing a specific
  Github issue, reference the issue directly in the pull request comments.
* If you are aware which maintainer is most closely related to the code you've edited, feel free to request their
  review.
* After you submit your pull request, verify that all status checks are passing.
* If a status check fails and it seems to be unrelated to your changes, explain why the failure is unrelated as a
  comment in your pull request.
* If you add a new external dependency, please check it is up to date. Packages which have not been updated for five
  years are considered outdated.
* If you rename an existing python module, please open a separate pull request to simplify the review process.

While the prerequisites above must be satisfied prior to having your pull request reviewed, the reviewer(s) may ask you
to complete additional design work, tests, or other changes before your pull request can be ultimately accepted.

## Styleguides

### Git commit messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line

> [!NOTE]
> Managing git commits is much easier using an IDE (we recommend PyCharm).

### Python styleguide

Please follow the PEP8 conventions for all python code added to PyRolL. Pull requests will be checked for PEP8, and will
be rejected if they do not meet the specified formatting criteria.

Any new features should include coverage with a unit test, such that your pull request does not decrease PyRolL's
overall coverage.

### Documentation styleguide

All new/modified dode objects should include a docstring that is valid reStructuredText to be used by Sphinx Autodoc.

Documentation is built automatically with Sphinx, and resides wihtin
the [`pyroll-docs` repository](https://github.com/pyroll-project/pyroll-docs)

Notebooks created to exemplify features in PyRolL are very useful, and can even be used as integration tests. If you
have added a major feature, consider creating a notebook to show its usage in
the [`pyroll-examples` repository](https://github.com/pyroll-project/pyroll-examples). See the other examples that are
already there.