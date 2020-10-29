# jupyterenv
Environment and configuration for running jupyter notebooks

# Installation
```
pyenv virtualenv 3.8.6 jupyter
pyenv local jupyter
poetry install
jupyter nbextension enable --py widgetsnbextension --sys-prefix
jupyter contrib nbextension install --sys-prefix
jupyter nbextensions_configurator enable --sys-prefix
```
