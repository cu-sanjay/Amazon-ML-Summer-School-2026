<p align="center">
  <img src="https://github.com/user-attachments/assets/09f4140a-0bfd-42ff-a359-446689218926" alt="Course Banner" width="700">
</p>

<h1 align="center">AMSS 2025 Module 6</h1>

# Hidden Markov Models and Sequential Learning

## Introduction
This summary covers the core concepts of Hidden Markov Models (HMMs) and recent advances in sequential learning, including attention mechanisms, Transformers, subword modeling, and pre-training strategies. The goal is to distill complex topics into clear, structured insights, emphasizing their applications in natural language processing (NLP) and speech recognition.

## Hidden Markov Models (HMMs): Foundations and Applications

### Overview
- HMMs are generative models used for sequential data, modeling the joint distribution of observed sequences and hidden states.  
- Main tasks:  
  - Inference: find the most probable hidden state sequence.  
  - Likelihood computation: calculate the probability of observed data.  
  - Training: learn initial, transition, and emission probabilities.  

### Application Example: Part-of-Speech Tagging
- Classifies words into categories (noun, verb, etc.).  
- Words are ambiguous, so context is essential.  
- Generative modeling approach with algorithms like Viterbi for decoding.  

### Model Components

- **States**  
Hidden tags \( Y \)  

- **Observations**  
Words in sequence \( X \)  

- **Initial Probabilities**  
Starting distribution ( π )  

- **Transition probabilities**

$$
  a_{ij} = P\big(Y_t = j \mid Y_{t-1} = i\big)
$$

- **Emission probabilities**

$$
  b_j(x) = P\big(X_t = x \mid Y_t = j\big)
$$
  

### Inference and Training
- Viterbi algorithm for most likely sequence.  
- Forward and backward algorithms for efficient likelihood.  
- Supervised training uses labeled data.  
- EM algorithm handles unlabeled data in semi-supervised settings.  

## Modern Sequential Learning: Attention, Transformers, and Pre-training

### Attention Mechanisms
- Focus on relevant parts of input sequences dynamically.  
- Compute relevance scores and weight context accordingly.  
- Types: additive (Bahdanau), scaled dot-product.  

### Transformers
- Encoder-decoder layers with self-attention.  
- Multi-head attention captures diverse relationships.  
- Positional encoding provides order information.  
- Advantages: better long-range modeling and parallelization compared to RNNs.  

### Subword Modeling
- Break words into smaller units to reduce vocabulary size.  
- Techniques: Byte Pair Encoding (BPE), WordPiece, Unigram models.  
- Helps with rare words and unseen tokens.  

### Pre-training Strategies
- Decoder pre-training (GPT): predicts next word.  
- Encoder pre-training (BERT): masked language modeling.  
- Unified models (T5): text-to-text training with span corruption.  

## Conclusion
- HMMs are still useful for foundational sequence tasks like speech recognition.  
- Attention and Transformers revolutionized sequence modeling by removing strict Markov assumptions.  
- Subword modeling and large-scale pre-training improved flexibility and robustness.  
- These ideas power modern NLP systems such as translation, summarization, and chatbots.  

> Sequential learning has evolved from probabilistic models like HMMs to deep architectures like Transformers. This shift enabled handling long-range dependencies, scaling to large data, and building practical applications in language and speech technologies.
