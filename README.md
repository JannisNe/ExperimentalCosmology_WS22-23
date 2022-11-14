# Experimental Cosmology WS 2022-2023


This directory includes material for the course Experimental Cosmology at the Humboldt University Berlin.
All of the exercises require a working `Python` instance. It's recommended to use `conda` to set up a virtual 
environment in which you can install the required `Python` packages.

## Getting started

### 0. Clone and update this repository

To get all data included in this repository, open a terminal, navigate to the directory you want to work in and execute
```
git clone https://github.com/JannisNe/ExperimentalCosmology_WS22-23_private.git
```

This will create a directory `ExperimentalCosmology_WS22-23_private` in the current directory. \
Any updates that will be posted can be downloaded by simply executing
```
git pull
```

### 1. Installing `Python` / `conda`
`Python` is the programming language we will be using. If you're not familiar with `Python` basics there are plenty 
of introductions, see e.g. https://www.learnpython.org.

If you do not have a `Python` instance set up on your computer, we recommend installing `conda`. `conda` does not only 
provide the interpreter for `Python` but is also a package manager, that allows to easily install ad-on packages that 
we will need. You can find more info here: https://docs.conda.io/projects/conda/en/latest/index.html \
We recommend installing the lightweight `conda` called `Miniconda`: https://docs.conda.io/en/latest/miniconda.html


### 2. Creating a virtual environment
Having installed `conda` you can set up a virtual environment that acts as a closed of programming environment and does 
not interfere with any other programing projects. All info for the environment is contained in `env.yml`. 
In your terminal type
```
conda env create -f env.yml
```

If for some reason this does not work you can set up an empty environment with
```
conda create --name experimental_cosmology python==3.10
```
You will have to install the packages manually as described in 5.

To activate the environment type
```
conda activate experimental_cosmology
```
If you want to leave the environment do
```
conda deactivate
```


### 3. Installing packages separately

If you successfully created the environment from `env.yml`, all packages are installed and you do not need to do 
anything else. \
If you set up an empty environment in step 2. (or you prefered a different way of setting up an environment), 
you can install all packages via `pip`.
All info about packages that are required for this course is located in `requirements.txt`. 
Make sure your environment is activated and execute
```
pip install -r requirements.txt
```


### 4. Running `jupyter`

The `jupyter notebook` is an interface to the interactive `python` called `IPython`. 
Notebook files have the file extension `.ipynb`. The `jupyter lab` allows you to view files, open terminals and 
run several Notebooks. To start it, activate your environment (if you haven't already) and run
```
jupyter lab
```

This opens the `jupyter lab` in your browser. You can now browse for a Notebook file in the file browser on the left
and open it via double click.