# Heart\_Disease\_Machine\_Learning\_FinalProject

Heart Disease Machine Learning Project: Classification, Regression, Clustering, Optimization, and Scenario Analysis



\## Project Overview



This project uses the UCI Heart Disease dataset to explore how machine learning can identify patterns in patient health information. The dataset contains 920 patient records and includes measurements such as age, cholesterol, resting blood pressure, and maximum heart rate.



The project focuses on three analytical tasks:



1\. \*\*Classification:\*\* Predict whether a patient has heart disease using Logistic Regression.

2\. \*\*Regression:\*\* Predict a patient's maximum heart rate using Gradient Boosting Regression.

3\. \*\*Clustering:\*\* Identify groups of patients with similar health characteristics using K-Means Clustering.



The models were evaluated and optimized to determine whether their performance could be improved. The final analysis also examines how hypothetical changes in cholesterol and resting blood pressure affect the optimized classification model's predictions.



The models were evaluated and optimized to determine whether their performance could be improved. The final analysis also examines how hypothetical changes in cholesterol and resting blood pressure affect the optimized classification model's predictions. 



\## Machine Learning Results



\### 1. Classification – Logistic Regression



The classification model was used to predict whether a patient had heart disease based on their health measurements.



\- \*\*Testing Accuracy:\*\* 84.78%

\- \*\*Precision:\*\* 83.64%

\- \*\*Recall:\*\* 90.20%

\- \*\*F1-Score:\*\* 86.79%



GridSearchCV was used to optimize the model. The optimized model maintained the same testing accuracy as the original model.



\### 2. Regression – Gradient Boosting Regressor



The regression model was used to predict a patient's maximum heart rate based on other health measurements.



\- \*\*Original Mean Squared Error (MSE):\*\* 522.19

\- \*\*Optimized MSE:\*\* 504.12

\- \*\*Original R² Score:\*\* 0.2407

\- \*\*Optimized R² Score:\*\* 0.2670



The optimized model showed a small improvement in predicting maximum heart rate, although its predictive accuracy remained limited.



\### 3. Clustering – K-Means



K-Means clustering was used to identify groups of patients with heart disease who shared similar health characteristics.



\- \*\*Original Number of Clusters:\*\* 5

\- \*\*Optimized Number of Clusters:\*\* 4

\- \*\*Original Silhouette Score:\*\* Approximately 0.173

\- \*\*Optimized Silhouette Score:\*\* Approximately 0.179



The optimized clustering model showed a slight improvement in how the patient groups were separated, although the silhouette scores suggest the clusters were not strongly defined.



\## Scenario and Impact Analysis



The optimized Logistic Regression model was used to explore how hypothetical changes in cholesterol and resting blood pressure affected heart disease predictions.



Three scenarios were tested:



1\. \*\*Lower Scenario:\*\* Cholesterol and resting blood pressure decreased by 10%.

2\. \*\*Baseline Scenario:\*\* Both measurements remained unchanged.

3\. \*\*Higher Scenario:\*\* Cholesterol and resting blood pressure increased by 10%.



\### Scenario Results



| Scenario | Average Predicted Probability |

|---|---|

| Lower | 54.76% |

| Baseline | 56.80% |

| Higher | 58.81% |



The model predicted a lower average probability of heart disease when both measurements decreased and a higher probability when both increased.



\### Sensitivity Analysis



Cholesterol and resting blood pressure were also tested separately to determine which measurement had a greater effect on the predictions.



| Feature | 10% Decrease | Baseline | 10% Increase |

|---|---|---|---|

| Cholesterol | 55.38% | 56.80% | 58.20% |

| Resting Blood Pressure | 56.18% | 56.80% | 57.41% |



The results showed that the model was more sensitive to cholesterol changes than resting blood pressure changes within the scenarios tested.



These findings demonstrate how changes in input measurements can affect machine-learning predictions. However, the scenarios are hypothetical and do not establish that changing these measurements would directly change a patient's actual heart disease risk.



\## Software Requirements



This project was completed using Python and Jupyter Notebook through Anaconda Navigator.



The following Python libraries are required:



\- pandas

\- numpy

\- matplotlib

\- seaborn

\- scikit-learn

\- IPython



\## How to Run the Project



1\. Install Anaconda or another Python environment that supports Jupyter Notebook.

2\. Download the project files from this GitHub repository.

3\. Make sure `Heart\_Disease\_Scenario\_Impact\_Analysis.ipynb` and `heart\_disease\_uci.csv` are saved in the same folder.

4\. Open the notebook using Jupyter Notebook or JupyterLab.

5\. Run the notebook cells in order, starting from the first cell.

6\. Review the classification, regression, clustering, optimization, scenario simulation, and sensitivity analysis results.



The notebook uses the included CSV dataset, so no personal computer file paths are required.



\## Dataset Source



UCI Heart Disease Dataset, accessed through Kaggle:



https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data/data



\## Project Author



Student ID: Lasgat0980

