🧠 What is KNN?

    -K-Nearest Neighbors is a supervised, distance-based machine learning algorithm.

For a new data point:

    -Compute distance to all training points
    -Select the K closest neighbors
    -Perform majority voting
    -Assign the most common class

📊 Dataset Used

    -Iris Dataset from sklearn.datasets:
    -150 samples
    -3 classes
    -4 features: Sepal length, Sepal width, Petal length, Petal width

⚙️ Pre-processing
🔹 Feature Scaling
    -StandardScaler is used before applying KNN.
    Why?
    KNN relies on distance calculations. If features have different ranges, larger-scale features dominate.


✅ Implementation 1: Using Scikit-Learn

                    Steps:

                    - Load dataset
                    - Convert to DataFrame
                    - Train-test split
                    - Apply StandardScaler
                    - Train KNN classifier
                    - Predict on test set
                    - Evaluate using:
                    - Accuracy
                    - Precision
                    - Confusion Matrix

✅ Implementation 2: KNN From Scratch

                      Implemented manually:

                    - Euclidean distance function
                    - Loop over test points
                    - Compute distance to all training points
                    - Sort neighbors
                    - Select top K
                    - Majority voting using Counter
                    - Evaluate accuracy
                    - Try multiple values of K

🧪 Testing Different K Values

    Odd values of K were tested to avoid ties: K = 1, 3, 5, 7, 9


All achieved high accuracy due to: Clean dataset, Well separated classes, Proper scaling

📈 Evaluation Metrics: Accuracy Score, Precision Score (weighted), Confusion Matrix

🧾 Key Learnings

    ✔ How distance-based algorithms work
    ✔ Why scaling is critical
    ✔ How majority voting is implemented
    ✔ How K affects model behavior
    ✔ Difference between library vs scratch implementation
    ✔ Computational cost of KNN

    ⚠️ Time Complexity

        - For each test point:
        - Distance calculation → O(n × d)
        - Sorting → O(n log n)
        - This makes KNN expensive for very large datasets.