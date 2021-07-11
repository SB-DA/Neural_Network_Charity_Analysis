# Neural Network Charity Analysis
Created a deep-learning neural network to analyze and classify the success of charitable donations.

![neural](https://user-images.githubusercontent.com/78935551/125122953-15453100-e0c4-11eb-8595-0fa4d953173b.jpg)

> ## Overview
Machine learning and neural networks enabled us to use Bek's dataset to create an unsupervised binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
In the past few years, Alphabet Soup has funded more than 34,000 organizations through its business fundraising efforts. Bek has received a CSV file that contains the full list. The dataset contains columns that contain information about each organization.

With the knowledge of Pandas and the StandardScaler() of Scikit-Learn, compile, train, and evaluate a neural network model based on the dataset 

> ## Results

### Data Processing 
- Variable IS_SUCCESSFUL was considered the target for the model.
- APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT was considered as the features for the model.
- The columns EIN and NAME were neither targets nor features, so it was removed from the input data.

### Compiling, Training, and Evaluating the Model
- The neural hidden layer has 2 neural hidden layers, the first layer has 80 neurons and the second has 30 neurons. The activation function of the first and second hidden layers is "relu" and the activation function of the output layer is "sigmoid".

- 75% of the target could not be reached by the model. According to my model, accuracy was 72%.

- Eliminated the SPECIAL_CONSIDERATIONS, STATUS column and changed the activation function for the three layers to Tanh to see if it performs better than the relu function.

> ## Summary 
Despite deep learning neural networks, the accuracy target set at 75 percent was not met. The model is not outperforming this target level due to the fact that it is pretty regular.
A supervised machine learning model, such as the Random Forest Classifier, could be used since our supervised model is dealing with binary classification.







