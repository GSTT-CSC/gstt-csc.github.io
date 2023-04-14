---
title: How to contribute
shorthand: Contributing
---

##### Website Development

If you would like to contribute to the development of this website, we suggest you:

1. If there isn't already an [existing Issue](https://github.com/GSTT-CSC/gstt-csc.github.io) that covers the bug fix and/or feature(s) you want to fix and/or add, [create a new Issue](https://github.com/GSTT-CSC/gstt-csc.github.io/issues/new/choose)
2. Fork or clone the repository (see the GitHub documentation [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) for more information on how to do so)
3. Since all code changes should be staged on the ``develop`` branch before releases, you will need to checkout this branch first (``git checkout -b develop``)
4. Create your Bugfix or Feature Branch off of `develop` (``git checkout -b bug/BugFix`` or ``git checkout -b feature/AmazingFeature``)
5. Commit your changes (``git commit -m 'Fixes a SmallBug'`` or ``git commit -m 'Adds some AmazingFeature'``)
   - For commit messages, we recommend this [commit message style](https://cbea.ms/git-commit/) (see [here](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html) for simplified summary)
6. Push to the remote (``git push bug/BugFix`` or ``git push origin feature/AmazingFeature``)
7. Open a [Pull Request (PR)](https://github.com/GSTT-CSC/gstt-csc.github.io/compare) and specify that you want to merge your branch into the ``develop`` branch
8. A CSC team member will review your PR and, if approved, merge it into the ``develop`` branch.

Code changes in the ``develop`` branch will be periodically merged into the ``gh-pages`` branch and the changes will be automatically reflected in the live website.


###### Reviewing your changes during development

You can view your changes during development with a locally-hosted version of the website on your machine by following the Installation instructions in the GitHub repository's README [here](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)).
