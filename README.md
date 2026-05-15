# ✍️ Handwritten Digit Recognition using PyTorch

### My First Neural Network & Deep Learning Project using PyTorch

A Deep Learning project that recognizes handwritten digits using a **Feedforward Neural Network implemented from scratch in PyTorch**.

This is my **first Neural Network / Deep Learning project**, and it marks the beginning of my journey into Deep Learning and Neural Networks.

This project was built step-by-step to deeply understand:

* How neural networks actually learn
* Forward propagation
* Backpropagation
* Loss functions
* Optimizers
* Model evaluation
* Error analysis
* Training visualization

Rather than simply using high-level APIs, this project focuses on understanding the **core mechanics of neural networks** using PyTorch.

I’m extremely excited about continuing my journey into:

* Neural Networks
* Computer Vision
* CNNs
* Transformers
* Generative AI
* Large Language Models (LLMs)

This project represents the foundation of that journey.

---

# 🚀 Project Overview

The goal of this project is to classify handwritten digits from the MNIST dataset:

```text id="v0b2ye"
(28 × 28 grayscale image) → Digit (0–9)
```

The neural network learns patterns from pixel values and predicts the most probable digit.

This project emphasizes:

* Understanding neural networks from scratch
* Deep learning workflow using PyTorch
* Visualization and model interpretation
* Training and evaluation mechanics

---

# 🧠 Deep Learning Concepts Used

This project covers:

* PyTorch Tensors
* Dataset & DataLoader
* Feedforward Neural Networks
* Linear Layers
* ReLU Activation Function
* Forward Pass
* Backpropagation
* Gradient Descent
* Adam Optimizer
* CrossEntropyLoss
* Model Evaluation
* Accuracy Calculation
* Loss Visualization
* Wrong Prediction Analysis
* Model Saving & Loading

---

# 📊 Dataset

The project uses the **MNIST handwritten digit dataset**.

Dataset details:

| Property        | Value           |
| --------------- | --------------- |
| Training Images | 60,000          |
| Test Images     | 10,000          |
| Image Size      | 28 × 28         |
| Classes         | 10 Digits (0–9) |
| Image Type      | Grayscale       |

Each image represents a handwritten digit.

---

# ⚙️ Data Processing

### 🔹 Tensor Conversion

Images are converted into PyTorch tensors using:

```python id="jlwm41"
transforms.ToTensor()
```

Pixel values are normalized from:

```text id="jlwm42"
0–255 → 0–1
```

This helps the neural network train more efficiently.

---

# 🧠 Neural Network Architecture

The model architecture:

```text id="jlwm43"
784 → 128 → 64 → 10
```

Where:

| Layer | Description                   |
| ----- | ----------------------------- |
| 784   | Flattened image input (28×28) |
| 128   | Hidden layer                  |
| 64    | Hidden layer                  |
| 10    | Output classes (digits 0–9)   |

The final layer outputs scores for each digit class, and the digit with the highest score becomes the prediction.

---

# ⚡ Activation Function

The project uses the **ReLU activation function**:

```text id="jlwm45"
f(x) = max(0, x)
```

ReLU introduces non-linearity and allows the network to learn complex patterns from handwritten digits.

---

# 📉 Loss Function

The model uses:

```python id="jlwm46"
nn.CrossEntropyLoss()
```

CrossEntropyLoss is widely used for classification problems because it:

* Converts logits into probabilities internally
* Penalizes incorrect predictions
* Rewards confident correct predictions

---

# ⚙️ Optimizer

The project uses the **Adam Optimizer**:

```python id="jlwm47"
torch.optim.Adam()
```

Adam updates the model weights during training using gradient-based optimization.

---

# 🔄 Training Process

Training pipeline:

```text id="jlwm48"
Input Images
↓
Forward Pass
↓
Loss Calculation
↓
Backpropagation
↓
Weight Update
↓
Repeat
```

The model is trained for multiple epochs using mini-batch gradient descent.

---

# 📈 Training Results

The project achieved:

```text id="jlwm49"
Test Accuracy ≈ 97%
```

The training loss consistently decreases across epochs, showing that the neural network successfully learned handwritten digit patterns.

---

# 📊 Visualizations

The project includes:

* Training Loss Graph
* Prediction Visualization
* Wrong Prediction Analysis
* Handwritten Digit Display

These visualizations help understand:

* Learning progress
* Model performance
* Common prediction mistakes

---

# 🔍 Wrong Prediction Analysis

Incorrect predictions are collected and visualized to analyze:

* Confusing handwritten digits
* Model weaknesses
* Similar digit patterns

This helps understand model behavior beyond simple accuracy numbers.

---

# 💾 Model Saving & Loading

The trained model is saved using:

```python id="jlwm50"
torch.save(model.state_dict(), "mnist_model.pth")
```

The project also demonstrates loading trained weights back into a neural network for inference.

---

# 📂 Project Structure

```text id="jlwm51"
mnist-digit-recognition-pytorch
│
├── mnist_nn.ipynb
├── mnist_model.pth
├── README.md
└── data/
```

---

# 🎯 Key Learning Outcomes

Through this project, I learned:

* How neural networks learn from data
* Importance of forward and backward propagation
* Role of loss functions and optimizers
* How PyTorch training loops work
* Difference between training and inference
* How to evaluate deep learning models
* How to visualize and analyze model performance
* Real-world deep learning workflow using PyTorch

Most importantly, this project gave me my first real hands-on experience with Neural Networks and Deep Learning.

---

# 📌 Future Improvements

Possible future extensions:

* Convolutional Neural Networks (CNNs)
* GPU/CUDA acceleration
* Hyperparameter tuning
* CNN vs Feedforward comparison
* Real-time digit drawing interface
* Deployment using Streamlit

---

# 🌱 Beginning of My Deep Learning Journey

This project is the starting point of my Neural Network and Deep Learning journey.

Building this project from scratch helped me move beyond tutorials and truly understand how neural networks work internally.

I’m excited to continue learning and building projects involving:

* Computer Vision
* CNNs
* Transformers
* LLMs
* Generative AI
* Advanced Deep Learning architectures

This is only the beginning.

---

# 👨‍💻 Built By

**Hemanth M**

Computer Science Student | Machine Learning Enthusiast
