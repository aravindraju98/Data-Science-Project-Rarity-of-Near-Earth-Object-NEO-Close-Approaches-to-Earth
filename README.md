# Data-Science-Project-Rarity-of-Near-Earth-Object-NEO-Close-Approaches-to-Earth

__Team Members:__ Surya Suresh Sriraman, Nivetha Sivakumar, Aravind Raju

__Problem:__

Near-Earth Objects (NEOs) pose a potential threat and necessitate close monitoring for planetary defens.

__Methodology:__

This study investigates factors influencing asteroid close approach rarity and leverages machine learning to predict rarity and classify encounters. We utilize a NASA CNEOS dataset filtered for close approaches within 10 lunar distances (LD). The dataset includes features like velocity, distance, and absolute magnitude, with "Rarity" as the target variable. We employ various machine learning models, including Logistic Regression, Decision Tree, KNN, SVM and Neural Network, to identify the key factors influencing rarity and develop a classification model to categorize encounters based on predicted rarity. 

__Major Outcomes:__

The project compares the performance of these models to determine the most effective approach for NEO encounter classification. The research endeavors to provide accurate predictions of NEO encounter rarity, facilitating a deeper understanding of asteroid dynamics. By leveraging machine learning models, insights are gained into the factors influencing the rarity of NEO close approaches. These outcomes are instrumental in guiding planetary defense strategies and optimizing mission planning for space exploration endeavors. Ultimately, the study contributes to the advancement of knowledge in the field of asteroid dynamics and strengthens efforts to mitigate potential hazards posed by NEOs.


Understanding the characteristics and frequency of asteroid close approaches is crucial for space exploration and potential hazard mitigation. NASA's Center for NEO Studies (CNEOS) tracks NEOs, providing valuable data for scientific research. This project investigates the factors contributing to the rarity of close approaches (Research Question 1) and utilizes machine learning models to predict rarity and classify encounters based on predicted rarity (Research Questions 2 & 3).

We leverage a dataset obtained from the __CNEOS website__ containing information on various NEO characteristics, including "Rarity" as the target variable. The data is filtered for close approaches within 10 LD, focusing on potentially hazardous encounters. By employing machine learning models, we aim to:

1) Identify the key factors (e.g., size, velocity) that most significantly contribute to the rarity of close approaches.
2) Develop multiple machine learning models to accurately predict the rarity of Earth close approaches for asteroids using the provided dataset.
3) Compare the effectiveness of different machine learning models in classifying NEO encounters based on their performance on unseen data.

This project contributes to a better understanding of NEO encounters and explores the potential of machine learning for classifying and predicting their rarity, aiding in space exploration and potential hazard mitigation strategies.

# Introduction
__Approach__ :

1) __Exploratory Data Analysis (EDA):__
    - Descriptive statistics will be used to gain insights into each variable in the dataset.
    - Correlation analysis will identify relationships between variables.  

2) __Data Preparation:__
    - Identify and handle missing values through techniques like imputation or deletion (justifying the chosen method).
    - Address outliers using methods like winsorization if necessary.
    - Standardize or normalize numerical features to ensure consistent scales and improve model performance.
    - Based on EDA insights, create new features that might enhance model performance.
    - Encode categorical features using appropriate techniques like one-hot encoding.

3) __Prepped Data EDA:__    
    - Perform EDA on the prepped data after handling nulls and outliers.

4) __Machine Learning Model Construction:__
    - Employ techniques like recursive feature elimination or feature importance ranking to identify the most informative features 
    - Use VIF to eliminate columns that shows multi-collinearity.
    - Apply dimensionality reduction methods, such as principal component analysis (PCA), to reduce the dataset's complexity while retaining essential information.
    - Build five distinct models to predict asteroid close-approach rarity: 
        - Logistic regression
        - Decision tree
        - KNN
        - SVM
        - Neural network 

5) __Model Selection:__
    - Evaluate the trained models on the unseen dataset using metrics like accuracy, precision, recall, f-1 score
    - Compare the performance of each model and identify the best performing one based on the chosen metrics.

6) __Ensemble Model:__
    - Select weak leaners with low performance and create an ensemble model to enhance overall prediction robustness.
    - Implement and compare ensemble techniques like stacking, voting and bagging.
    
This project is feasible within the given time frame as the scope is manageable, focusing on specific variables to address the research questions effectively.



# Conclusions
This project investigated the factors influencing the rarity of asteroid close approaches and explored the effectiveness of machine learning models in predicting and classifying such encounters. We utilized a NASA CNEOS dataset containing information on various NEO characteristics, focusing on close approaches within 10 LD.

__Key Findings:__

- Our exploratory data analysis revealed significant correlations between rarity and factors like velocity, distance, and absolute magnitude.
- Machine learning models, particularly the KNN classifier, achieved good performance in classifying NEO encounters based on rarity.
- In our case, the stacking ensemble model performed better than voting ensemble model due to more number of weak learners.

__Addressing Research Questions:__

- __Factors Contributing to Rarity:__ The analysis identified absolute magnitude and diameter as key factors influencing rarity.
- __Develop multiple ML models:__ Successfully created ML models like logistic regression, KNN, Decision Tree, Neural Network with promising capabilities in predicting rarity based on various NEO characteristics.
- __Best Performing Model:__ The project successfully developed a best performing Decision Tree classification model with an __accuracy and F-1 score of 0.92__.

## Future Scope

Expanding the dataset to include a broader range of NEO characteristics related to hazard could potentially improve the overall usecase.
