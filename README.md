# jupyterenv
Environment and configuration for running jupyter notebooks

# Installation
1. Clone this repository
2. Inside the repository, run the commands below
3. Edit your `~/.zshenv` and make sure you have something like `export JUPYTER_CONFIG_DIR=~/GitHub/jupyterenv/config`

```
pyenv virtualenv 3.9.4 jupyter
pyenv local jupyter
poetry install
pyenv rehash

# Enable nbextensions
jupyter nbextension enable --py widgetsnbextension --sys-prefix
jupyter contrib nbextension install --sys-prefix
jupyter nbextensions_configurator enable --sys-prefix

# Enable nbdime
jupyter serverextension enable --py nbdime --sys-prefix
jupyter nbextension install --py nbdime --sys-prefix
jupyter nbextension enable --py nbdime --sys-prefix

```
