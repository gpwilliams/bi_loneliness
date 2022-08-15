# Dunne, S., Williams, G. P., Bradbury, C., Keyes, T., Lane, A. R., Yang, K., & Ellison, A. (August, 2022). A life in lockdown: Brain injury survivors' experiences of loneliness in lockdown.

This repository contains the data, code, and analysis product necessary to reproduce the analyses described in Dunne et al. (August, 2022). [*A life in lockdown: Brain injury survivors' experiences of loneliness in lockdown.*](https://osf.io/rbtms/).

This repository, along with materials and interview transcripts, is hosted on the [OSF](https://osf.io/rbtms/).

Please see the metadata file for a description of the files and folders in this repository.

This work is licensed under [CC-By Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode).

# Reproducing the analyses in Python

The cleanest way to reproduce these analyses is to create a virtual environment in Python and then install the required packages using the requirements.txt file.

## Using conda virtual environments

- To create a virtual environment: `conda create -n bi_loneliness python=3.9.5`.

- Activate the virtual environment: `conda activate bi_loneliness`.

## Using venv

Open the terminal and run the following:

- To create a virtual environment: `python -m venv venv`.

- Activate the virtual environment: `source venv/bin/activate`.

## For both methods

Install the necessary packages from the requirements.txt file: `pip install -r requirements.txt`.

You should now be ready to run the code in the repository. Note, if this did not work try installing the same python version used in our analyses, Python 3.9.5.

# Deactivating and removing the environment

## Using conda virtual environments

To deactivate the environment: `conda deactivate`.

To delete the virtual environment: `conda remove -n bi_loneliness --all`.

## Using venv

To deactivate the environment: `deactivate`.

To delete the virtual environment: simply delete the folder containing the environment.
