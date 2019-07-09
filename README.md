# jupyter

## Setup
- use [miniconda3](https://docs.conda.io/en/latest/miniconda.html)
- make sure miniconda bin path is in $PATH
- conda env create -f environment.yml
- conda activate tadpole
- python setup.py develop
- jupyter lab

## Creating conda environment.yml
- make sure miniconda bin path is in $PATH
- create virtual env:
  `conda create -n tadpole python=3`
  
- `activate tadpole`
- `conda install -n tadpole -y jupyterlab pandas scikit-learn numpy matplotlib ipywidgets widgetsnbextension`
- `conda install -n tadpole -y -c conda-forge ipdb`
- `conda env export -n tadpole --no-builds > environment.yml`
