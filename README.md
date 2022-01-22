# jupyterhub-binder-template

**The following information was extracted from ["From Zero to Binder in Python!" by Sarah Gibson (The Alan Turing Institute)](https://github.com/alan-turing-institute/the-turing-way/blob/main/workshops/boost-research-reproducibility-binder/workshop-presentations/zero-to-binder-python.md) (21.01.2022) which belongs to [The Turing Way Community](https://github.com/alan-turing-institute/the-turing-way). This repo is an excercise and summary of required steps to run a Jupyter Notebook in a Git repository using [Binder](https://mybinder.org/).**

## Binder Badge
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mle313/jupyterhub-binder-template/HEAD) (Click on the badge, to run the Jupyter Notebook in Binder.)

### How to add a binder badge to your README.md
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

## Add data to your Binder

### Small size data (up to 10 MB)
- Add directly to your repository
- 
### Middle size data (between 10 MB and 100 MB)
- Add a `postBuild` script/file  to your repo
- `postBuild` script can include middle size data into your image
- See [Binder's `postBuild` example](https://mybinder.readthedocs.io/en/latest/using/config_files.html#postbuild-run-code-after-installing-the-environment) for more uses of the `postBuild` script.

### Large size data
- Use a library specific to the data format to stream the data as you're using it or to download it on demand as part of your code
- For security reasons, the outgoing traffic of your Binder is restricted to HTTP or GitHub connections only. You will not be able to use FTP sites to fetch data on mybinder.org

_Note: Only public data can be shared here. In order to share private data, the local deployment of [BinderHub](https://binderhub.readthedocs.io/en/latest/) is required. This is not part of this manual._

## Beyond Notebooks...

**JupyterLab** is installed into your containerized repo by default.
You can access the environment by changing the URL you visit to:

> **<https://mybinder.org/v2/gh/mle/jupyterhub-binder-template/main?urlpath=lab>**

or add `lab` to _URL to open (optional)_ in [Binder](https://mybinder.org/) and go to link generated in the box below.

---

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
