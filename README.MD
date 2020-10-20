# PTDEX score calculation

This repository contains jupyter notebooks to compute PTDEX scores from differential expression input files.

### System requirements and installation guide
The notebooks run on Python 3 which can be found [here](https://www.python.org/downloads/release/python-360).
The overall installation from scratch should take less than 10 minutes.

To run the notebooks with all the necessary libraries, it is recommended to set up a virtual environment. This can be done with the `virtualenv` package, installable with
```bash
pip3 install virtualenv
``` 

With this package on, we can create, activate and set up a virtualenv with the following commands:
```bash
virtualenv -p python3 venv
source venv/bin/activate
(venv) pip3 install -r requirements.txt
```
We now need to add the virtual environment into the jupyter kernel.
```bash
(venv) ipython kernel install --user --name=venv
```

### Demo and instructions for use
Once this is done, one can simply visualize and run the notebooks with
```bash
(venv) jupyter notebook
```
Once the notebook is launched, the `venv` kernel can be selected in the dropdown menu.
The notebooks can be ran sequentially by selecting the cells and `cmd + enter`. For an introduction to jupyer notebooks, please refer to [this tutorial](https://realpython.com/jupyter-notebook-introduction/). Alternatively, all cells can be ran by clicking on the two triangles icon, which will restart and run the notebooks, taking the input data from the `data` folder and generating the scores used in the analysis in the output folder `output`.
