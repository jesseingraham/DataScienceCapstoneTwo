# Electric Motor Temperature Prediction
A project for exploring predictive models for electric motor temperatures and torque.

## File Strucutre
- **README_files/** contains the images shown in this README file.
- **notebooks/** contains jupyter notebooks following the data science method.
- **presentations/** contains a PDF project overview.
- **reports/** contains a PDF report summarizing the process in the notebooks and a text file describing the final models.

## Problem Overview
Without proper temperature management, Permanent Magnet Synchronous Motors can undergo irreversible thermal damage. Furthermore, it is difficult to maintain or replace any sensors within these types of motors. Torque measurement requires the installation of torque transducers which not only add cost, but also take up extra space. Having predictive models for temperatures and torque can help prevent these issues as well as serve as a backup for any failed sensors.

## Data
The dataset used for this project was taken from [Kaggle](https://www.kaggle.com/datasets/wkirgsn/electric-motor-temperature).

## Results
Out of the models compared, the **exponentially weighted moving average regression** model performed the best for temperature predictions. A preview of the predictions vs the truth are shown below as well as the root-mean-squared-error for each temperature:

![Temperature Prediction Results](/README_files/temperature_prediction_results.PNG)

Out of the models compared, the **polynomial regression** model performed the best for torque predictions. A preview of the predictions vs the truth are shown below as well as the root-mean-squared-error:

![Torque Prediction Results](/README_files/torque_prediction_results.PNG)

## Future Work
Future work on this project could include the following:
1. Exploring methods to lower the error spikes at the beginning of each new motor session.
2. Optimizing the predictive models to be fast enough for real time application on a vehicle’s 
computer.
