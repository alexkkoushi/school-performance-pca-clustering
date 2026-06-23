# school-performance-pca-clustering
Analysis of school SAT performance using PCA, K-Means clustering, and data visualization.
School Performance Analysis Using PCA and Clustering
Project Overview

This project analyzes school performance using SAT results and the number of test takers. The goal is to explore school performance patterns, reduce the dimensionality of the dataset using Principal Component Analysis (PCA), and group schools into meaningful categories using K-Means clustering.

The project was completed as an academic machine learning assignment and focuses on data preprocessing, exploratory data analysis, PCA, clustering, visualization, and interpretation of results.

Dataset

The dataset contains SAT performance data for schools, including:

Number of SAT test takers
Average reading score
Average mathematics score
Average writing score

The original dataset contained 478 schools. Some missing values were recorded as "s", which were replaced with missing values and removed. After cleaning, 421 schools remained.

Two additional features were created:

Total SAT score
Average SAT score

These features helped represent overall school performance more clearly.

Methods Used

The project includes the following steps:

Data cleaning and preprocessing
Feature creation
Exploratory data analysis
Standardization using StandardScaler
Principal Component Analysis
K-Means clustering
Cluster evaluation using silhouette score
Interpretation of clusters for decision-making
Exploratory Data Analysis

The analysis showed that most schools had total SAT scores between 1000 and 1300. The average total SAT score was around 1208.

Schools were also divided into above-average and below-average groups:

145 schools were above average
276 schools were below average

School size was also analyzed using the number of SAT test takers.

PCA

PCA was used to reduce the number of variables and simplify the dataset. Before applying PCA, the data was standardized using StandardScaler so that all variables contributed equally.

PCA helped represent the schools in a lower-dimensional space and made the clustering results easier to visualize and interpret.

Clustering

K-Means clustering was applied to group schools based on SAT performance and school size.

The final model included both school performance and number of test takers, making the clustering more useful for decision-making.

The final clusters were interpreted as:

Low-performing, small schools
Medium-performing schools
High-performing, large schools

The final clustering model achieved a silhouette score of approximately 0.51, indicating a reasonable separation between clusters.

Main Insights

The analysis showed that school size alone does not fully explain school performance. However, combining school size with SAT performance provides more meaningful groups.

The final clustering model can help identify which schools may need more support. For example, large low-performing schools may be a higher priority because improving them can affect more students.

Limitations

This project was completed as an academic learning project and has some limitations:

Only a limited number of features were available.
More socioeconomic or school-level features could improve the analysis.
K-Means requires choosing the number of clusters manually.
More clustering algorithms could be tested for comparison.
More advanced validation methods could be used to evaluate the clusters.
The interpretation of clusters depends on the available data and should not be used alone for real policy decisions.
Future Improvements

If I were to improve this project, I would:

Add more features such as school location, funding, teacher-student ratio, and socioeconomic indicators.
Compare K-Means with other clustering methods.
Use the elbow method and silhouette analysis to better justify the number of clusters.
Compare clustering results with and without PCA.
Improve the visualizations and add more detailed cluster profiles.
Build an interactive dashboard to present the results more clearly.
What I Learned

This project helped me understand how PCA can simplify a dataset while preserving important information. It also showed me how clustering can be used not only to group data points, but also to support decision-making.

Through this project, I practiced data cleaning, feature creation, standardization, PCA, K-Means clustering, silhouette score evaluation, visualization, and interpretation of machine learning results.

Technologies Used
Python
pandas
NumPy
matplotlib
scikit-learn
StandardScaler
PCA
K-Means
Silhouette Score
Jupyter Notebook
