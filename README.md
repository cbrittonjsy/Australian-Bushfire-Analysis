# Australian Bushfire Prediction Using Machine Learning and Neural Networks

## Project Summary

This project explores the use of machine learning and deep learning techniques for the prediction of Fire Radiative Power (FRP) based on data gathered from satellites during a period of prolonged bushfire activity in Australia in 2019.

In this project I delve into three different approaches for tackling this regression problem as FRP is a continuous variable and not a class.

The first notebook utilises a traditional machine learning technique, a  random forest regressor. This notebook begins by exploring the dataset, cleaning it and preprocessing it ready for training, then fits and evaluates the random forest regressor.

The second notebook moves on to a deep learning technique where I build a feedforward neural network using PyTorch. The cleaned dataset from notebook 1 is used but additional steps are needed, such as normalisation and tensor transformation. The neural network approach is subsequently comapred to the traditional approach.

The third notebook looks even futher into deep learning with the use of a pre-trained model, TabNet. The use of different batch sizes and epochs is tested and the feedforward neural network from question 2 is comapred to the pre-trained TabNet model.

## Dataset

The dataset used for this project contains Australian bushfire data, with information about the fire's intensity and other environmental factors. The data is sourced from satellite observations by NASA's Visible Infrared Imaging Radiometer Suite (VIIRS).

The dataset can be accessed via this link: [Australian Bush fire satellite data (NASA)](https://www.kaggle.com/datasets/nagarajbhat/australian-bush-fire-satellite-data-nasa?select=fire_archive_V1_101674.csv)

The dataset consists of the following columns:


| **Column**        | **Description**                                      | 
|-------------------|------------------------------------------------------|
| `latitude`        | Latitude of the fire's location                      |
| `longitude`       | Longitude of the fire's location                     |
| `bright_ti4`      | Thermal infrared brightness measured by VIIRS I-4    |
| `scan`            | Along scan pixel size                                |
| `track`           | Along track pixel size                               |
| `acq_date`        | Date of VIIRS acquisition                            |
| `acq_time`        | Time of acquisition                                  |
| `satellite`       | Satellite recording the data                         |
| `instrument`      | Instrument used (MODIS or VIIRS)                     |
| `confidence`      | Measure of quality of fire detection                 |
| `version`         | Data collection version                              |
| `bright_ti5`      | Thermal infrared brightness measured by VIIRS I-5    |
| `frp`             | Fire radiative power in megawatts                    |
| `type`            | Day or night fire                                    |

## Running the Notebooks

Using a terminal, this repository can be cloned with the command `git clone https://https://github.com/cbrittonjsy/Australian-Bushfire-Analysis.git` to gain access to the notebooks. All dependencies will be listed below as well as in the file `dependencies.txt`.

The dataset will need to be downloaded and saved locally, as well as a countries shapefile which is needed for fire location visualisation. The link for the shapefile will be credited below.

## Dependencies

| **Package**        | **Version** |
|--------------------|-------------|
| geopandas          | 1.0.1       |
| ipython            | 8.31.0      |
| matplotlib         | 3.10.0      |
| numpy              | 2.2.2       |
| pandas             | 2.2.3       |
| scikit-learn       | 1.6.1       |
| scipy              | 1.15.1      |
| seaborn            | 0.13.2      |
| pytorch            | 2.5.1       |


## Acknowledgements

I would like to thank

- **ChatGPT (OpenAI)**: Used for code adjustment, troubleshooting and explanations

- **Claude 3.5 Sonnet (Anthropic)**: Used for debugging

- **Natural Earth Data**: Used for a shapefile of Australia. [Natural Earth Data](https://www.naturalearthdata.com/downloads/10m-cultural-vectors/10m-admin-0-details/)

## Contact

Ciaran Britton\
ciaranbritton10@gmail.com\
University of Portsmouth
