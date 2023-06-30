# Beta-Secretase 1 Inhibitor Activity Classification

Beta-Secretase 1 (BACE1) is an enzyme that plays a crucial role in the production of beta-amyloid peptides, which are known to contribute to the formation of amyloid plaques in Alzheimer's disease. Inhibiting the activity of BACE1 is considered a potential therapeutic strategy for Alzheimer's disease treatment. Machine learning techniques can be applied to predict the inhibitor activity of compounds based on their molecular properties.


## Methodology
The following steps were followed to build the classification model:

1. Data Preprocessing:

    Removal of features with zero variance: Features that do not vary across the dataset do not contribute meaningful information for classification and were removed.
    Removal of highly correlated features: Features with a correlation coefficient above 0.95 were identified and removed to eliminate multicollinearity.

2. Feature Selection:

    Genetic algorithms: A genetic algorithm approach was employed to select the 20 best molecular descriptors from the remaining set of features. Genetic algorithms are optimization techniques inspired by the process of natural selection.

3. Model Training and Evaluation:

    Train-Test Split: The dataset was split into training and testing sets in an 80:20 ratio, respectively.
    Ensemble Machine Learning Algorithms: AdaBoost, Extra Tree, Gradient Boosting, and Random Forest algorithms were employed for classification.

## Results and Discussion

The performance of the classification models was evaluated using various metrics, including accuracy, precision, recall, and F1-score. The best performing model in this study was the Random Forest algorithm, which achieved an accuracy of 82.53%. The precision, recall, and F1-score for the active class were 82.39%, 82.53%, and 82.37%, respectively These results indicate that the Random Forest model successfully predicts the inhibitor activity of compounds based on the selected molecular descriptors. The accuracy and balanced precision-recall metrics suggest that the model is capable of effectively identifying both active and inactive compounds.

## Related Paper:

Noviandy, Teuku Rizky, et al. "QSAR Classification of Beta-Secretase 1 Inhibitor Activity in Alzheimer's Disease Using Ensemble Machine Learning Algorithms." Heca Journal of Applied Sciences 1.1 (2023): 1-7.