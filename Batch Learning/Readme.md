# Batch Learning

## Offline Machine Learning
It means training the model with the entire data set we have on the local machine, testing the model, and updating it on the server.

**Example**  
A movie recommendation website trained with user data from daily watch history.

**Problem**  
Because the data is big, we can train the model on the server. If we want to update the model with the user's next day watch history data, we need to pull the model, train it with the new + old data, test it, and push it back to the server.

![alt text](/assert/BatchLearning.png)

**Disadvantages**
- The data doubles or triples every time we repeat the process.
- Hardware resources are not available everywhere to download the app trained with the new data every time after updation.
- There is a gap in updating the model with data. In the processing time period, users will use the same old model.

**Libraries for Offline Machine Learning**
- Scikit-learn (want to practice)
- TensorFlow (want to practice)

## Online Machine Learning
![alt text](/assert/Olinelearning.png)

Here the model is trained side by side while running on the server by small batches of data.

The model is first trained with some basic data and evaluated, then deployed on the server. Whenever new data is generated, it is given to the model in small batches to keep the model updated in real-time.

**Real-time Example:** YouTube content recommendation system.

### Learning Rate
Learning rate is an important part of online machine learning. It decides at what time period you want to train your model with new data.

### Out-of-Core Learning
If we train the model with a big data set on the server, it requires a lot of resources, so we split the big data set into small batches and train the model on the server.

**Libraries for Online Machine Learning**
- River (want to practice)
- Vowpal Wabbit (want to practice)

