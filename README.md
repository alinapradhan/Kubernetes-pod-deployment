Iris Dataset PCA Analysis
This repository contains a Jupyter Notebook (specifically, a Google Colab notebook) that demonstrates a Principal Component Analysis (PCA) on the famous Iris dataset.



This notebook walks through the following steps:

Loading the Iris Dataset: Imports the Iris dataset from sklearn.datasets.

Data Exploration:
Loads the data into a Pandas DataFrame.

Displays the head and tail of the DataFrame.

Adds the 'target' column (species information) to the DataFrame.

Data Preprocessing:
Separates features (X) and target (y).

Applies StandardScaler to normalize the feature data, which is crucial for PCA.

Principal Component Analysis (PCA):

Initializes and applies PCA from sklearn.decomposition to the scaled data.

Examines the pca.components_ (loading scores), pca.explained_variance_, and pca.explained_variance_ratio_.

Calculates the np.cumsum of the explained variance ratio to understand the cumulative variance explained by each principal component.

Transforms the original data into the new principal component space (x_pca).

Adds the 'target' column to the x_pca DataFrame and renames columns for clarity (PC1, PC2, PC3, PC4).

Visualization:

Scree Plot: Generates a scree plot using matplotlib.pyplot to visualize the proportion of explained variance by each principal component. This helps in determining the optimal number of components to retain.

Bar Plot of Explained Variance: Visualizes the explained variance ratio of each component using a bar plot.

Loading Scores: Displays a DataFrame of the PCA components (loading scores) which indicate the correlation between the original features and the new principal components.


Run the Cells: Once opened, you can run each cell sequentially by clicking the "Play" button next to each cell or by going to Runtime -> Run all.

Requirements
The notebook uses standard Python libraries for data science and machine learning, which are readily available in Google Colab:

sklearn (scikit-learn) for dataset loading, preprocessing, and PCA.

pandas for data manipulation.

numpy for numerical operations.

matplotlib for plotting.
