
# Process Fault Diagnosis: A Supervised Machine Learning Approach

## Introduction

In this project, we explore various machine learning techniques for diagnosing faults in complex systems. Our focus will be on applying these techniques to the widely used **Tennessee Eastman dataset**, a benchmark dataset for fault diagnosis in a simulated chemical process. The dataset includes process data with multiple fault types, allowing us to experiment with different fault detection methods.

You can access the dataset [here](https://www.kaggle.com/datasets/averkij/tennessee-eastman-process-simulation-dataset).

## Requirements

The following Python packages are required for this project:

```
numpy==1.21.4
pandas==1.3.4
matplotlib==3.4.3
seaborn==0.11.2
scikit-learn==1.1
xgboost==1.5.1
tensorflow==2.7.0
keras==2.7.0
```

## Project Structure

### Part 1: Exploratory Data Analysis (EDA)

We begin by performing **Exploratory Data Analysis (EDA)** to better understand the Tennessee Eastman dataset. This step involves visualizing the data, analyzing its statistical properties, and identifying any underlying patterns or anomalies. EDA is essential for gaining insights into how the system behaves under normal and faulty conditions.

### Part 2: Long Short-Term Memory (LSTM) Networks for Fault Diagnosis

In the second phase, we delve into **Long Short-Term Memory (LSTM) networks**, which are well-suited for analyzing time series data. We'll explore the fundamentals of LSTMs and demonstrate how they can be applied to detect faults in the Tennessee Eastman dataset. By leveraging LSTM's ability to capture long-term dependencies, we aim to improve the accuracy of fault diagnosis in this time-sensitive dataset.

## Metrics and Performance Evaluation

To evaluate the performance of our machine learning models, we use **accuracy** as the primary metric. Below is a summary of the average accuracy scores obtained by different models. These results exclude faults No. 9 and No. 15, and all 52 sensor measurements were retained for the analysis.

| Method                                    | Accuracy  |
|-------------------------------------------|-----------|
| XGBoost                                   | 0.887     |
| Neural Network                            | 0.943     |
| 1D CNN (Time Series)                      | 0.892     |
| LSTM (Time Series)                        | 0.924     |
| ANN + Random Forest                       | 0.936     |

Each method offers unique advantages in diagnosing faults, with LSTM networks and Neural Networks yielding particularly high accuracy scores. The project will continue to evaluate and refine these methods to enhance fault detection capabilities.
