Eco Bank Customer Churn Prediction (ANN)

Eco Bank has observed an increasing trend of customers leaving the bank (churning) over the past six months. To address this, this project involves building a Geodemographic Segmentation Model using an Artificial Neural Network (ANN). The goal is to predict which customers are at the highest risk of leaving the bank so that proactive retention strategies can be implemented.

Dataset Description
The bank collected data on 10,000 customers. The dataset contains the following attributes:

Independent Variables:

CreditScore: The customer's credit score.

Geography: The customer’s location (France, Spain, or Germany).

Gender: Male or Female.

Age: Customer age.

Tenure: Number of years the customer has been with the bank.

Balance: Account balance.

NumOfProducts: Number of bank products the customer uses.

HasCrCard: Whether the customer has a credit card (1 = Yes, 0 = No).

IsActiveMember: Whether the customer is an active member (1 = Yes, 0 = No).

EstimatedSalary: Customer's estimated annual salary.


Dependent Variable:

Exited: Whether the customer left the bank (1 = Yes, 0 = No).

Technical Stack
Language: Python

Libraries: - NumPy & Pandas (Data Manipulation)

Scikit-Learn (Preprocessing & Evaluation)

TensorFlow / Keras (Deep Learning)

Implementation Steps

Data Preprocessing

Data preprocessing is the most critical step to ensure the ANN can process the information correctly.

Variable Selection: Removed non-predictive columns (RowNumber, CustomerId, Surname).

Encoding Categorical Data:

Label Encoding: Converted the "Gender" column into binary (0 and 1).

One-Hot Encoding: Converted the "Geography" column into dummy variables to avoid ordinal ranking among countries.

Splitting: Divided the data into an 80% Training set and a 20% Test set.

Feature Scaling: Applied StandardScaler to all features. This is mandatory in Deep Learning to prevent features with larger scales from dominating the model training.

Building the ANN
The model is a Sequential neural network consisting of:

Input Layer: Takes the processed customer features.

Hidden Layer 1: 6 neurons with the ReLU activation function.

Hidden Layer 2: 6 neurons with the ReLU activation function.

Output Layer: 1 neuron with the Sigmoid activation function (perfect for binary classification, as it provides the probability of churn).

3. Training the Model
Optimizer: Adam (Stochastic Gradient Descent method).

Loss Function: binary_crossentropy (Required for binary classification).

Epochs: 100

Batch Size: 32

4. Model Evaluation
After 100 epochs, the model reached a training accuracy of approximately 87%.

Confusion Matrix Results:

True Negatives (Stayed): 1505

True Positives (Left): 213

Accuracy Score: 85.9%

Predictive Example
We tested the model with a sample customer:

Location: France

Credit Score: 600

Gender: Male

Age: 40

Tenure: 3 years

Balance: $60,000

Products: 2

Has Credit Card: Yes

Active Member: Yes

Salary: $50,000

Result: The model predicted False, meaning this specific customer is likely to stay with Eco Bank.

Conclusion
The ANN model provides a robust way for Eco Bank to identify at-risk customers with ~86% accuracy. By focusing on these specific individuals, the bank can offer personalized incentives to reduce churn and increase customer lifetime value.
