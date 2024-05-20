# Insurance-Prediction-Analysis
# README

## Final Project: Insurance Charges Analysis and Prediction

This project involves analyzing and predicting insurance charges using a dataset with various attributes such as age, sex, BMI, children, smoker status, and region. The analysis includes data visualization, hypothesis testing, and linear regression modeling.

### Prerequisites

Ensure you have the following R packages installed:

```R
install.packages(c("ggplot2", "MASS", "MLmetrics", "dplyr", "caret", "Metrics"))
```

### Data Description

The dataset contains 348 observations with the following 7 attributes:
- `age`: Age of the individual.
- `sex`: Sex of the individual (0 for female, 1 for male).
- `bmi`: Body Mass Index.
- `children`: Number of children/dependents covered by the insurance.
- `smoker`: Smoking status (0 for non-smoker, 1 for smoker).
- `region`: Region of residence (0 to 3).
- `charges`: Yearly medical charges incurred.

### Project Structure

1. **Data Reading and Visualization**
   - Import necessary libraries.
   - Load and inspect the data.
   - Summary statistics and structure of the data.
   - Check for missing values and duplicates.

2. **Graphical Representation**
   - Histogram of insurance charges.
   - Histogram with quartiles (Q1 and Q3) marked.
   - Boxplot of charges by smoker status.
   - Overlay histogram of charges for smokers vs. non-smokers.

3. **Data Analysis**
   - Hypothesis testing to determine the effect of smoker status and sex on charges.
   - Linear regression modeling using forward and backward stepwise selection.
   - Evaluation of model performance using Mean Absolute Error (MAE) and Mean Squared Error (MSE).

### Usage

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/insurance-charges-analysis.git
   cd insurance-charges-analysis
   ```

2. **Run the R script:**
   Open the script `FinalProject.R` in your R environment and execute it to see the data analysis, visualizations, and linear regression results.

### Key Findings

- **Histogram Analysis:** Insurance charges are right-skewed with most charges in the lower range.
- **Boxplot Analysis:** Smokers have significantly higher insurance charges compared to non-smokers.
- **Hypothesis Testing:**
  - Strong evidence to reject the null hypothesis that there is no difference in mean charges between smokers and non-smokers.
  - Insufficient evidence to reject the null hypothesis that there is no difference in mean charges between males and females.
- **Linear Regression:**
  - Forward stepwise regression identified `smoker`, `age`, `bmi`, and `children` as significant predictors of charges.
  - The forward model had better performance (lower MAE and MSE) compared to the backward model.

### Conclusion

The analysis provides insights into factors affecting insurance charges and demonstrates the application of statistical and machine learning techniques for predictive modeling.

