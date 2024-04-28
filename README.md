# Tracking Barbell Exercises

## Overview

This is my side project to learn about how to create an end-to-end Data Science project.

The original idea of the idea is taken from the bloom of smart-tracking devices like [Apple Watch](https://www.apple.com/watch/), [Meta Motions](https://mbientlab.com/metamotions/), etc. And while there are activity-recognizing applications, there are still not much applications specifically on gym activities, which are really potential.

This project aim is to create a machine learning model that can automatically classify barbell exercises and count repetitions from quantified information.

## About barbell exercises

![Barbell Exercises](docs/problemsAnalysis//barbellExercises.png)
![Exercises Graphs](docs/problemsAnalysis/exercisesGraphs.png)

Barbell exercises are weight-training exercises that involve lifting heavy weights loaded onto a barbell. These exercises are typically seen in the gym. 

There are five exercises in this project: Bench Press, Deadlift, Overhead Press, Barbell Row and Quat. 

## About the quantified self

The quantified self is any individual engaged in the self-tracking of any kind of biological, physical, behavioral, or environmental information. 

The self-tracking is driven by a certain goal of the individual, with a desire to act upon the collected information — Hoogendoorn, M., & Funk, B. (2018). Machine learning for the quantified self. On the art of learning from sensory data.



## About the dataset

There are five participants joining in the dataset, which there information in the image below, noticing that Experience column showing the time experience individual has on gym. Below is the information about the participants:

![participants](docs/problemsAnalysis//participants.png)

The dataset was collect through a [Mbientlab's WristBand Sensor Research Kit](https://mbientlab.com/) in two weeks during January 2019, every participants were asked to do a light set and heavy set on the following barbell exercises. 

During each set, the data was collected through Accelerometer and Gyroscope measurement and were saved in different files. For better understanding how these two works, please check out [docs/Accelerometer-and-Gyroscope.md](docs/Accelerometer-and-Gyroscope.md).

The time stored in the dataset is written in Unix time. You can read it in [docs/Working with Unix time](docs/Working-with-Unix-time.md)


## Process 

Below are the processes of making this project, you can check detailed documents for everythign I've made.

1. [Problem's Analysis](docs/problemsAnalysis/)
2. [Processing Raw Data](docs/processingRawData/)
3. [Data Visualization](docs/dataVisualization/)
4. [Outliers Detection](docs/outliersDetection/)
5. [Feature Engineering](docs/featureEngineering.md)
6. [Predictive Modelling](docs/predictiveModelling/)
7. [Counting Repetitions](docs/countingRepetitions/)


## Installation 

To install and run successfully this repository, please follow these instructions: 

1. Deactivate the current conda environment 
```
conda deactivate
```
2. Create a new environment and download the prerequisite
```
conda env create -f environment.yml
```

3. Check the environment list: 
```
conda env list
```
4. Activate the environment (make sure the name of the environment is correct): 
```
conda activate tracking-barbell-exercises
```

## Reports 
I also visualized every single exercises tracking and script the workflow of the project: 
- [Exercises Visualization](reports/figures/)
- [Project's workflow](reports/projects/)
## Files Structure
```
├── data
│   ├── interim          <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw                <- The original, immutable data dump.
│
├── docs                     <- documents for every steps in the project.
│   └── countingRepetitions 
│   └── featureEngineering
│   └── outliersDetection
│   └── predictiveModelling
│   └── problemsAnalysis
│   └── processingRawData
│
├── reports                 <- Project's reports.
│   └── figures           <- Image of exercises' visualizations.
│   └── projects          <- Project workflow's report.
│
├── src                        <- Source code for use in this project.
│   ├── data                <- Download and generate data.
│   ├── features          <- Turn raw data into features for modeling.
│      └── ml4qs          <- functions from the machine learning for quantified self book
│   ├── models           <- Choose models and use models to make predictions.
│   ├── visualizations <- Visualize the data out.
├── environment.yml
├── LICENSE
├── README.md          <- Overview of the project.
```

## References
Thank you [Cookie Cutter](https://drivendata.github.io/cookiecutter-data-science/) for awesome Data Science template.

Thank you Mark Hoogendoorn and Burkhardt Funk from the book [Machine Learning for the Quantified Self, On the Art of Learning from Sensory Data](https://link.springer.com/book/10.1007/978-3-319-66308-1) for awesome book and [good codes](https://github.com/mhoogen/ML4QS/tree/master/Python3Code). 

Thank you [Dave Ebbelaar](https://www.youtube.com/@daveebbelaar) for the dataset and awesome instructions, I've learnt a lot in this project. 

## License
This repository license is under the MIT License.

Please check the LICENSE file. 

## Contact

If you want to have more information, please contact me through lenam1072004@gmail.com.

