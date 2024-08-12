
# Smoke Detection IoT - Decision Tree Classifier

This project demonstrates how to use a Decision Tree Classifier to predict fire alarms based on IoT sensor data. The dataset used in this project contains various environmental parameters that could influence the occurrence of a fire alarm.

## Project Structure

- **`archive.zip`**: The compressed file containing the dataset `smoke_detection_iot.csv`.
- **`notebook.ipynb`**: The Jupyter notebook that contains the code for loading the data, training the model, and evaluating the results.
- **`README.md`**: Documentation of the project, including a description of the code and how to run it.

## Prerequisites

To run this project, you need to have the following libraries installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `zipfile` (built-in Python module)

You can install these packages using pip:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Project Steps

1. **Unzip Data File**: The `archive.zip` file is unzipped to extract the `smoke_detection_iot.csv` dataset.

2. **Load the Data**: The dataset is loaded into a pandas DataFrame and the first few rows are displayed to understand its structure.

3. **Feature and Target Selection**: Specific columns are chosen as features to train the model, and the target variable is the `Fire Alarm` column.

4. **Data Splitting**: The dataset is split into training and testing sets using an 80-20 split.

5. **Model Training**: A Decision Tree Classifier is trained on the training data. The model's parameters, such as `max_depth` and `min_samples_split`, can be adjusted.

6. **Model Evaluation**: 
   - The accuracy of the model is calculated and printed.
   - A confusion matrix is generated to visualize the performance of the model.
   - The accuracy is recalculated using the confusion matrix for verification.

7. **Visualization**: The confusion matrix is visualized as a heatmap using Seaborn and Matplotlib.

## Running the Project

1. Unzip the `archive.zip` file.
2. Run the Jupyter notebook `notebook.ipynb` to execute the code step by step.
3. Review the output in the notebook, which includes accuracy scores and the confusion matrix heatmap.
