# South-German-Credit
A machine learning project aimed at predicting credit risk using the South German Credit dataset.  The goal of this repository is to show the basic workflow of training a machine model which includes exploratory analysis, data preprocessing, and model evaluation.

Dataset: South German Credit [Dataset]. (2019). UCI Machine Learning Repository. [https://doi.org/10.24432/C5X89F](https://doi.org/10.24432/C5X89F).
> The widely used Statlog German credit data (https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29), as of November 2019, suffers from severe errors in the coding information and does not come with any background information. The 'South German Credit' data provide a correction and some background information, based on the Open Data LMU (2010) representation of the same data and several other German language resources.

From the UCI Machine Learning Repository [page](https://archive.ics.uci.edu/dataset/522/south+german+credit).
***
## Dependencies:
- [Numpy](https://numpy.org)
- [Pandas](https://pandas.pydata.org)
- [Matplotlib](https://matplotlib.org)
- [Seaborn](https://seaborn.pydata.org)
- [Scikit-Learn](https://scikit-learn.org/stable/)
- [Imblearn](https://imbalanced-learn.org/stable/)
- [Tensorflow](https://www.tensorflow.org)
- [XGBoost](https://xgboost.readthedocs.io/en/release_3.2.0/#)
***
## Data Dictionary
|  Variable Name  |  Translation  |  Data Type  |  Description  |
|  ---  |  ---  |  ---  |  ---  |
|  laufkont  |  status  |  Integer  |  Status of the debtor's checking account with the bank (categorical)  |
|  laufzeit  |  duration  |  Integer  |  Credit duration in months (quantitative)  |
|  moral  |  credit_history  |  Integer  |  History of compliance with previous or concurrent credit contracts (categorical)  |
|  verw  |  purpose  |  Integer  |  Purpose for which the credit is needed (categorical)  |
|  hoehe  |  amount  |  Integer  |  Credit amount in DM (quantitative; result of monotonic transformation; actual data and type of transformation unknown)  |
|  sparkont  |  savings  |  Integer  |  Debtor's savings (categorical)  |
|  beszeit  |  employment_duration  |  Integer  |  Duration of debtor's employment with current employer (ordinal; discretized quantitative)  |
|  rate  |  installment_rate  |  Integer  |  Installments as a percentage of debtor's disposable income (ordinal; discretized quantitative)  |
|  famges  |  personal_status_sex  |  Integer  |  Combined information on sex and marital status (categorical)  |
|  buerge  |  other_debtors  |  Integer  |  Is there another debtor or a guarantor for the credit? (categorical)  |
|  wohnzeit  |  present_residence  |  Integer  |  Length of time (in years) the debtor lives in the present residence (ordinal; discretized quantitative)  |
|  verm  |  property  |  Integer  |  The debtor's most valuable property (ordinal)  |
|  alter  |  age  |  Integer  |  Age in years (quantitative)  |
|  weitkred  |  other_installment_plans  |  Integer  |  Installment plans from providers other than the credit-giving bank (categorical)  |
|  wohn  |  housing  |  Integer  |  Type of housing the debtor lives in (categorical)  |
|  bishkred  |  number_credits  |  Integer  |  Number of credits including the current one the debtor has (or had) at this bank (ordinal, discretized quantitative)  |
|  beruf  |  job  |  Integer  |  Quality of debtor's job (ordinal)  |
|  pers  |  people_liable  |  Integer  |  Number of persons who financially depend on the debtor (i.e., are entitled to maintenance) (binary, discretized quantitative)  |
|  telef  |  telephone  |  Integer  |  Is there a telephone landline registered on the debtor's name? (binary)  |
|  gastarb  |  foreign_worker  |  Integer  |  Is the debtor a foreign worker? (binary)  |
|  kredit  |  credit_risk  |  Integer  |  Has the credit contract been complied with (good) or not (bad) ? (binary)  |
***
## Approach
### Data Exploration
- Importing Data
- Conduct exploratory analysis
- Create data visualizations
### Data Preprocessing
- Splitting data into train and test
- Data Resampling
- Data scaling
- Feature Engineering
### Baseline Model Selection
- Train models through supervised machine learning
  - Logistic Regression
  -  K-Nearest Neighbors
  -  Naive Bayes
  -  Support Vector Machine
  -  Random Forest Classifier
  -  Extreme Gradient Boosting
  -  Neural Network
- Evaluate baseline model performance
### Final Model Selection
- Tune best performing models' hyperparameters
- Compare confusion matrix
- Analyze feature importance
- Recommend future improvements
