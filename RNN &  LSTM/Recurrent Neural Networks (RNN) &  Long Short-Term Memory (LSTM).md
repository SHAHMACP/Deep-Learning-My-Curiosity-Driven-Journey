# Recurrent Neural Networks (RNN) &  Long Short-Term Memory (LSTM)

This document provides a concise overview of **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)** networks used for sequential data modeling in Deep Learning.

---

# Recurrent Neural Network (RNN)

![Image](https://www.researchgate.net/publication/321811462/figure/fig2/AS%3A758310718406662%401557806772700/An-unrolled-Recurrent-Neural-Network.ppm)

![Image](https://d2l.ai/_images/rnn.svg)

## Overview

Recurrent Neural Networks (RNNs) are neural networks designed to process **sequential data** where the output depends on previous inputs.

Unlike feedforward neural networks, RNNs maintain a **hidden state** that captures information from previous time steps.

---

## Mathematical Representation

At time step $ t $:

$$
h_t = f(W_x x_t + W_h h_{t-1} + b)
$$

Where:

* $x_t$ → Input at time step ( t )
* $h_{t-1}$ → Previous hidden state
* $h_t$ → Current hidden state
* $W_x, W_h$ → Weight matrices
* $b$ → Bias
* $f$ → Activation function (tanh / ReLU)

---

## Key Characteristics

* Shared weights across time steps
* Sequential dependency modeling
* Suitable for variable-length inputs

---

## Applications

* Sentiment Analysis
* Language Modeling
* Time-Series Forecasting
* Speech Recognition

---

## Limitations

RNNs suffer from:

* **Vanishing Gradient Problem**
* **Exploding Gradient Problem**
* Difficulty learning long-term dependencies

---

# Long Short-Term Memory (LSTM)

![Image](https://www.researchgate.net/publication/352658938/figure/fig5/AS%3A1038391751737346%401624583294392/LSTM-cell-architecture.png)

![Image](https://media.licdn.com/dms/image/v2/D4D12AQF7aHYXD7SINQ/article-cover_image-shrink_600_2000/article-cover_image-shrink_600_2000/0/1721761416816?e=2147483647\&t=B5_d1-po8kcVseMpzGjJ_69vYypHwZunvAUjGQ3v3YU\&v=beta)

## Overview

LSTM is a specialized type of RNN introduced to overcome the vanishing gradient problem and capture **long-term dependencies**.

It introduces a **memory cell** that preserves information over long sequences.

---

## Core Components of LSTM

An LSTM cell contains:

1. **Forget Gate** – Controls what information to discard
2. **Input Gate** – Controls what new information to store
3. **Output Gate** – Controls what to output

Additionally:

* Cell state ( C_t ) carries long-term memory
* Hidden state ( h_t ) carries short-term memory

---

## Gate Equations

Forget Gate:
$f_t = \sigma(W_f [h_{t-1}, x_t] + b_f)$


Input Gate:
$i_t = \sigma(W_i [h_{t-1}, x_t] + b_i)$


Cell Update:
$C_t = f_t * C_{t-1} + i_t * \tilde{C}_t$


Output Gate:
$h_t = o_t * \tanh(C_t)$


---

## Why LSTM is Powerful

* Maintains long-term memory
* Reduces vanishing gradient issue
* More stable training for long sequences

---

## Applications

* Machine Translation
* Text Generation
* Question Answering
* Financial Time-Series Prediction

---

# RNN vs LSTM Comparison

| Feature                       | RNN        | LSTM            |
| ----------------------------- | ---------- | --------------- |
| Memory Type                   | Short-term | Long-term       |
| Vanishing Gradient            | Severe     | Reduced         |
| Architecture                  | Simple     | Gated & Complex |
| Performance on Long Sequences | Weak       | Strong          |
| Training Stability            | Lower      | Higher          |

---

# Summary

* **RNN** models sequential dependencies using hidden states.
* **LSTM** enhances RNN by introducing gated memory mechanisms for long-term learning.

---
