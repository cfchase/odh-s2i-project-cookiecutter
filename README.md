# ODH s2i Project Cookiecutter


#### [Project homepage](http://drivendata.github.io/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:

 - Python 3.5+
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0

``` bash
pip install cookiecutter
```


###  Simple ODH Project.

A simple, unstructured, and unopinionated project for data science that is deployable as an OpenShift s2i Application.

To generate your project run the cookiecutter and follow the prompts

``` bash
cookiecutter https://github.com/rh-aiservices-bu/odh-s2i-project-cookiecutter --checkout simple
```
After you've generated your project, the following project file structure will be created.

```
├── README.md
├── LICENSE
├── requirements.txt        <- Used to install packages for s2i application
├── 0_start_here.ipynb      <- Instructional notebook
├── 1_run_flask.ipynb       <- Notebook for running flask locally to test
├── 2_test_flask.ipynb      <- Notebook for testing flask requests
├── .gitignore              <- standard python gitignore
├── .s2i                    <- hidden folder for advanced s2i configuration
│   └── environment         <- s2i environment settings
├── gunicorn_config.py      <- configuration for gunicorn when run in OpenShift
├── prediction.py           <- the predict function called from Flask
└── wsgi.py                 <- basic Flask application
```

Follow the project [README.md](https://github.com/rh-aiservices-bu/odh-s2i-project-cookiecutter/blob/simple/%7B%7B%20cookiecutter.repo_name%20%7D%7D/README.md) to create an s2i friendly data science project you can work on in Open Data Hub and deploy to OpenShift.


### Cookiecutter Data Science ODH Project 

S2I buildable version of [cookiecutter-data-science](https://drivendata.github.io/cookiecutter-data-science/), "A logical, reasonably standardized, but flexible project structure for doing and sharing data science work."

To generate your project run the cookiecutter and follow the prompts

``` bash
cookiecutter https://github.com/rh-aiservices-bu/odh-s2i-project-cookiecutter --checkout cds
```
After you've generated your project, the following project file structure will be created.

```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│   │                     the creator's initials, and a short `-` delimited description, e.g.
│   │                     `1.0-jqp-initial-data-exploration`.
│   ├── 0_start_here.ipynb    <- Instructional notebook
│   ├── 1_run_flask.ipynb     <- Notebook for testing flask requests
│   └── 2_test_flask.ipynb    <- Notebook for testing flask requests
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for use inside Jupyter notebooks and 
│                         also used to install packages for s2i application
│
├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py <- the predict function called from Flask
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
├── tox.ini                  <- tox file with settings for running tox; see tox.readthedocs.io
├── .gitignore               <- standard python gitignore
├── .s2i                     <- hidden folder for advanced s2i configuration
│   └── environment          <- s2i environment settings
├── gunicorn_config.py       <- configuration for gunicorn when run in OpenShift
└── wsgi.py                  <- basic Flask application

```

Follow the project [README.md](https://github.com/rh-aiservices-bu/odh-s2i-project-cookiecutter/blob/simple/%7B%7B%20cookiecutter.repo_name%20%7D%7D/README.md) to create an s2i friendly data science project you can work on in Open Data Hub and deploy to OpenShift.