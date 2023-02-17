# liver-fibrosis-on-ct-
Liver Fibrosis Classification using CT Texture Features
Liver Fibrosis Classification using CT Texture Features
This Python code analyzes and tests machine learning models (Support Vector Machines, Random Forests, and Neural Networks) for classifying the presence of liver fibrosis based on CT texture features.

Data Preprocessing
The data is split into input (X) and output (y) variables. The values are shifted to make them non-negative and extreme values are replaced with the nearest values within the 5th and 95th percentile range. The resulting X data is converted to a pandas DataFrame. The correlation matrix is calculated, and highly correlated features are dropped. Principal component analysis (PCA) is performed on the remaining features, and the number of components needed to explain 95% of the variance is determined.

Training and Testing
The X and y data is split into training and testing sets using a 0.2 test size and a random state of 0. The X training data is standardized using a StandardScaler. Three classifiers are used: Support Vector Machines, Random Forests, and Neural Networks. The classifiers are trained on the X training data and evaluated on the X testing data. The ROC curve is plotted for each classifier.

Saving Trained Models
The SVC, Random Forest, and Neural Network models are trained and evaluated. The confusion matrix is computed for each model. The trained models are saved using the pickle module.

How to Use
To use this code, you can clone this repository to your local machine and run the Python code on your dataset. You will need to modify the input and output variables to match your dataset, and you may need to adjust the classifier parameters to achieve the best results. You will also need to install the required Python packages, which are listed in the requirements.txt file.

Requirements
This code requires the following Python packages:

numpy
pandas
scikit-learn
matplotlib
seaborn
pickle
