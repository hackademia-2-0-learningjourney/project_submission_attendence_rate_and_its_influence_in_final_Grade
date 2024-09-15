Group_Name : SmartSparks
Group Members: Nirajan Subedi, Pratik Neupane, Sadip Tamang, Umang Manandhar

Project Name: Attendance Rate and Its Influence on Final Grades 

## Overview

This Python script generates a pseudo dataset to analyze the influence of attendance rate on final grades and evaluates the performance of a logistic regression model in classifying students as 'High Achievers' or 'Struggling Students'. 

## Dataset Generation

- **Number of Students**: 400
- **Attendance Rate**: Randomly generated between 0% and 100%.
- **Final Grade**: Determined based on whether the student is a high achiever or struggling, with added noise to make the relationship less direct.

### Code Breakdown

1. **Dataset Creation**:
   - `attendance_rate`: Uniformly distributed between 0 and 100.
   - `probability_high_achiever`: Probability derived from attendance rate.
   - `is_high_achiever`: Randomly assigned based on the probability.
   - `noise_factor`: Normally distributed noise added to final grades.
   - `final_grade`: Calculated based on achievement status and noise.

2. **Model Preparation**:
   - **Features**: Attendance Rate
   - **Target**: High Achiever vs. Struggling Student (encoded as 1 and 0).
   - **Train-Test Split**: 70% training, 30% testing.
   - **Standardization**: Features scaled using `StandardScaler`.
   - **Model**: Logistic Regression trained on standardized features.

3. **Evaluation**:
   - **Classification Report**: Displays precision, recall, F1-score, and support.
   - **Confusion Matrix**: Heatmap visualizing prediction performance.
   - **Scatter Plot**: Shows the relationship between Attendance Rate and Final Grade, colored by category.
   - **Histograms**: Distribution of Attendance Rate and Final Grade, categorized by student type.

## Tech Stack Used

- `numpy`
- `pandas`
- `scikit-learn`
- `seaborn`
- `matplotlib`

## Instructions

1. **Install Stacks**: Ensure all necessary packages are installed.
2. **Run the Script**: Execute the script to generate the dataset, train the model, and produce visualizations.
3. **Review Results**: Analyze the output metrics and plots to understand the influence of attendance on student performance.

## Example Output

- **Confusion Matrix**: Visual representation of classification performance.
- **Scatter Plot**: Visualization of how attendance relates to final grades.
- **Histograms**: Distribution of attendance rates and final grades based on student categories.

This script provides insights into how attendance affects academic performance and evaluates a logistic regression model's ability to classify students based on their final grades.
