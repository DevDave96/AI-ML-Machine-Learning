**The Machine Learning Master Project: From Energy to Healthcare**

Welcome to my Machine Learning portfolio! This repository contains a collection of end-to-end data science projects. I have explored both Regression (predicting numbers) and Classification (predicting categories) using real-world datasets.


**Executive Summary**

In this journey, I acted as a Lead Data Scientist across three different industries:

Energy Sector: Predicting Power Plant output.

Automotive Industry: Predicting SUV buyer behavior.

Healthcare: Diagnosing Breast Cancer.


**Project 1: Power Plant Energy Prediction (Regression)**

The Mission: Predict the net hourly electrical energy output of a power plant based on environmental factors like Temperature, Humidity, and Pressure.

Models Tested: Linear Regression, Polynomial Regression, Support Vector Regression (SVR), Decision Tree, and Random Forest.

The Winner: Random Forest Regressor.

What I Achieved: By using an "ensemble" of 100 decision trees, I was able to predict energy output with incredible precision, helping power grid managers plan for demand.

Layman's Lesson: I learned that many small guesses (trees) averaged together are better than one single big guess.


**Project 2: The SUV Launch Campaign (Classification)**

The Mission: A car company is launching a new luxury SUV. I had to predict which customers would actually buy it based on their Age and Salary.

Models Tested: Logistic Regression, K-NN, SVM, Kernel SVM, Naive Bayes, Decision Tree, and Random Forest.

The Insight: Using Feature Scaling, I ensured that a $100,000 salary didn't "outweigh" a 45-year-old age in the eyes of the computer.

What I Achieved: I created a "Heat Map" of customer behavior, showing that the sweet spot for the SUV was older, high-earning individuals, allowing the marketing team to save money on ads.

Layman's Lesson: Some models draw straight lines to separate people, while others (like Kernel SVM) draw circles to find hidden groups.


**Project 3: Breast Cancer Diagnosis (The Mission for Safety)**

The Mission: Classify tumors as Benign (Safe) or Malignant (Cancerous) using clinical data.

🏆 **The Clinical Leaderboard**

I compared my models not just on accuracy, but on Safety (how many sick people did we miss?).

🥇 **Kernel SVM (The Best Overall)**

Accuracy: 95.3%

Missed Cases (False Negatives): 3

The Verdict: This was the most balanced model. It achieved the highest accuracy while keeping missed cases extremely low, making it the most reliable tool for a doctor’s daily use.

🛡️ **Naive Bayes (The Safety First)**

Accuracy: 94.2%

Missed Cases (False Negatives): 2

The Verdict: While its overall score was slightly lower, this model was the "safest." It caught almost every single cancer case, missing only 2. In healthcare, this high sensitivity is often the top priority.

⚡ **K-NN & Logistic Regression (The Fast Baseline)**

Accuracy: 94.7%

Missed Cases (False Negatives): 5

The Verdict: These models are incredibly fast and easy to explain. They serve as a perfect "second opinion" to double-check results from more complex systems.

🌲 **Random Forest (The Complex Choice)**

Accuracy: 93.6%

Missed Cases (False Negatives): 6

The Verdict: Usually a powerhouse, the Random Forest was slightly less sensitive on this specific dataset. It showed that sometimes simpler, math-based models can outperform complex "forests" in clinical settings.

**What I Achieved**: I prioritized the Confusion Matrix over simple accuracy. I learned that in medicine, it is better to have a "False Alarm" than to miss a single sick patient.

**Layman's Lesson**: The Naive Bayes model is like a very cautious doctor—it might be a bit more worried than others, but it rarely misses a problem.
