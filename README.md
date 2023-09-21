# Implementing-K-Nearest-Neighbours-from-Scratch
## Task
Design K-Nearest Neighbour Classifier algorithm from scratch.</br>
Tool Used: Jupyter Notebook, Python
## Building the Classifier
- Define a class and implement all the necessary function in it.
- Initiate the Hyperparameter in __init__ function: distance metrice
- define a function to calculating the distance Metric i.e **Euclidian Distance** and **Manhattan Distance**
- Function to Get the Nearest Neighbour(Get the CLoased value from the test data point)
  - Intiate a distance list and append all the neighbors with there distance(Claculated using the above function)
  - Sort the list in Ascending order i.e closest one with come at first and return the list
- Function to predict the label for the test data point
  - Call the above function to get the sort list of top K datapoints of neighbors with distance
  - Create a empty list of labels and append the labels/ target calues of all the K neighbours
  - Get the mode(Most accuring Label) of the labels found from the above step and return that label
## Implementing the Built model
- Import all the necessary libraries
- Load the data using read_csv method of Pandas
- Analyse the data
- Split the data into Features and Target and convert them into numpy array
- Split into training and test data
- Combine the X and Y of training data
- Load the built model with the distance metric 'Eucledian' or 'Manhattan'
- Predict the label of the one test data point at a time
- Define a function to predict the label for all the test data points
- Get the accuracy score </br></br></br>
Reference: 7.5.5. Implementing K-Nearest Neighbors Classifier from Scratch in Python | KNN Classifier, Siddhardhan, https://www.youtube.com/watch?v=JcOYd870RWM&list=PLfFghEzKVmjsNtIRwErklMAN8nJmebB0I&index=115
