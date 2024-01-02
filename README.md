# Analyzing Optimal Video Game Playing Conditions

## Introduction
This project investigates the optimal conditions for video game playing by analyzing hardware specifications and their impact on gaming performance. We focus on CPU and GPU features and their relationships with Frames Per Second (FPS) in games.

## Data Preparation
- **Feature Engineering**: Developed new columns like CPU Brand, Model, Series, Generation, and Type.
- **Data Imputation**: Utilized Moore’s Law to impute missing values in the CPU Transistors column using a geometric sequence.
- **Data Cleaning**: Standardized CPU and GPU names, dropped columns with over 50% missing values, resolved dataset conflicts, and converted data types appropriately.

## Exploratory Data Analysis
- Analyzed the relationship between Die Size, Process Size, and Transistor count in CPUs and GPUs, discovering trends in line with technological advancements.

## Hypothesis Testing
- **Goal**: To validate Moore's Law in modern Integrated Circuits.
- **Approach**: Created synthetic columns for the actual and expected number of transistors, comparing them using statistical tests.
- **Results**: Our analysis supported Moore's Law, showing the doubling of transistors approximately every two years.

## Regression Analysis
- **Goal**: Predict FPS using CPU, GPU, and game features.
- **Approach**: Implemented Random Forest Regressor and Deep Neural Network models.
- **Results**: The models effectively predicted FPS, demonstrating the significant impact of hardware on gaming performance.

## Clustering
- **Goal**: Group data points to understand the relationships between gaming settings, FPS, and resolutions.
- **Approach**: Employed K-prototypes and DBSCAN clustering algorithms.
- **Analysis**: Identified meaningful clusters that highlight trends in gaming performance based on hardware configurations.

## Classification
- **Goal**: Predict game settings (low, medium, high, max) based on hardware and game specifications.
- **Approach**: Used Random Forest and LightGBM classifiers.
- **Results**: Successfully classified game settings, providing insights into the hardware requirements for various gaming experiences.

## Conclusion
Our study confirms the continued relevance of Moore’s Law in the context of gaming hardware. We found a strong correlation between hardware specifications and gaming performance, providing valuable insights for gamers and manufacturers.
