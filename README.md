# Dunne, S., Williams, G. P., Bradbury, C., Keyes, T., Lane, A. R., Yang, K., & Ellison, A. (August, 2022). A life in lockdown: Brain injury survivors' experiences of loneliness in lockdown.

This repository contains the data, code, and analysis product necessary to reproduce the analyses described in Dunne et al. (August, 2022). [*A life in lockdown: Brain injury survivors' experiences of loneliness in lockdown.*](https://osf.io/rbtms/).

This repository, along with materials and interview transcripts, is hosted on the [OSF](https://osf.io/rbtms/).

Please see the metadata file for a description of the files and folders in this repository.

This work is licensed under [CC-By Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode).

# Reproducing the analyses in Python

The cleanest way to reproduce these analyses is to create a virtual environment in Python and then install the required packages using the requirements.txt file. VS Code is recommended to complete the following. 

1. Install VS Code from [https://code.visualstudio.com/download](https://code.visualstudio.com/download).
2. Install Anaconda [https://docs.anaconda.com/anaconda/install/](https://docs.anaconda.com/anaconda/install/) or Miniconda from [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
3. Set up Python in VS Code by following the instructions here [https://code.visualstudio.com/docs/languages/python](https://code.visualstudio.com/docs/languages/python).

Using VS Code ope nthe folder for this repository (File...Open Folder...). 

Next, create a virtual environment from which to run the analyses. For details of working with virtual environments in VS Code, see [https://code.visualstudio.com/docs/python/environments](https://code.visualstudio.com/docs/python/environments) or instead follow the quick instructions below.

## Quick start instructions for using virtual environments

### Using conda virtual environments

- To create a virtual environment: `conda create -n bi_loneliness python=3.9.5`.

- Activate the virtual environment: `conda activate bi_loneliness`.

### Using venv

Open the terminal and run the following:

- To create a virtual environment: `python -m venv venv`.

- Activate the virtual environment: `source venv/bin/activate`.

### Installing Packages in the conda or venv environment

Install the necessary packages from the requirements.txt file: `pip install -r requirements.txt`.

# Running analyses in VS Code

Once you have activated the virtual environment and installed the relevant packages, in VS Code you can select your Python interpreter (from the virtual environment) using Cmd + Shift + P. Choose your recently created environment (if using Conda, this should be bi_loneliness Python version 3.9.5). Open the file /python/analysis.ipynb and click the Run All button at the top of the analysis file in VS Code. The whole analyses will rerun from the top of the file to the bottom.

# Deactivating and removing the environment

If you want to deactivate and/or remove the environment after reproducing these analyses, follow these instructions depending on whether you created the virtual environment in conda or venv.

## Using conda virtual environments

To deactivate the environment: `conda deactivate`.

To delete the virtual environment: `conda remove -n bi_loneliness --all`.

## Using venv

To deactivate the environment: `deactivate`.

To delete the virtual environment: simply delete the folder containing the environment.
