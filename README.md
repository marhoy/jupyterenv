# jupyterenv
Environment and configuration for running jupyter notebooks

# Installation
```
pyenv virtualenv 3.8.6 jupyter
pyenv local jupyter
poetry install

# Enable nbextensions
jupyter nbextension enable --py widgetsnbextension --sys-prefix
jupyter contrib nbextension install --sys-prefix
jupyter nbextensions_configurator enable --sys-prefix

# Enable nbdime
jupyter serverextension enable --py nbdime --sys-prefix
jupyter nbextension install --py nbdime --sys-prefix
jupyter nbextension enable --py nbdime --sys-prefix

```
