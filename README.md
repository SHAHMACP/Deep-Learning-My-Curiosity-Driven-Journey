<div align="center">

  <h1>Deep Learning Materials & Learning Journey</h1>

  <p>
    <strong>From basics to advanced — collected, explained, and derived by hand</strong><br>
    A growing personal knowledge base started from pure curiosity about how neural networks actually learn.
  </p>

</div>

## 🌱 Why This Repository Exists

It all started with one question:

**“What is really happening inside when we call model.fit() or when gradients flow backward?”**

So I built a small 4-4-1 feedforward network **completely by hand** — no PyTorch, no TensorFlow — just matrices, chain rule, sigmoid derivative, and a calculator.  
Computing forward pass → loss → δ errors → weight gradients step by step gave me the clarity I was looking for.

This repository is the result: my evolving collection of:

- Presentation slides  
- Mathematical derivations  
- Step-by-step manual calculations  
- Comparison tables  
- Visual explanations  

… covering **Deep Learning from the very beginning** and expanding over time.

Right now the focus is on foundational concepts, but this is **not just about ANNs / MLPs**.  
In the future it will include CNNs, RNNs/LSTMs/GRUs, Transformers, GANs, diffusion models, optimization tricks, regularization, modern architectures, training recipes, and anything else I find interesting and worth understanding deeply.

## 📂 Current Content (as of Jan 2026)

| Topic                              | Format                  | Status      | Highlights                                      |
|------------------------------------|-------------------------|-------------|-------------------------------------------------|
| AI vs ML vs Deep Learning          | Slides + diagrams       | Complete    | Venn, pyramid, definitions                      |
| What is Deep Learning?             | Slides                  | Complete    | Layers, hierarchy, supervised/unsupervised      |
| Why Deep Learning?                 | Detailed comparison     | Complete    | Feature learning, scalability, unstructured data|
| Biological inspiration → ANN basics| Slides + visuals        | Complete    | Neuron comparison, weighted sum                 |
| Perceptron & Multi-Layer Perceptron| Math + diagrams         | Complete    | Single vs multi-layer, fully connected          |
| Activation functions               | Math + graphs           | Complete    | Sigmoid, tanh, ReLU, Softmax                    |
| Forward Propagation                | Matrix form             | Complete    | Layer-by-layer computation                      |
| Loss Functions                     | Matrix expressions      | Complete    | MSE, Binary/CE, Categorical/CE                  |
| Backpropagation                    | Full derivation         | Complete    | Chain rule, δ propagation, worked 4-4-1 example |
| Optimization Algorithms            | Update rules + table    | Complete    | GD, SGD, Momentum, Adam, AdamW                  |
| …and growing                       | —                       | In progress | CNN, RNN, Transformers, attention, etc.         |
