# Datasets

All the experimental notebooks look for their corresponding datasets in this folder. We'll high level detail each of these.

## WISDM
Consumed by `feature-engineering` experiment. Once the dataset is obtained (https://www.cis.fordham.edu/wisdm/dataset.php), `untar` it and drop its files (leaf level) in `datasets/wisdm` folder.

## WIT
This folder (`datasets/wit`) contains samples gathered by a data-logger that matches specs of the device we're developing that once attached to a subject's waist (Sacrum area) supplies both Accelerometer + Gyroscope data. Datasets located in this folder are consumed by multiple experiments (i.e. `step-identifier`).