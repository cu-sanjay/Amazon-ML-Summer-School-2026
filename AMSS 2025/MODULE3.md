<p align="center">
  <img src="https://github.com/user-attachments/assets/71aeeadb-f242-442e-8642-fdbbd2801d5e" alt="Dimensionality Reduction" width="700">
</p>

<h1 align="center">AMSS 2025 Module 3</h1>

## Introduction

This summary explains the main concepts from the lecture on dimensionality reduction in machine learning. It covers why these methods are important, how they work, and where they are applied. Key methods include feature selection, feature extraction, singular value decomposition, principal component analysis, matrix factorization, and autoencoders. These help in handling high dimensional data, improving model understanding, reducing computation, and finding hidden structures.

## The Challenge of High Dimensional Data

* Large datasets with many features are common in supervised learning.
* Text and categorical data can create huge feature spaces such as bag of words with hundreds of thousands of features.
* Models can suffer from overfitting, slow training, and low interpretability.
* Goal is to reduce feature space while keeping important information.

## Approaches to Dimensionality Reduction

| Method | Description | Use Cases | Benefits |
| --- | --- | --- | --- |
| Feature Selection | Choose a subset of original features | When interpretability or cost limits exist | Improves accuracy, faster predictions |
| Feature Extraction | Create new features from old ones | When data is complex | Finds structure, reduces noise |
| Representation Learning | Learn embeddings with neural networks | Large scale, complex data | Flexible and powerful, pre trained models available |

## Feature Selection Techniques

* Wrapper Methods use models to test feature subsets. They can be accurate but slow for large sets.
* Filter Methods use statistical scores like mutual information or correlation to rank features. They are fast but ignore interactions.
* Embedded Methods like Lasso select features during training. They balance speed and interpretability.

## Feature Extraction Techniques

* Principal Component Analysis uses singular value decomposition to find directions of maximum variance and project data with minimum loss. Works for image compression, noise reduction, and visualisation.
* Singular Value Decomposition splits a matrix into U, S, and V transpose to reveal hidden patterns such as in text or recommendation data.
* Matrix Factorization works on incomplete data such as user item ratings and finds hidden factors for recommendations.

## Advanced Techniques

* Autoencoders are neural networks that compress and then reconstruct data. They help in complex high dimensional cases like images and text.
* Non negative Matrix Factorization forces factors to be non negative for easy interpretation. Useful for topics in text and features in images.

## Applications

* Recommendation Systems place users and products in the same low dimensional space to match preferences.
* Genomics visualises gene data in 2D or 3D to study ancestry or expression.
* Image and Voice Recognition reduces data for faster and more accurate classification.
* Text Analysis extracts topics from documents using NMF or latent semantic analysis.
* Facial Recognition simplifies images for faster and efficient matching.

## Conclusion

Dimensionality reduction is key for efficient and understandable models. PCA, SVD, matrix factorization, and autoencoders help to find structure, improve speed, and understand data. These methods work across recommendation, image, text, and many other domains. A strong understanding of basic linear algebra like eigenvalues and matrix decomposition supports deeper learning in this area.

> In this session, students were taught the basics of dimensionality reduction and practiced live on datasets using techniques like PCA and t-SNE. The session also connected these ideas with neural networks such as CNNs, RNNs, and other deep learning architectures, showing how reducing dimensions helps in regression, classification, and clustering tasks. Students were encouraged to experiment hands-on and apply these methods in Jupyter Notebook.
