<p align="center">
  <img src="https://github.com/user-attachments/assets/0dca38f5-383f-4cb6-b982-3a9b99b2bd36" alt="Unsupervised Learning" width="700">
</p>

<h1 align="center">AMSS 2025 Module 4 | Unsupervised Learning</h1>

## Introduction

This session on **unsupervised learning** explains the main concepts, techniques, and uses. The speakers cover clustering, dimensionality reduction, generative models, and representation learning, showing how these are applied in real-world data analysis.

## Overview of Unsupervised Learning

- **Definition**: Learning from data without labels to find hidden patterns or structures.
- **Difference from Supervised Learning**: No target labels are given. The model finds patterns on its own.
- **Importance**:
  - Works with large amounts of unlabeled data.
  - Finds useful insights without needing manual labeling.
  - Used in areas like anomaly detection and image super-resolution.

## Core Problems in Unsupervised Learning

| Problem Type | Description | Examples |
|--------------|-------------|----------|
| Dimensionality Reduction | Reduce data size while keeping important information | Visualization, compression, feature extraction |
| Clustering | Group similar data points together | Customer segmentation, image grouping |
| Generative Modeling | Learn the data pattern to make new data | Image synthesis, anomaly detection |
| Representation Learning | Create compact and useful data forms for later tasks | Word embeddings, image features |

## Dimensionality Reduction

- **Goal**: Make data easier to work with and faster to process.
- **Technique**: **Principal Component Analysis (PCA)** finds directions that capture the most variation.
- **Example**: Compressing images by keeping only important components to save space and speed up processing.

## Clustering

- **Goal**: Group similar items and separate different ones.
- **Methods**:
  - **K-means**: Groups data based on closest center points.
  - **Hierarchical Clustering**: Connects items based on closeness.
  - **Gaussian Mixture Models**: Uses probabilities to assign items to groups.
- **Example**: Image compression by grouping pixel colors into a few main clusters.

## Generative Modeling

- **Goal**: Learn the structure of data and create new examples.
- **Methods**:
  - **Density Estimation**: Models like Gaussian mixtures.
  - **GANs**: A generator makes data and a discriminator checks if it is real or fake.
- **Uses**: Image enhancement, style changes, and creating realistic images from scratch.

## Representation Learning

- **Goal**: Build simple and meaningful representations of data.
- **Examples**:
  - **Text**: Word embeddings like Word2Vec and BERT.
  - **Graphs**: Node embeddings using methods like DeepWalk.
  - **Images**: Self-supervised methods like SimCLR.

## Graph Representation Learning

- **DeepWalk**: Random walks on a graph to learn node relationships.
- **Node2Vec**: Improved walks to balance local and global structure.
- **Uses**: Social networks, recommendations, and anomaly detection.

## Self-Supervised Contrastive Learning

- **Goal**: Learn without labels by comparing different views of the same data.
- **Method (SimCLR)**:
  - Make two changed versions of the same image.
  - Train the model to keep them close and push away different images.
- **Benefits**: Less data labeling needed and works well in many tasks.

## Conclusion

Unsupervised learning helps find value in unlabeled data for images, text, and graphs. Methods like clustering, dimensionality reduction, generative models, and embeddings are key skills for modern data science. Advances like GANs, transformers, and contrastive learning make these methods even more powerful.

> In this session, students explored machine learning and deep learning with practical use of TensorFlow and Keras. They practiced core ideas like regression, classification, clustering, and dimensionality reduction, while also working with models such as SVMs, Decision Trees, and Ensemble methods. The session further introduced advanced neural networks, training methods, and how to deploy models for real applications.
