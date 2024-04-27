# Tracking barbell exercises

## Overview

The original idea of the idea is taken from the bloom of smart-tracking devices like [Apple Watch](https://www.apple.com/watch/), [Meta Motions](https://mbientlab.com/metamotions/), etc. And while there are activity-recognizing applications, there are still not much applications specifically on gym activities, which are really potential.

This project aim is to create a machine learning model that can automatically classify barbell exercises and count repetitions from quantified information.

## About barbell exercises


![barbel_exercises](docs/problemsAnalysis/barbelExercises.jpg)

Barbell exercises are weight-training exercises that involve lifting heavy weights loaded onto a barbell. These exercises are typically seen in the gym. 

There are five exercises in this project: Bench Press, Deadlift, Overhead Press, Barbell Row and Quat. 

## About the quantified self

The quantified self is any individual engaged in the self-tracking of any kind of biological, physical, behavioral, or environmental information. 

The self-tracking is driven by a certain goal of the individual, with a desire to act upon the collected information — Hoogendoorn, M., & Funk, B. (2018). Machine learning for the quantified self. On the art of learning from sensory data.



## About the dataset

There are five participants joining in the dataset, which there information in the image below, noticing that Experience column showing the time experience individual has on gym. 

![participants](docs/problemsAnalysis//participants.png)

The dataset was collect through a [Meta Motions](https://mbientlab.com/metamotions/) watch in two weeks during January 2019, every participants were asked to do a light set and heavy set on the following barbell exercises. 

During each set, the data was collected through Accelerometer and Gyroscope measurement and were saved in different files. For better understanding how these two works, please check out [**docs/Accelerometer-and-Gyroscope.md**](docs/Accelerometer-and-Gyroscope.md).

The time stored in the dataset is written in Unix time. You can read it in [**docs/Working with Unix time**](docs/Working-with-Unix-time.md)


## Process 

Below are my processes of making this project, you can check detailed documents for everything I've made.

1. [Problem's Analysis](docs/problemsAnalysis/)
2. [Processing Raw Data](docs/processingRawData/)
3. [Data Visualization](docs/dataVisualization/)
4. [Outliers Detection](docs/outliersDetection/)
5. [Feature Engineering](docs/featureEngineering.md)
6. [Predictive Modelling](docs/predictiveModelling/)
7. [Counting Repetitions](docs/countingRepetitions/)


## Installation 
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

## References
Thank you [Cookie Cutter](https://drivendata.github.io/cookiecutter-data-science/) for awesome Data Science template.

Thank you Mark Hoogendoorn and Burkhardt Funk from the book [Machine Learning for the Quantified Self, On the Art of Learning from Sensory Data](https://link.springer.com/book/10.1007/978-3-319-66308-1) for awesome book and [good codes](https://github.com/mhoogen/ML4QS/tree/master/Python3Code). 

## License
This repository license is under the MIT License.

Please check the LICENSE. 

## Contact

If you want to have more information, please contact me through lenam1072004@gmail.com

