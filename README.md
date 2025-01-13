<!-- omit in toc -->
# CS102-Jupyter

Contents
- [Binder](#binder)
- [Colab](#colab)
- [On your own machine](#on-your-own-machine)
    - [Conda](#conda)
    - [Manual set up](#manual-set-up)
- [The way I Jupyter in class](#the-way-i-jupyter-in-class)
- [Bugs or Typos?](#bugs-or-typos)

This work is licensed under a [Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by] 
Joshua Maglione

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

---

## Binder

<a target="_blank" href="https://notebooks.gesis.org/binder/v2/gh/joshmaglione/CS102-Jupyter/HEAD">
  <img src="https://mybinder.org/badge_logo.svg" alt="Binder"/>
</a>

Launches this repository in a Jupyter Notebook in your browser. Sometimes Binder can take a few minutes to start, but it should usually be quick. This way you do not have to install anything on your computer.

---

## Colab

<a target="_blank" href="https://colab.research.google.com/github/joshmaglione/CS102-Jupyter">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a> 

Launches the Jupyter notebooks in your browser using Google's Colab server. I believe you need a Google account to run Colab, so use [Binder](#binder) if you do not want to use or create a Google account. A Google account is *not* necessary for the module. 

---

## On your own machine

I mention two ways of installing Python and Jupyter on your machine. This is not an exhaustive list.

You will need to have the repository on your machine as well. A zip file containing the whole repository can be downloaded here:
[zip file](https://github.com/joshmaglione/CS102-Jupyter/archive/refs/heads/main.zip)

#### Conda

[Conda](https://anaconda.org/anaconda/conda) is a very popular way to get Python and associated software on your own machine without needing to get your hands dirty with the installation process. I have not personally used it, but I know others that have and recommend it.

From within Conda, one installs Python, the required packages (see requirements.txt), and Jupyter Lab.


#### Manual set up

If you want to get this up and running on your own machine, then I recommend building a *virtual environment* (via `venv`). This enables you to deviate from the Python your operating system might need.

You can put the venv wherever you want, but it might be most convenient at the base of this directory. For example you could run the following code in the terminal.

```bash
python3 -m venv ./.venv
source ./.venv/bin/activate
```

Note that you might need to use `python` rather than `python3` depending on your settings. 

Once you have a version of Python that you can install packages with, run the following code to make sure you have all of the necessary Python packages.

```bash
pip3 install -r requirements.txt
```

Again, you might need to use `pip` rather than `pip3`.

Finally, run the following to start up Jupyter Lab.
```bash
jupyter lab
```

---

## The way I Jupyter in class

I use [VS Code](https://code.visualstudio.com/) together with many extensions within VS Code for Jupyter Notebooks and Python. There is also [VSCodium](https://vscodium.com/) for those that would prefer to use the version not distributed by Microsoft.

For Python, the extensions I use are 
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
  
For Jupyter Notebooks, the extensions I use are 
- [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- [Jupyter Notebook Renderers](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter-renderers)

I also use [Rainbox CSV](https://marketplace.visualstudio.com/items?itemName=mechatroner.rainbow-csv) for viewing CSV files.

--- 

## Bugs or Typos?

If you find any bugs or typos, please let me know. I also welcome you to create a pull request. 