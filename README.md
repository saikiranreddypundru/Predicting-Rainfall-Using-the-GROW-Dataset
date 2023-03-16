# Predicting-Rainfall-Using-the-GROW-Dataset.

## GROW soil moisture data.

Using low cost soil sensors, the GROW Observatory gathered data about soil and growing conditions from various locations across Europe. In total, 6,500 Flower Power sensors were deployed in `24` GROW places across `13` countries, and participants included community groups, land managers, small and family farms, science and educational institutes, and vineyards, agro-forestry, and food-growing establishments with access to land. The sensors were deployed between `November 2017` and `October 2019`, and followed a scientifically validated protocol to collect time series data. Data were collected every `15` minutes and uploaded to the GROW servers by participants using their mobile phones.

The Data for the project is made available by the [GROW Observatory](https://discovery.dundee.ac.uk/en/datasets/grow-soil-moisture-data)

Grow sensors are visualised here:

![Location Data about Grow Sensors](https://github.com/saikiranreddypundru/Predicting-Rainfall-Using-the-GROW-Dataset/blob/main/Grow_Sensor_Locations.png "Grow sensors visualised")

## Data Preparation:

**1. Locations_Cleaned.ipynb**

A preliminary Cleaning of Location data for the sensors, defining peoper bounding boxes for the co-ordinates and some data cleaning
	
**2. Dataprocessing_1.ipynb**:

This is the first part of Data processing notebooks, these databricks notebooks were worked upon in azure cloud. The resultant data from this notebook is fed as an input second notebook. 

**3. Dataprocessing_2.ipynb**:

This is the second notebook from the dataprocessing tasks. The notebook details the generation of train, test and validation datasets which are to be fed to the models. Train_Test_Val_Datasets Folder contains the outputs from this notebook.
	
	The notebooks are split to optimise the costs of computing resources.
	
	
	
## Machine Learning:
The notebook details different models on which the data is trained and performance stats about them. The code is adapted from [Google Tensorflow tutorials](https://www.tensorflow.org/tutorials/structured_data/time_series)

