# END-TO-END-DATA-SCIENCE-PROJECT

"COMPANY": CODETECH IT SOLUTIONS

"NAME": Narasapuram Safin Sulthan

"INTERN ID": CT06DF620

"DOMAIN": DATA SCIENCE

"DURATION": 6 WEEKS

"MENTOR": NEELA SANTOSH

Dataset and Problem Statement: The foundation of this project is the Iris dataset, one of the most commonly used datasets in machine learning for classification tasks. It contains 150 samples of iris flowers belonging to three species: Setosa, Versicolor, and Virginica. Each flower is described using four numerical features: sepal length, sepal width, petal length, and petal width (all in centimeters). The goal of the model is to classify a given flower into one of the three species based on these four measurements. This makes it a multiclass classification problem, suitable for experimenting with various supervised learning algorithms.

Model Selection and Algorithm: For this task, a Random Forest Classifier was chosen as the machine learning model. Random Forest is an ensemble learning algorithm that constructs a multitude of decision trees during training and outputs the class that is the majority vote among the trees. This method significantly improves accuracy and reduces the risk of overfitting compared to a single decision tree. The algorithm is especially well-suited for problems where interpretability, reliability, and robustness are important, which makes it ideal for this type of structured tabular data

Data Preprocessing and Training: Before training, the dataset was split into training and testing subsets using an 80-20 split. This means that 80% of the data was used to train the model, and 20% was reserved for evaluating its performance. This was done using the train_test_split function from scikit-learn, with a fixed random_state for reproducibility. No advanced preprocessing (like feature scaling) was required in this case because tree-based models like Random Forest are invariant to feature scaling. The classifier was then trained using the training set by calling the .fit() method, which allowed it to learn patterns in the data and build a series of decision trees internally.

Model Saving and Reusability: After the model was successfully trained, it was serialized using Python’s pickle module. Serialization allows the trained model to be saved in a binary format and reloaded later for inference without retraining. The model was saved to a file named iris_model.pkl inside a directory called model/. This file contains the entire trained classifier, including its learned parameters and internal structure. Saving the model in this way is especially useful when deploying it into a web application, as it reduces processing time and allows predictions to be made quickly and efficiently.

Model Performance and Deployment: Although the script doesn't explicitly include performance metrics like accuracy, confusion matrix, or cross-validation scores, the Random Forest algorithm is generally known to perform very well on the Iris dataset, often achieving accuracy levels above 95%. The trained model was later integrated into a Flask web application, where it can make real-time predictions based on user inputs. The application collects the four required features from the user, reshapes them into the expected format, and feeds them into the model to return a prediction. This demonstrates how a machine learning model can transition from a standalone script to a fully interactive web-based tool.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ea6f5e0d-f14d-4f81-9ed0-7984667a4972" />
