# Machine-Learning-project

This pdf explains what I analyse and result of the project.  

[Project README.pdf](https://github.com/Kumoichi/Machine-Learning-project/files/10494901/Project.README.pdf)

# Rice Type Classification Dataset

## Data Description
This dataset contains data for classifying rice into two types: Jasmine and Gonen. The dataset is provided in CSV format and has a size of 910 KB. It consists of 18,185 instances and 12 features, including id, Area, MajorAxisLength, MinorAxisLength, Eccentricity, ConvexArea, EquivDiameter, Extent, Perimeter, Roundness, and AspectRation. All features are numeric values.

## Why Use this Dataset for a Machine Learning Project?
- Sufficient Data: With 18,185 instances and 12 features, this dataset provides enough data for analysis and accurate results.
- Numeric Features: All features are numeric values, making it suitable for regression analysis and clear feature correlation understanding.
- No Missing Values: The dataset is complete without any missing values, ensuring accurate analysis.

## Dataset Links
- [Rice Type Classification Dataset](https://www.kaggle.com/datasets/mssmartypants/rice-type-classification)
- [Project Link on Google Colab](https://colab.research.google.com/drive/1t1q-UI9Fb5RSwmEq7xm4K02K_7UKTUh#scrollTo=CvOAAmNm4elI)

## Data Analysis
- Regression: Finding correlations between features using simple LinearRegression and RandomForestRegressor.
- Classification: Comparing all features and specific feature comparisons.
- Experimental Methods: Hypotheses, regression and classification methods used.

## Results & Analysis

### Regression
- Correlation: ConvexArea and MajorAxisLength exhibit some correlation.
- Simple LinearRegression Score: 0.3616
- Simple LinearRegression with Additional Features: By adding Area, MajorAxisLength, EquivDiameter, Extent, Roundness, and AspectRation, the score improves to 0.9865. These features contribute significantly to the improved score.

Comparison between Simple LinearRegression and RandomForestRegressor:
- X = MajorAxisLength, Y = ConvexArea
  - Simple LinearRegression Score: 0.3616
  - RandomForestRegressor Score: 0.0729
  - RandomForestRegressor performs worse due to having only one feature (X). Although RandomForestRegressor usually provides better results, it doesn't perform well when there is only one feature. This is the reason for the lower score obtained with RandomForestRegressor.

Please refer to the [project link](https://colab.research.google.com/drive/1t1q-UI9Fb5RSwmEq7xm4K02K_7UKTUh#scrollTo=CvOAAmNm4elI) for more detailed analysis and experimental details.

