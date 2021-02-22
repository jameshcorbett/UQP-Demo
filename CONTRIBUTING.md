Contributions to the UQP
========================

The following contract is an evolution of Github's Fork + Pull model,
aimed at providing an optimal collaboration model for free software
projects.


Design
------

### Preliminaries

-  A "Contributor" is a person who wishes to provide a patch, being a set of commits that solve some clearly identified problem.

-  A "Maintainer" is a person who merge patches to the project. Maintainers are not developers; their job is to enforce process.

-  Contributors do not have commit access to the repository unless they are also Maintainers.

-  Maintainers do have commit access to the repository.


### UQP Maintainers

The UQP is an open source project and is developed by a team of scientists and software developers at
Lawrence Livermore National Laboratory. The maintainers of the project are the members of that team.


### Licensing and Ownership

-  The UQP uses the LGPL v2.1 license.

-  The copyrights in the UQP project are owned collectively by all contributors. No copyright assignment is required to contribute to UQP.

-  The git commit history is considered the primary source of contributor identities.


### Patch Requirements

-  Maintainers and Contributors must have a Github account and should use their real names or a well-known alias.

-  A patch should be a minimal and accurate answer to exactly one identified and agreed problem.

-  A patch must adhere to the code style guidelines.

-  A patch must not include non-trivial code from other projects unless the Contributor is the original author of that code.

-  A patch must compile cleanly and pass project self-tests on at least the principle target platform.

-  A patch must be accompanied by a commit message.

-  A commit message should consist of a title (50 characters or less) summarizing the change, optionally followed by a blank line and a message body.

-  A commit message should be written in the imperative (Fixes or Fix).

-  A commit message title should denote the section of code being changed with a tag followed by a single colon, e.g. ``name: short description``.

-  A commit message title should include a period.

-  A commit message body should be wrapped at 72 characters, with the exception of non-prose lines like list items, quoted text, or quotes from other commits.

-  A commit message body should include a description of the change being made and its reason and/or purpose.

-  Where applicable, a commit message body should reference a Github Issue by number (e.g. Fixes #33").

-  A commit message body should begin with ``Problem:`` and a short paragraph describing the problem solved by the commit.  Even commits that add features MAY include such a problem statement.

-  A "Correct Patch" is one that satisfies the above requirements.


### Development Process

-  Change on the project should be governed by the pattern of accurately identifying problems and applying minimal, accurate solutions to these problems.

-  To request changes, a user should log an issue on Github, describing the problem they face.

-  To work on an issue, a contributor should fork the repository and then work on their forked repository.

-  To submit a patch, a contributor should create a Github pull request back to the project.


### Creating Stable Releases

-  The project has one branch ("main") that always holds the latest in-progress version and should always build.

-  To make a stable release someone should fork the repository by copying it and thus become maintainer of this repository.

-  Forking a project for stabilization may be done unilaterally and without agreement of project maintainers.

-  A stabilization project should be maintained by the same process as the main project.

-  A patch to a stabilization project declared "stable" should be accompanied by a reproducible test case.


### Python Coding Style

All Python code must be formatted with ``Black``.

