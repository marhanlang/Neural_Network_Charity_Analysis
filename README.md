# Neural_Network_Charity_Analysis

# Overview:
The purpose of this analysis is to assist the foundation in predicting where to make investments using the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

# Results: 

## Data Preprocessing
![ResultImage](https://github.com/marhanlang/Neural_Network_Charity_Analysis/blob/main/ASOptimization.png)

- What variable are considered the target for the model?
  - IS_SUCCESSFUL
- What variable(s) are considered to be the features for the model?
  - APPLICATION_TYPE,	AFFILIATION	CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT	
- What variable(s) are neither targets nor features, and should be removed from the input data?
  - EIN, NAME
  
## Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model?
  - Layer 1: 80 neurons, ReLU 
  - Layer 2: 28 neurons, ReLU
  - Output Layer: 1 neuron, sigmoid
 
- Were you able to achieve the target model performance?
  - I was unable to achieve 75% accuracy. The highest accuracy I was able to accomplish was 71.6%.
- What steps did you take to try and increase model performance?
  - Bin ASK_AMT by amount 5000 or less than 5000, Remove SPECIAL_CONSIDERATIONS and STATUS, Add Hidden Layer, Change number of Neurons for Hidden Layers
  
# Summary: 
In the end of this analysis, I was unable to meet the target 75% accuracy despite mulitple attempts to narrow data for optimal processing. A different model such as a RandomForest classifier could solve this classification problem because it works in a similar fashion and is more interpretable. A Random Forest model would also require less preparation before begnning the analysis.
