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
    ├── results            <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                           the creator's initials, and a short `-` delimited description, e.g.
    │                           `1.0-jqp-initial-data-exploration`.
    │
    ├── scratch            <- This folder contains temporal or intermediate files that can be
    │                           easily generated. Periodically the contents of this folder
    │                           will be deleted.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── bin               <- Project-specific scripts.
    │                           This type of scripts provides a generic functionality
    │                           used by multiple experiments within the given project.
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
        ├── __init__.py    <- Makes src a Python module
        │
        ├── data           <- Scripts to download or generate data
        │   └── make_dataset.py
        │
        ├── features       <- Scripts to turn raw data into features for modeling
        │   └── build_features.py
        │
        ├── models         <- Scripts to train models and then use trained models to make
        │   │                 predictions
        │   ├── predict_model.py
        │   └── train_model.py
        │
        └── visualization  <- Scripts to create exploratory and results oriented visualizations
            └── visualize.py
--------
