Machine Learning Quick Overview
1. What is Machine Learning and When is it Useful?

Machine Learning (ML) is a field of AI that allows systems to learn patterns from data and make predictions or decisions without being explicitly programmed.

Useful when rules are too complex to program manually, like:

Speech recognition

Fraud detection

Recommendation systems

2. AI vs ML vs DL

Artificial Intelligence (AI): Broad concept of machines mimicking human intelligence.

Machine Learning (ML): Subset of AI that learns patterns from data.

Deep Learning (DL): Subset of ML using neural networks with many layers.

3. Types of ML

Supervised Learning → Data has both input and output (answers are known).
Example: Predicting house prices from size and location.

Unsupervised Learning → Data has only input (no answers). The goal is to find patterns.
Example: Grouping customers by buying habits.

Reinforcement Learning → An agent learns by trial and error.
Example: Training a robot to walk.

Semi-Supervised Learning

A mix of labeled and unlabeled data.
Example: Few labeled medical images + many unlabeled ones.

More Types of Unsupervised Learning

Clustering → Grouping similar data points.

Dimensionality Reduction → Reduce features while keeping information.

Anomaly Detection → Detecting unusual events (e.g., fraud).

Association Rule Learning → Finding relationships (e.g., bread → butter).

4. Batch Learning vs Online Learning

Batch Learning: Train on the full dataset at once.

Online Learning: Learn continuously as new data arrives.

5. Instance-Based vs Model-Based Learning

Instance-Based: Memorizes examples, compares new ones (e.g., KNN).

Model-Based: Builds a general model (e.g., Linear Regression).

6. Challenges in ML

Poor quality or insufficient data

Overfitting / Underfitting

Data bias and fairness issues

Scalability and computation limits

7. Applications of ML

Healthcare → disease prediction

Finance → fraud detection, stock prediction

Retail → recommendation engines

Autonomous vehicles → self-driving cars

NLP → chatbots, translations

8. Machine Learning Development Lifecycle

Define the problem

Collect and prepare data

Exploratory Data Analysis (EDA)

Feature engineering

Model training

Model evaluation

Deployment

Monitoring and improvement

9. ML Engineer vs Data Analyst vs Data Scientist

Data Analyst: Analyzes and visualizes data.

Data Scientist: Builds models and applies ML.

ML Engineer: Deploys and scales ML in production.

10. Tensors

Tensors = multi-dimensional arrays used in deep learning (TensorFlow, PyTorch).

0D: Scalar → 2

1D: Vector → [1, 2, 3]

2D: Matrix → [[1, 8], [2, 4]]

3D: RGB image → (H, W, C)

4D: Batch of images → (N, H, W, C)

5D: Video → (N, T, H, W, C)

11. End-to-End Example (Overview)

Frame the problem (predict house prices).

Collect data (CSV, SQL, APIs).

Clean & preprocess data.

Perform EDA.

Train model.

Evaluate accuracy.

Deploy model.

12. Framing a Problem

Clearly define:

Input data

Output predictions

Evaluation metrics

13. Data Gathering

CSV Files → load with pandas

JSON Files → structured data

SQL Databases → query with SQL

APIs → fetch live data

Web Scraping → extract from websites

14. Understanding Your Data

Check for:

Missing values

Duplicates

Data types

Distributions

15. Exploratory Data Analysis (EDA)

Univariate Analysis → histograms, bar plots

Bivariate Analysis → scatter plots, correlations

Multivariate Analysis → pair plots, heatmaps

Pandas Profiling → automated EDA report

16. Feature Engineering

Feature Engineering = transforming raw data into meaningful features that improve ML performance.

Why Important?

Boosts model accuracy

Handles missing/noisy data

Improves generalization

Highlights useful patterns

Techniques

Handling missing data

Feature creation (e.g., BMI)

Feature transformation (log, binning, polynomials)

Feature scaling (see next section)

17. Feature Scaling

Different features can have very different ranges (e.g., income = 1000–100000 vs age = 18–70).

Why Scaling Matters

Prevents dominance of large-value features

Improves convergence (gradient descent)

Helps distance-based algorithms (KNN, clustering)

Types of Scaling

Normalization (Min-Max Scaling)

Scales values between 0–1.

Formula:

X' = (X - Xmin) / (Xmax - Xmin)


Best for bounded data (e.g., Neural Nets).

Standardization (Z-score Scaling)

Mean = 0, Std Dev = 1.

Formula:

X' = (X - μ) / σ


Best when data is Gaussian.

Robust Scaling

Uses median + IQR (less sensitive to outliers).

MaxAbs Scaling

Scales between -1 and 1 (good for sparse data).

18. Encoding Categorical Data

ML models require numeric input, not text.

Types of Categorical Data

Nominal: No order (e.g., colors, countries).

Ordinal: Ordered categories (e.g., education level).

Encoding Techniques

One-Hot Encoding (Nominal)

Red, Green, Blue → [1,0,0], [0,1,0], [0,0,1]

Works well but increases dimensions.

Ordinal Encoding (Ordinal)

Education → School = 0, UG = 1, PG = 2

Preserves order but assumes equal spacing.

Label Encoding

Red = 0, Green = 1, Blue = 2

 Misleading for nominal data (model may assume order).

Target / Mean Encoding

Replaces category with mean of target variable.

Example: "Location = CityA" → average house price in CityA.
