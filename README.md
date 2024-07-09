## MIMB_cellpainting_tutorial

This repository contains the materials for the MIMB cell painting tutorial, including Jupyter Notebooks, data files, and annotations.

## Repository Structure

### Data Directory
- **Data/Annotations/**: Contains various annotation files including:
  - `blocklist_features.txt`: Text file listing features to be blocked, downloaded [here](https://figshare.com/articles/dataset/Blacklist_Features_-_Cell_Profiler/10255811/3)
  - `chemical_annotations.csv`: CSV file containing chemical annotations, dowloaded [here](http://gigadb.org/dataset/100351).
  - `toxcast_data.csv`: The dataset used for estrogen receptor activity prediction, downloaded from [Moleculenet](https://moleculenet.org/datasets-1).
  - `ER_activity_luc_bg1.csv`: The activity dataset obtained after processing `toxcast_data.csv`, can be generated when running `Part3-Machine_Learning.ipynb`


### Cell_Profiles Directory
- **Data/Cell_Profiles/**: Directory containing cell profile data files.
  - `part_1.csv` -> `part_63.csv` queried from [GigaDB](http://gigadb.org/dataset/100351)
        

### Output Directory
- **Data/Output/**: Directory where the output of the Jupyter Notebooks will be stored. This directory is initially non-existing and will be created and generated after running the 1st notebook, it will contain:
  - `output_notebook_1.pkl`: Output of _Part1-Data_Processing.ipynb_ 
  - `output_notebook_2.pkl`: Output of _Part2-Similarity_Analysis.ipynb_ output
  - `ER_activity_luc_bg1.csv` : Output of _ToxCast_Tox21_ERa.ipynb_


### Notebooks Directory
- **Notebooks/**: Contains Jupyter Notebooks for different parts of the tutorial:
  - `Part1-Data_Processing.ipynb`: Notebook for data processing.
  - `Part2-Similarity_Analysis.ipynb`: Notebook for similarity analysis.
  - `Part3-Machine_Learning.ipynb`: Notebook for machine learning tasks.
  - `ToxCast_Tox21_ERa.ipynb`: Notebook to prepare Toxcast data

### Other Files

- **README.md**: This file, provides an overview of the repository structure and contents.
- **LICENSE**: License information 
- **mimb_cellpainting.yml** : File listing Python dependencies.

## Getting Started

To run the Jupyter Notebooks locally on your machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/volkamerlab/MIMB_cellpainting_tutorial.git
   cd MIMB_cellpainting_tutorial

## Setting Up the Environment
For setting up the environment install conda :

1. **Install CONDA**
To install and use Conda; miniconda installer, follow the instructions on the official [Conda installation page](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) for your operating system.

2. **Install pip**
To install pip follow the instructions on the [official pip installation page](https://pip.pypa.io/en/stable/installation/).

3. **Setting Up the Environment**
You can now create and activate the environment with the following commands:

```sh
conda env create -f mimb_cellpainting.yml
conda activate mimb_cellpainting

```
2. **Lunch Jupyter lab**:
Start JupyterLab to work with the notebooks
Once JupyterLab is running, you can navigate to the Notebooks directory and open the relevant notebooks to start working with the tutorial.
```sh
jupyter-lab
```
or
```sh
jupyter-notebook
```
You can open and run, specific notebooks from your terminal as follows; more can be found on the official [Jupyter page](https://docs.jupyter.org/en/latest/running.html).
```sh
jupyter-notebook ToxCast_Tox21_ERa.ipynb
jupyter execute ToxCast_Tox21_ERa.ipynb