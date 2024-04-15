# Hackathon Project - Fight Wildfire

This repository contains our team's work on developing a visualization tool to summarize the gravity of land degradation issues in Brazil focusing on wildfires for the G20 Global Land Initiative Hackathon.

## Task1

### Stage 1: Baseline Model
In the initial phase, we built a baseline model. This model was able to achieve a Test Set Accuracy of 0.9146 after training for 15 epochs using the Adam optimizer.The baseline model is composed of the preprocessing layer of the EfficientNetB0 backbone, the pre-trained EfficientNetB0 base model for feature extraction, pooling to condense the features, and a prediction layer for output. All baseline performances and model specifications can be found in the `baseline_model` directory in this repository.

### Stage 2: Improved Wildfire Detection Model
After obtaining results from the baseline model, we refined and fine-tuned our model in order to build an enhanced version. Details of the improvements and additional features that were included, as well as clarity on the results are documented in the `Task1_Submission` directory.

#### Improvements

##### 1. Data Augmentation

The baseline model lacked data augmentation, which is essential for increasing the model's robustness and reducing overfitting. We incorporated various augmentation techniques such as random flips, rotations, and Gaussian noise to simulate real-world variations in the data.

##### 2. Fine-Tuning on Hidden Dataset

In addition to training on the main dataset, we fine-tuned the model on a smaller, augmented dataset of 20 hidden images. This further improved the model's performance by exposing it to additional unseen data and enhancing its ability to generalize.

## Task 2
Starting from the provided Colab file, we added functions to obtain various metrics from the burned areas. For example, we analyzed how the extension of all types of territories in Brazil has varied over the years, grouping them into:

- ['1-5'] forest
- ['6-7'] shrublands
- ['8-9-16'] savannas
- ['12-14'] croplands
- ['10'] grasslands
- ['11'] wetlands
- ['15'] snowIce


We collected the results in CSV files. Subsequently, based on this data, we observed how the trend of each type has changed over the years to see if there were any trends of interest.

These results were then useful for supporting the final pitch.

We built a mockup using the data provided by the case partner for data visualization `Task2Submission.jpeg`

## Task 3
Thruogh the power-point presentation `G20_LatinStGallen.pptx` we provided and pitched a possible innovative solution to the wildfire problem, trying to tackle the different active actors in the problem

