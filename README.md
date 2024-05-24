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
- **Cell_Profiles/**: Directory containing cell profile data files. 

### Output Directory
- **Output/**: Directory where the output of the Jupyter Notebooks will be stored. This directory is initially non-existing and will be created and generated after running the 1t notebooks.

### Notebooks Directory
- **Notebooks/**: Contains Jupyter Notebooks for different parts of the tutorial:
  - `Part1-Data_Processing.ipynb`: Notebook for data processing.
  - `Part2-Similarity_Analysis.ipynb`: Notebook for similarity analysis.
  - `Part3-Machine_Learning.ipynb`: Notebook for machine learning tasks.

### Other Files

- **README.md**: This file, providing an overview of the repository structure and contents.

## Getting Started

To run the Jupyter Notebooks locally on your machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/volkamerlab/MIMB_cellpainting_tutorial.git
   cd MIMB_cellpainting_tutorial

## Setting Up the Environment

To ensure compatibility and reproducibility, it's recommended to use a Conda environment. You can create and activate the environment with the following commands:

```sh
conda create --name mimb_cellpainting python=3.8
conda activate mimb_cellpainting
pip install -r requirements.txt
