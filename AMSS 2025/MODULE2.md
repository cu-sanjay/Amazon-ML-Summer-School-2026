<p align="center">
  <img src="https://github.com/user-attachments/assets/a5687be1-c2cc-4c79-a944-5976d48d017c" alt="Deep Neural Networks and Sequence Models" width="700">
</p>
<h1 align="center">AMSS 2025 Module 2</h1>

## Summary of Deep Neural Networks and Sequence Models Lecture

## Introduction

This summary explains key points from the second session of Amazon India Machine Learning Summer School. It focuses on deep neural networks, convolutional neural networks and recurrent neural networks. It covers core ideas, history, model designs, training methods and uses. The goal is a clear view of modern deep learning methods.

## Deep Neural Networks: Foundations and Evolution

### Historical Context
* Early AI used hand crafted rules like edge detectors for images. These needed a lot of manual tuning and were not flexible.
* Neural networks moved to learning features from data. For example CNNs use local receptive fields and learn patterns from nearby pixels.
* Over time systems moved from fixed priors to learned features. Models started to extract complex patterns on their own.

### Core Concepts
* Single layer and multi layer perceptrons have inputs, weights, biases, activation functions and outputs.
* Training uses gradient descent and backpropagation to reduce loss.
* Activation functions include sigmoid, ReLU and leaky ReLU. Choice affects speed and stability.
* Code examples in PyTorch show how to build and train networks with automatic differentiation.

### Why Deep Learning Took Off
* Large data became available from the web and other sources.
* GPUs made matrix operations fast and training practical.
* Error rates in vision tasks dropped a lot over the last decade.

## Convolutional Neural Networks

### Applications
* Face detection, object recognition, visual recommendation and defect detection.
* CNNs work well when data has spatial structure.

### Why CNNs Are Needed
* Limits of basic perceptrons on images
  * Parameter count becomes huge for large images.
  * Flattening images loses spatial structure.
* CNN advantages
  * Local receptive fields with shared weights.
  * Translation invariance.
  * Hierarchical features from edges to textures to objects.

### Architecture and Components

<table>
  <thead>
    <tr>
      <th>Layer</th>
      <th>Function</th>
      <th>Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Convolution</td>
      <td>Extracts local features with sliding filters</td>
      <td>Common sizes 3x3 and 5x5, learned during training</td>
    </tr>
    <tr>
      <td>ReLU</td>
      <td>Adds nonlinearity</td>
      <td>Helps faster training and reduces vanishing gradients</td>
    </tr>
    <tr>
      <td>Pooling</td>
      <td>Reduces spatial size and adds small shift invariance</td>
      <td>Max pool 2x2 with stride 2 is common</td>
    </tr>
    <tr>
      <td>Fully Connected</td>
      <td>Combines features for final decisions</td>
      <td>Connects flattened features to outputs</td>
    </tr>
    <tr>
      <td>Softmax</td>
      <td>Converts scores to probabilities</td>
      <td>Used for classification</td>
    </tr>
  </tbody>
</table>

### Key Insights
* Early layers learn edges and colors. Deeper layers learn shapes and objects.
* Known designs include AlexNet, GoogleNet with inception blocks, ResNet with residual links and DenseNet.
* Training tips include data augmentation, good init, regularization like dropout and optimizers like Adam and Momentum.

## Recurrent Neural Networks

### Purpose and Applications
* Used for speech, translation, sentiment analysis, caption generation and video tasks.
* Handle sequential data where order of inputs matters.

### Core Principles
* Keep a memory or state to carry past information.
* For each time step there is an input, a hidden state and an output.
* Feedback links pass context across time.

### Challenges and Solutions

<table>
  <thead>
    <tr>
      <th>Issue</th>
      <th>Explanation</th>
      <th>Mitigation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Vanishing gradient</td>
      <td>Gradients shrink for long sequences</td>
      <td>LSTM with gates, residual links, attention</td>
    </tr>
    <tr>
      <td>Forgetfulness</td>
      <td>Difficult to keep long term context</td>
      <td>LSTM forget gate and memory cell</td>
    </tr>
    <tr>
      <td>Long term dependency</td>
      <td>Early context is lost with long inputs</td>
      <td>LSTM, bidirectional RNNs, transformers with attention</td>
    </tr>
  </tbody>
</table>

### LSTM and Bidirectional RNNs
* LSTM has input, forget and output gates with a memory cell to keep useful information.
* Bidirectional RNNs read sequences forward and backward to use both contexts.
* Attention allows the model to look back at all past states and pick what matters.

### Training and Implementation
* Backpropagation through time extends backpropagation to sequences.
* PyTorch and TensorFlow handle gradients automatically.
* Common tasks include word prediction, sentiment analysis and translation.

## Practical Insights and Future Directions
* Good data often beats complex models. Clean and relevant data helps a lot.
* Transfer learning uses large pre trained models such as BERT and RoBERTa and then fine tunes for tasks.
* Transformers use self attention to handle long context and often replace recurrence for text tasks.
* Pick simple RNNs for short sequences and LSTM or transformers for long ones.
* Regularization like dropout and batch norm with strong optimizers improves results.

## Conclusion

This session explained the core building blocks and where each model fits.
* MLPs are basic units for many tasks.
* CNNs handle spatial data and reduce parameter explosion while keeping structure.
* RNNs and LSTMs work for sequences and manage long term effects.
* Transformers with attention are the recent advance and power many modern models.

>[!IMPORTANT]
> In this session, students will analyze the Titanic passenger dataset to uncover patterns that influenced survival in the historic disaster. This exercise combines exploratory data analysis (EDA) with machine learning—allowing you to build predictive models that determine survival outcomes based on features such as age, gender, passenger class, fare, and family relationships. You may use this [Titanic dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset?select=Titanic-Dataset.csv) or another dataset of your choice. Use Jupyter Notebook to apply your EDA skills and build your predictive model in an interactive and exploratory way.

