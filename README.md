## Zero-dose Risk Prediction

Analysing the performance of predictive algorithms in estimating the risk of being a zero-Dose child in India, Mali, and Nigeria using Demographics and Health Surveys (DHS) data https://dhsprogram.com/data/


The Code folder contains the following four Jupyter Notebook files: 

1. Preprocess_data.ipynb: Contains the script to preprocess a .dta file, creating necessary categories and splitting the dataset per country-year. 
2. Summary_statistics.ipynb: Creates the summary statistics of each country-year dataset, including the mean and standard deviation for each predictor.
3. Models.ipynb: Generates training models by using a 70% sample from each dataset in a way that maintains the regional stratification used by DHS to account for heterogeneity across regions. The cost-sensitive versions of the following four supervised learning algorithms are compared against each other: Ridge Classification, Decision Tree, Nearest Neighbor, and Multi-Layer Perceptron. Furthermore, models are trained on relatively older data and then applied to the test data collected a few years later. 
4. Comparison_geotarget_vs_model.ipynb: Compares the performance of the machine learning approach to a simple geographic rule that target districts with less than 80% full-immunization coverage according to the survey data. 
