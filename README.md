# Sun/Goldberg Lab
# Cookiecutter Data Science (GainField Edition) 

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work within the Sun/Goldberg Lab._


#### [Project homepage](http://drivendata.github.io/linussun/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5
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

    cookiecutter https://github.com/linussun/cookiecutter-data-science/  --checkout gainfield

```
[![asciicast](https://asciinema.org/a/9bgl5qh17wlop4xyxu9n9wr02.png)](https://asciinema.org/a/9bgl5qh17wlop4xyxu9n9wr02)
```

### The resulting directory structure
------------

The directory structure of your new project looks like this: 
Note that (*) directories are the principle ones which will be the most useful in the Sun Lab.

```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train` 
├── README.md     (*)  <- The top-level README for developers using YOUR project. 
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw       (*)  <- ``` *The original, immutable data dump.* ```
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks     (*)  <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`. 
│                         *** Do most of MATLAB exploration here!!! ***
│
├── references    (*)  <- Data dictionaries, manuals, and all other explanatory materials.
│               
│
├── reports       (*)  <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures   (*)  <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── src           (*)  <- Source code for use in this project. (LDS: STORE YOUR MATLAB .m files HERE)
│   ├── __init__.py    <- Makes src a Python module (LDS: we won't use this for now)
│   │
│   ├── data      (*)  <- Scripts to download or generate data
│   |   ├─  make_dataset.m  *** (LDS: STORE YOUR .m files to convert raw data into useable files here) ***
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling (LDS: not yet) 
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions (LDS: not yet, would like to soon)
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization * <- Scripts to create exploratory and results oriented visualizations
│       ├── makefigure.m   (LDS: put your MATLAB Figure generating scripts here)
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.testrun.org (LDS: not yet)
```

## Contributing

We welcome contributions! [See the docs for guidelines](https://drivendata.github.io/cookiecutter-data-science/#contributing).

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
