---
title: How to contribute
shorthand: Contributing
---

##### Website Development

If you would like to contribute to the development of this website, we suggest you:

1. If there isn't already an [existing Issue](https://github.com/GSTT-CSC/gstt-csc.github.io) that covers the bug fix and/or feature(s) you want to fix and/or add, [create a new Issue](https://github.com/GSTT-CSC/gstt-csc.github.io/issues/new/choose).
2. Go to the GitHub repository [here](https://github.com/GSTT-CSC/gstt-csc.github.io) and fork or clone the repository (see the GitHub documentation [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) for more information on how to do so).
3. Checkout the main i.e., ``gh-pages`` branch first by running ``git checkout -b gh-pages``.
4. Create your Bugfix or Feature Branch off of ``gh-pages`` (``git checkout -b bug/BugFix`` or ``git checkout -b feature/AmazingFeature``).
5. Commit your changes (``git commit -m 'Fixes a SmallBug'`` or ``git commit -m 'Adds some AmazingFeature'``).
   - For commit messages, we recommend this [commit message style](https://cbea.ms/git-commit/) (see [here](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html) for simplified summary).
6. Push to the remote (``git push bug/BugFix`` or ``git push origin feature/AmazingFeature``).
7. Open a [Pull Request (PR)](https://github.com/GSTT-CSC/gstt-csc.github.io/compare) and specify that you want to merge your branch into the ``gh-pages`` branch.
8. A CSC team member will review your PR and, if approved, merge it into the ``gh-pages`` branch and the changes will be automatically updated in the live website.

⚠️ If, at any point, you find something unexpected happens or require further support, [please reach out to us](mailto:CSCTeam@gstt.nhs.uk). 

###### Reviewing your changes during development

You can view your changes during development with a locally-hosted version of the website on your machine by following the Installation instructions in the GitHub repository's README [here](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)).
