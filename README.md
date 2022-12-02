# __Electrochemical Metrics for Corrosion Resistant Alloys__
### Aim:
* Corrosion is a major problem on all sort industries, our Risk Analysis Company aims to predict the pitting corrosion and the conditions that influence them.

### The dataset:
A dataset with multiple sections using different measured corrosion resistance metrics. The six sections include data on various metal alloys with measurements of 1) pitting potential, 2) repassivation potential, 3) crevice corrosion potential, 4) pitting temperature, 5) crevice corrosion temperature, and 6) corrosion potential, corrosion current density, passivation current density, and corrosion rate. The experimental data were collected from 81 publications and include Al- and Fe-based alloys, high entropy alloys (HEAs), and NiCrMo alloys.

|[Article Nature](https://www.nature.com/articles/s41597-021-00840-y)-|[Dataset](https://www.nature.com/articles/s41597-021-00840-y)|
|---|---|

### Insides into the dataset:
The dataset has different sessions. 
1. HEA has several target values which make it a richer prediction interest. However there were many missing data and only 53 observations. 
2. Repasivation potential has 191 observations and are independent from the pitting potential (800 obs).
3. Pitting Temperature:
4. Crevise Corrosion:
5. Other
6. Pitting potential has more than 800 observations for ML. However it has a lot of missing values and dirty data. At the   moment I am not considering nor thinking in consider Methods and conditions of the method.
_______________________

## Requirements:

- pyenv with Python: 3.9.4

### Setup

Use the requirements file in this repo to create a new environment.

```BASH
make setup
 brew install hdf5
 brew install graphviz

#or

pyenv local 3.9.8
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements_dev.txt

### NNeworks
export HDF5_DIR=/opt/homebrew/Cellar/hdf5/1.12.2

pip install -U pip
pip install --no-binary=h5py h5py
pip install -r requirements.txt
```
#and 
you should reinstall the requeriments.txt eventually again
pip install -r requirements.txt 

The `requirements.txt` file contains the libraries needed for deployment.. of model or dashboard .. thus no jupyter or other libs used during development.
