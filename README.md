# Cookiecutter Genomics Project Template

The goal of this template is to
organize your computational genomics projects.


### Requirements to use the cookiecutter template:
-----------
 - Python 3.5+
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```

### To start a new project, run:
------------

    cookiecutter https://github.com/santiago1234/cookiecutter-genomics-project


### The resulting directory structure

The directory structure of your new project looks like this: 
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

### Carrying out a sinlge experiment

Inside the results dir is where experiments are performed, to se a new
experiment/analysis use the [cookiecutter-analysis-directory](https://github.com/santiago1234/cookiecutter-analysis-directory)

```bash
cookiecutter https://github.com/santiago1234/cookiecutter-analysis-directory
```

### References

This template is based on my personal experience working in bioinformatics projects,
as well as the best practices and insights gained from:

* [Noble 2009, A Quick Guide to Organizing Computational Biology Projects](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000424)
* [Buffalo 2015, Bioinformatics Data Skills](https://vincebuffalo.com/book/)
* [Wilson et al 2017, Good enough practices in scientific computing](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510)
