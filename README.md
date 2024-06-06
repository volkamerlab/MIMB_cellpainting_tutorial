## MIMB_cellpainting_tutorial

This repository contains the materials for the MIMB cell painting tutorial, including Jupyter Notebooks, data files, and annotations.

## Repository Structure

### Data Directory
- **Data/Annotations/**: Contains various annotation files including:
  - `blocklist_features.txt`: Text file listing features to be blocked.
  - `chemical_annotations.csv`: CSV file containing chemical annotations.
  - `cytotox_invitrodb_v4_1_SEPT2023.xlsx`: Excel file with cytotoxicity data.
  - `INVITRODBv3_20181017.xls`: Excel file with invitro database version 3 data.

### Cell_Profiles Directory
- **Data/Cell_Profiles/**: Directory containing cell profile data files.
  - `part_1.csv` -> `part_63.csv`
        

### Output Directory
- **Data/Output/**: Directory where the output of the Jupyter Notebooks will be stored. This directory is initially non-existing and will be created and generated after running the 1st notebook.

### Notebooks Directory
- **Notebooks/**: Contains Jupyter Notebooks for different parts of the tutorial:
  - `Part1-Data_Processing.ipynb`: Notebook for data processing.
  - `Part2-Similarity_Analysis.ipynb`: Notebook for similarity analysis.
  - `Part3-Machine_Learning.ipynb`: Notebook for machine learning tasks.

### Other Files

- **README.md**: This file, provides an overview of the repository structure and contents.
- **LICENSE**: License information 
- **requirements.txt** : File listing Python dependencies.

## Getting Started

To run the Jupyter Notebooks locally on your machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/volkamerlab/MIMB_cellpainting_tutorial.git
   cd MIMB_cellpainting_tutorial

## Setting Up the Environment
For setting up the environment install conda :

1. **Install CONDA**
To install and use Conda, follow the instructions on the [official Conda installation page](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).

2. **Install pip**
To install pip follow the instructions on the [official pip installation page](https://pip.pypa.io/en/stable/installation/).

3. **Setting Up the Environment**
You can now create and activate the environment with the following commands:

```sh
conda create --name mimb_cellpainting python=3.8
conda activate mimb_cellpainting
pip install -r requirements.txt
