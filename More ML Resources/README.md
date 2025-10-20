<div align="center">
  <h1>🌟 ML-Extras</h1>
  <p><strong>Advanced Machine Learning Resources Beyond the Core Curriculum</strong></p>
  <p>
    A curated repository beyond the Amazon ML Summer School, offering in-depth insights into modern machine learning (ML), deep learning (DL), and large language models (LLMs) for learners, developers, and researchers. Updated with trends and resources as of August 2025.
  </p>

  <!-- Badges -->
  <p>
    <a href="https://img.shields.io/badge/License-MIT-blue.svg"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT"/></a>
    <a href="https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg"><img src="https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg" alt="Contributions Welcome"/></a>
    <a href="https://img.shields.io/badge/Last%20Updated-Aug%202025-blue.svg"><img src="https://img.shields.io/badge/Last%20Updated-Aug%202025-blue.svg" alt="Last Updated: Aug 2025"/></a>
    <a href="https://github.com/cu-sanjay/Amazon-ML-Summer-School-2025"><img src="https://img.shields.io/github/stars/cu-sanjay/Amazon-ML-Summer-School-2025?style=social" alt="GitHub Stars"/></a>
  </p>

  <p>
    <a href="#topics">Topics</a> •
    <a href="#llm-trends">LLM Trends</a> •
    <a href="#resources">Resources</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#license">License</a>
  </p>
</div>

## 🔍 Featured Topics

This section covers foundational and advanced ML/DL topics, including mathematical foundations (with corrected LaTeX syntax), practical resources, and authoritative references.

### 1. Core Machine Learning
Core ML focuses on classical algorithms for regression, classification, clustering, and model evaluation. Key algorithms include linear regression, decision trees, and support vector machines (SVMs). For example, the SVM optimization problem is:

$$
\min_{\mathbf{w}, b} \frac{1}{2} \|\mathbf{w}\|^2 + C \sum_{i=1}^n \xi_i
$$  

subject to  

$$
y_i (\mathbf{w}^T \mathbf{x}_i + b) \geq 1 - \xi_i,
$$  

where $\mathbf{w}$ is the weight vector, $b$ is the bias, $C$ is the regularization parameter, and $\xi_i$ are slack variables.

- **Key Concepts**:
  - Model evaluation metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC.
  - **Cross-validation:** $k$-fold CV to assess model generalization.
  - Hyperparameter tuning: Grid search, random search, Bayesian optimization.

- **Resources**:
  - [Scikit-learn Documentation](https://scikit-learn.org/stable/) – Official documentation for Python’s core ML library.
  - [An Introduction to Statistical Learning](https://www.statlearning.com/) – Book by James et al. (2021).
  - [Model Evaluation Metrics](https://scikit-learn.org/stable/modules/model_evaluation.html) – Scikit-learn’s guide to metrics.
  - [Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow – Géron (2022)](Hands-On%20Machine%20Learning%20with%20Scikit-Learn,%20Keras,%20and%20TensorFlow,%202nd%20Edition.pdf)

### 2. Deep Learning
Deep learning leverages neural networks with multiple layers to model complex patterns. Frameworks like **[PyTorch](https://docs.pytorch.org/docs/stable/index.html)** and **[Fast.ai](https://www.fast.ai/)** simplify implementation.  

For a neural network with weights $\mathbf{W}$, biases $\mathbf{b}$, and activation $\sigma$, the forward pass for a layer is:

$$
\mathbf{z}^{(l)} = \sigma\!\left(\mathbf{W}^{(l)} \mathbf{a}^{(l-1)} + \mathbf{b}^{(l)}\right)
$$

- **Key Concepts**:
  - Convolutional Neural Networks (CNNs): Layers for spatial feature extraction.
  - Optimization: Stochastic Gradient Descent (SGD), Adam optimizer.
  - Regularization: Dropout, batch normalization.

- **Resources**:
  - [Fast.ai: Practical Deep Learning](https://course.fast.ai/) – Free course for practical DL.
  - [PyTorch Documentation](https://pytorch.org/docs/stable/index.html) – Official PyTorch guide.
  - [Deep Learning Book](https://www.deeplearningbook.org/) – Goodfellow et al. (2016).
  - [CS231n: CNNs for Visual Recognition](http://cs231n.stanford.edu/) – Stanford’s CNN course.

### 3. NLP & Large Language Models (LLMs)
**NLP** focuses on processing and generating human language, with LLMs like **BERT** and **GPT-4o** dominating recent advancements.  

The transformer’s self-attention mechanism is:

$$
\text{Attention}(\mathbf{Q}, \mathbf{K}, \mathbf{V}) 
= \text{softmax}\!\left( \frac{\mathbf{Q} \mathbf{K}^T}{\sqrt{d_k}} \right) \mathbf{V}
$$

where $\mathbf{Q}, \mathbf{K}, \mathbf{V}$ are query, key, and value matrices, and $d_k$ is the key dimension.

- **Key Concepts**:
  - Word embeddings: Word2Vec, GloVe, contextual embeddings (BERT).
  - Fine-tuning: Adapting pre-trained LLMs for specific tasks.
  - Instruction tuning: Enhancing LLMs for task-specific performance.

- **Resources**:
  - [Hugging Face Transformers](https://huggingface.co/docs/transformers/index) – Library for NLP and LLMs.
  - [BERT: Pre-training of Deep Bidirectional Transformers](https://arxiv.org/abs/1810.04805) – Devlin et al. (2018).
  - [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) – Visual guide by Jalammar.
  - [CS224n: NLP with Deep Learning](http://web.stanford.edu/class/cs224n/) – Stanford’s NLP course.

### 4. Computer Vision
**Computer vision** involves processing and analyzing visual data using models like **CNNs** and **vision transformers**.  
Transfer learning leverages pre-trained models to improve performance on new tasks.  

For example, a CNN’s convolution operation is:

$$
(f * g)(x, y) = \sum_{m,n} f(m, n)\, g(x-m, y-n)
$$

where $f$ is the input image and $g$ is the kernel.

- **Key Concepts**:
  - Vision models: ResNet, EfficientNet, Vision Transformer (ViT).
  - Transfer learning: Fine-tuning pre-trained models on custom datasets.
  - Object detection: YOLO, Faster R-CNN.

- **Resources**:
  - [ResNet: Deep Residual Learning](https://arxiv.org/abs/1512.03385) – He et al. (2015).
  - [EfficientNet: Rethinking Model Scaling](https://arxiv.org/abs/1905.11946) – Tan & Le (2019).
  - [YOLOv8 Documentation](https://docs.ultralytics.com/yolov8/) – Ultralytics’ object detection framework.
  - [Vision Transformer](https://arxiv.org/abs/2010.11929) – Dosovitskiy et al. (2020).

### 5. Reinforcement Learning
**Reinforcement learning (RL)** trains agents to maximize cumulative rewards through interaction with an environment.  

The value function for a policy $\pi$ is:

```math
V^\pi(s) = \mathbb{E}_\pi\left[\sum_{t=0}^\infty \gamma^t R(s_t, a_t) \mid s_0 = s\right]
```

where $\gamma$ is the discount factor and $R$ is the reward.

- **Key Concepts**:
  - Basics: Markov Decision Processes (MDPs), Q-learning.
  - Agents: Policy gradient methods, Deep Q-Networks (DQNs).
  - Applications: Robotics, game playing, resource management.

- **Resources**:
  - [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book.html) – Sutton & Barto (2018).
  - [David Silver’s RL Course](https://davidstarsilver.wordpress.com/teaching/) | [YT Lectures](https://www.youtube.com/watch?v=2pWv7GOvuf0) – Foundational RL lectures.
  - [Deep RL Bootcamp](https://sites.google.com/view/deep-rl-bootcamp/lectures) – Advanced deep RL.
  - [Stable-Baselines3](https://stable-baselines3.readthedocs.io/) – RL algorithms in PyTorch.

### 6. Causal Inference & Probabilistic Models
**Causal inference** estimates treatment effects, often using the potential outcomes framework.  

The average treatment effect (ATE) is:

$$
\text{ATE} = \mathbb{E}[Y(1) - Y(0)]
$$

where $Y(1)$ and $Y(0)$ are outcomes under treatment and control.

- **Key Concepts**:
  - Causal graphs: Directed Acyclic Graphs (DAGs) for modeling relationships.
  - Probabilistic models: Bayesian networks, Markov random fields.
  - Tools: Pyro, Stan for probabilistic programming.

- **Resources**:
  - [Elements of Causal Inference](https://mitpress.mit.edu/9780262037310/) – Peters et al. (2017).
  - [CS228: Probabilistic Graphical Models](https://cs228.stanford.edu/) – Stanford’s PGM course.
  - [Pyro Documentation](https://pyro.ai/) – Uber AI’s probabilistic programming library.

## 🌐 Recent LLM Trends (2024–2025)

| Model | Developer | Highlights | Reference |
|-------|-----------|------------|-----------|
| **Mixtral 8x7B** | Mistral AI | Sparse Mixture of Experts (MoE) with 8x7B parameters, optimizing efficiency and performance. | [Mistral AI Blog](https://www.superannotate.com/blog/mistral-ai-mixtral-of-experts) |
| **Qwen2 & Qwen3** | Alibaba | Multilingual LLMs with superior reasoning and instruction-following capabilities. | [Qwen GitHub](https://github.com/QwenLM/Qwen3) |
| **Phi-2 / Phi-3** | Microsoft | Small-scale models leveraging synthetic data, outperforming larger models in efficiency. | [Phi-3 Technical Report](https://arxiv.org/abs/2404.14219) |
| **GPT-5** | OpenAI | Multimodal model supporting text, image, and audio with advanced reasoning. | [OpenAI GPT-5 Announcement](https://openai.com/index/introducing-gpt-5/) |
| **Chain-of-Model** | Various | Compositional workflows integrating specialized models for complex tasks. | [arXiv:2502.11083v1](https://arxiv.org/html/2502.11083v1) |

## 📚 Additional Resources

### Books

- *Deep Learning* by Ian Goodfellow, Yoshua Bengio, and Aaron Courville (2016) – [View PDF](Deep%20Learning%20by%20Ian%20Goodfellow,%20Yoshua%20Bengio,%20Aaron%20Courville.pdf)
- *Elements of Causal Inference* by Jonas Peters, Dominik Janzing, Bernhard Schölkopf – [View PDF](Elements%20of%20Causal%20Inference%20-%20Peters%20Janzing%20Scholkopf%20-%20MIT%20Press.pdf)
- *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow* (2nd Edition) – [View PDF](Hands-On%20Machine%20Learning%20with%20Scikit-Learn,%20Keras,%20and%20TensorFlow,%202nd%20Edition.pdf)
- *An Introduction to Statistical Learning* by Gareth James et al. (2021) – [View PDF](James%20G.%20et%20al.%202nd%20ed%20Springer%202021.pdf)
- *Probabilistic Graphical Models* by Daphne Koller and Nir Friedman (2009) – [View PDF](Probabilistic%20Graphical%20Models-Dafne%20Koller,%20Friedman%20(2009).pdf)
- *Reinforcement Learning: An Introduction* – [View PDF](Reinforcement%20Learning%20An%20Introduction.pdf)
- *Transformers from Scratch* – [View PDF](TRANSFORMERS%20from%20SCRATCH.pdf)

### Courses
- [CS231n: CNNs for Visual Recognition](http://cs231n.stanford.edu/) – Stanford University.
- [CS224n: NLP with Deep Learning](http://web.stanford.edu/class/cs224n/) – Stanford University.
- [Fast.ai: Practical Deep Learning](https://course.fast.ai/) – Free, hands-on DL course.

### Tools & Libraries
- **Scikit-learn**: [Official Site](https://scikit-learn.org/stable/) – Core ML algorithms.
- **PyTorch**: [Official Site](https://pytorch.org/) – Flexible DL framework.
- **Hugging Face Transformers**: [Official Site](https://huggingface.co/docs/transformers/index) – NLP and multimodal models.
- **JAX**: [Official GitHub](https://github.com/google/jax) – High-performance numerical computing.

### Project Inspiration
- [Top 10 Deep Learning Projects for 2025](https://blog.huebits.in/top-10-deep-learning-projects-to-build-in-2025-with-code-use-cases-career-impact/) – Curated DL projects with use cases and career impact.

## 🤝 Contributing

Contributions are welcome to enhance **ML-Extras**! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Add resources, tutorials, or improvements.
4. Submit a pull request with a clear description.

---

<div align="center">
  <p>Built with ❤️ for the ML community.</p>
  <p>Star this repo to support! ⭐</p>
</div>
