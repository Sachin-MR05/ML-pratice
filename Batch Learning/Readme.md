# Batch Learning

## Offline Machine Learning
It means training the model with the entire data set we have on the local machine, testing the model, and updating it on the server.

**Example**  
A movie recommendation website trained with user data from daily watch history.

**Problem**  
Because the data is big, we can train the model on the server. If we want to update the model with the user's next day watch history data, we need to pull the model, train it with the new + old data, test it, and push it back to the server.

![alt text](assert/BatchLearning.png)

**Disadvantages**
- The data doubles or triples every time we repeat the process.
- Hardware resources are not available everywhere to download the app trained with the new data every time after updation.
- There is a gap in updating the model with data. In the processing time period, users will use the same old model.

## Online Machine Learning

