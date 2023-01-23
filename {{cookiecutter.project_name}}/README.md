{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── TableOfContents.md <- The table of contents that points to specific/important
    │                           analysis or data.
    │
    ├── data               <- Directory for storing fixed data sets. 
    │   │
    │   ├── generated      <- Important data and results that are generated.
    │   ├── external       <- Data from third party sources.
    │   └── raw            <- The original, immutable data dump.
    │
    │                      Inside each data subfolder we use the naming convention:
    │                           year (last two digits)-month (number, two digits)-short-description
    │                           e.g. `2306-1kgpmetada`, `2307-OtherData`
    │
    ├── docs               <- Project documentation.
    │
    ├── results            <- Directory to place/run experiments, to make a new experiment
    │                           use the cookiecutter template [cookiecutter-analysis-directory].
    │                           This cookiecutter is based on Noble 2009, Carrying Out a Single Experiment
    │
    ├── scratch            <- This folder contains temporal or intermediate files that can be
    │                           easily generated. Periodically the contents of this folder
    │                           will be deleted.
    │
    ├── envs               <- Conda environments for reproducing experiments in the Project.
    │   └── popgene.yaml   <- A conda environment.
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── bin               <- Project-specific scripts.
    │                           This type of scripts provides a generic functionality
    │                           used by multiple experiments within the given project.
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    │
    │
    └── {{cookiecutter.python_module_name}} <- Source code for use in this project.
        ├── __init__.py    <- Makes {{cookiecutter.python_module_name}} a Python module
        │
        ├── data.py        <- Scripts to download or generate data
        │
        └─ utils.py       <- Usefull functions
--------


## Contents

See the [Table of Contents](TableOfContents.md).


## Contact

{{cookiecutter.author_name}} at {{cookiecutter.author_email}}

## CITATION

To cite this project, please see the file [CITATION](./CITATION).
