# jupyterhub-binder-template

**The following information was extracted from [Sarah Gibson (The Alan Turing Institute)](https://github.com/alan-turing-institute/the-turing-way/blob/main/workshops/boost-research-reproducibility-binder/workshop-presentations/zero-to-binder-python.md) (21.01.2022). It is a summary of required steps of how to run a Jupyter Notebook in a Git repository using [Binder](https://mybinder.org/).**

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mle313/jupyterhub-binder-template/HEAD)

## How to add a binder badge to your README.md
1. Type in the URL of your Git repository on the [Binder webpage](https://mybinder.org/).
2. Expend the the last toggle element in the gray box (**Expand to see the text below, paste it into your README to show a binder badge:**).
3. Copy the Markdown or ReStructeured text snippet into your `README.md/`.

It should have the following format:
- Markdown
```
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/<GIT USER>/<REPOSITORY>/HEAD)
```
- ReStructured Text
```
.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/<GIT USER>/<REPOSITORY>/HEAD
```
