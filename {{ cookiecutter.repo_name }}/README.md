{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------

The directory structure of your new project looks like this: 

├── LICENSE
├── Makefile              <- Makefile with commands like `make data` or `make train` (N/A)
├── README.md         (*) <- The top-level README for developers using YOUR project. 
├── data
│   ├── external      (*) <- Data from third party sources. 
│   ├── interim       (*) <- Intermediate data that has been transformed. (LDS: put your .mat files here)
│   ├── processed     (*) <- The final, canonical data sets for modeling. (LDS: put your .mat files here)
│   └── raw           (*) <- The original, immutable (untouchable) data dump. (LDS: store raw data)
│
├── docs                  <- A default Sphinx project; see sphinx-doc.org for details (N/A)
│
├── models                <- Trained and serialized models, model predictions, or model summaries (N/A)
│
├── notebooks         (*) <- Jupyter notebooks. Naming convention is a number (for ordering),
│                            the creator's initials, and a short `-` delimited description, e.g.
│                            `1.0-jqp-initial-data-exploration`. <--- how to name your scripts!!! (LDS: important)
│                            *** Do your MATLAB documentation/exploration here!!! ***
│
├── references        (*) <- Data dictionaries, manuals, and all other explanatory materials.
│                            LDS: Put papers, links, other relevant papers/comparisons/figures here.
│
├── reports               <- Generated analysis as HTML, PDF, PNG, LaTeX, etc.
│   └── figures       (*) <- Generated graphics and figures to be used in reporting (LDS: Final figs here)
│
├── requirements.txt      <- The requirements file for reproducing the analysis environment, e.g.
│                            generated with `pip freeze > requirements.txt`
│
├── src                   <- Source code for use in this project. (LDS: STORE YOUR MATLAB .m files HERE)
│   ├── __init__.py       <- Makes src a Python module (LDS: we won't use this for now)
│   │
│   ├── data          (*) <- Scripts to download or generate data
│   |   ├─  rexdat_extract.m (LDS: STORE YOUR .m files to convert raw data into useable files here)
│   │   └── make_dataset.py
│   │
│   ├── features          <- Scripts to turn raw data into features for modeling (N/A) 
│   │   └── build_features.py
│   │
│   ├── models            <- Scripts to train models and then use trained models to make
│   │   │                    predictions. (LDS: N/A for now, would like to soon)
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization     <- Scripts to create exploratory and results oriented visualizations
│       ├── makefig.m (*)    (LDS: put your MATLAB Figure generating scripts here)
│       └── visualize.py
│
└── tox.ini                <- tox file with settings for running tox; see tox.testrun.org (LDS: N/A)

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
