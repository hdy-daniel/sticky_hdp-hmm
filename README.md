# Sticky Hierarchical Dirichlet process hidden Markov model (HDP-HMM)

This repository reflects my understanding of the Sticky HDP-HMM. Note some of the code was shamelessly copied from [Tim Hopper](https://github.com/tdhopper/notes-on-dirichlet-processes).

## Jupyter Lab notebook setup

**Install python libs:**<br>
pip install jupyterlab plotly pandas numpy seaborn pyldavis beautifulsoup4 nltk<br>

**Install jupyter extension:**<br>
<sup>This is to generate plotly graphs inline, if install hangs, downgrade to nodejs v9:</sup><br>
choco install nodejs.install --version 9.0.0<br>
jupyter labextension install @jupyterlab/plotly-extension<br>

**run Jupyter Lab**<br>
jupyter-lab.exe<br>

## Docker image
Ther docker image can be executed with: <br>
docker run -p 8888:8888 -v **\<mount dir\>**:/jup notebooks<br>

example:<br>
docker run -p 8888:8888 -v /home/username/projects/notebooks:/jup notebooks
