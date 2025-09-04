# Machine Learning Quick Overview

## 1. What is Machine Learning and When is it Useful?

Machine Learning (ML) is a field of AI that allows systems to learn
patterns from data and make predictions or decisions without being
explicitly programmed.
It is useful when rules are too complex to program manually, like speech
recognition, fraud detection, or recommendation systems.

------------------------------------------------------------------------

## 2. AI vs ML vs DL

-   **Artificial Intelligence (AI):** Broad concept of machines
    mimicking human intelligence.
-   **Machine Learning (ML):** Subset of AI that learns patterns from
    data.
-   **Deep Learning (DL):** Subset of ML using neural networks with many
    layers.

------------------------------------------------------------------------
## 3. Types of ML

- **Supervised Learning** → The data has both input and output (answers are known).  
  Example: Predicting house prices from size and location.  

- **Unsupervised Learning** → The data has only input (no answers). The goal is to find patterns.  
  Example: Grouping customers by buying habits.  

- **Reinforcement Learning** → A computer program (agent) learns by trial and error.  
  It gets rewards for good actions and penalties for bad ones.  
  Example: Training a robot to walk.  

### Semi-Supervised Learning
A mix of labeled and unlabeled data.  
Example: Having a small amount of medical images with labels (disease type) and a large set without labels.  

### More Types of Unsupervised Learning
- **Clustering** → Grouping similar data points together.  
  Example: Grouping news articles by topic.  

- **Dimensionality Reduction** → Making data smaller by reducing features but keeping important information.  
  Example: Compressing image data while keeping quality.  

- **Anomaly Detection** → Finding unusual or rare data points.  
  Example: Detecting credit card fraud.  

- **Association Rule Learning** → Finding relationships between items.  
  Example: People who buy bread often buy butter.  



------------------------------------------------------------------------

## 4. Batch Learning vs Online Learning

-   **Batch Learning:** Model is trained on the entire dataset at once.
-   **Online Learning:** Model learns continuously as new data arrives.

------------------------------------------------------------------------

## 5. Instance-Based vs Model-Based Learning

-   **Instance-Based:** Memorizes examples and compares new cases (e.g.,
    KNN).
-   **Model-Based:** Builds a general model to make predictions (e.g.,
    linear regression).

------------------------------------------------------------------------

## 6. Challenges in ML

-   Poor quality or insufficient data
-   Overfitting/Underfitting
-   Data bias and fairness
-   Scalability and computation power

------------------------------------------------------------------------

## 7. Applications of ML

-   Healthcare (disease prediction)
-   Finance (fraud detection, stock prediction)
-   Retail (recommendation engines)
-   Self-driving cars
-   Natural Language Processing (chatbots, translations)

------------------------------------------------------------------------

## 8. Machine Learning Development Lifecycle

1.  Define the problem
2.  Collect and prepare data
3.  Exploratory Data Analysis (EDA)
4.  Feature engineering
5.  Model training
6.  Model evaluation
7.  Deployment
8.  Monitoring and improvement

------------------------------------------------------------------------

## 9. ML Engineer vs Data Analyst vs Data Scientist

-   **Data Analyst:** Focuses on analyzing and visualizing data.
-   **Data Scientist:** Builds models, does research, applies ML
    techniques.
-   **ML Engineer:** Deploys, scales, and optimizes ML models for
    production.

------------------------------------------------------------------------

## 10. Tensors

Tensors are multi-dimensional arrays used in deep learning frameworks
like TensorFlow and PyTorch.

-   0D: Scalar → 2
-   1D: Vector → [1,2,3]
-   2D: Matrix → [[1,8],[2,4]]
-   3D: RGB image → (H, W, C)
-   4D: Batch of images → (N, H, W, C)
-   5D: Video → (N, T, H, W, C)

------------------------------------------------------------------------

## 11. End-to-End Example (Overview)

1.  Frame the problem (predict house prices).
2.  Collect data (CSV, SQL, APIs).
3.  Clean and preprocess data.
4.  Perform EDA.
5.  Train a model.
6.  Evaluate accuracy.
7.  Deploy the model.

------------------------------------------------------------------------

## 12. Framing a Problem

Define input data, output predictions, and evaluation metrics.

------------------------------------------------------------------------

## 13. Data Gathering

-   **CSV Files** → Load with pandas.
-   **JSON Files** → Load structured data.
-   **SQL Databases** → Query data using SQL.
-   **APIs** → Fetch live data.
-   **Web Scraping** → Extract data from websites.

------------------------------------------------------------------------

## 14. Understanding Your Data

Check missing values, duplicates, data types, and distributions.

------------------------------------------------------------------------

## 15. Exploratory Data Analysis (EDA)

-   **Univariate Analysis:** Single variable (histograms, bar plots).
-   **Bivariate Analysis:** Two variables (scatter plots, correlation).
-   **Multivariate Analysis:** Multiple variables (pair plots,
    heatmaps).
-   **Pandas Profiling:** Automated EDA report.

------------------------------------------------------------------------

