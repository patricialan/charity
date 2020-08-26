# Neural Network & Deep Learning Models to Fund Charities

Neural networks and deep learning models were created to predict which charities managed money effectively. See [AlphabetSoupChallenge.ipynb](AlphabetSoupChallenge.ipynb) for the models. The target accuracy for prediction was > 75%. The target was not reached. Instead, the most accurate model (73%) was a neural network with one (input-hidden) layer and 132 neurons. This number of neurons was chosen since for one layer, the optimum number of neurons is 2-3X the number of inputs (which was 44). Both one and multiple hidden layers were trialed.

Steps taken to try to increase model performance included data preprocessing: discarding non-feature variables (i.e. columns), and binning low-frequency categorical variables. Attempts to optimize the model itself included increasing the number of neurons per layer, increasing the number of hidden layers, changing the activation functions of the layers, and increasing the epoch number. 

Generally, the dataset seemed to produce higher accuracy with use of "sigmoid" activation function. Also, using deep learning models didn't increase accuracy (highest accuracy of 73% was achieved) beyond neural network models. This suggests that the dataset is more amenable to less complex modelling. Thus, I would trial logistic regression models like Easy Ensemble AdaBoost, Random Forest, or Support Vector Machine (SVM). Random Forest would also rank feature importances, which would help further optimize the model. 

## Resources
### Data
[charity_data.csv](charity_data.csv)

### Software
Python 3.7.7, Jupyter Notebook 6.1.1, tensorflow 2.0.0, scikit-learn 0.23.1, and pandas 1.1.0