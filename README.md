# AutoGenKernel: Code Generation for Linux Kernel with Char RNNs

## Overview
The AutoGenKernel project explores the feasibility of using Character-Level Recurrent Neural Networks (Char RNNs) to automate the generation of Linux kernel code snippets. By leveraging machine learning models trained on a comprehensive dataset of Linux kernel source code, this project aims to push the boundaries of AI's capabilities in system-level programming.

## Key Features
- Utilizes Char RNNs, including LSTM (Long Short-Term Memory) and GRU (Gated Recurrent Units) models.
- Trained on over 15 million lines of Linux kernel source code, ensuring a diverse and representative learning set.
- Capable of generating syntactically plausible and thematically relevant code snippets for Linux kernel development.
- Includes systematic experimentation with various model architectures and hyperparameter configurations to optimize performance.

## Getting Started

### Prerequisites
- Python 3.6+
- TensorFlow 2.x
- Keras
- Additional Python libraries as listed in `requirements.txt`

### Installation
1. Clone the repository: `github clone https://github.com/yfranci/AutoGenKernel/`
2. Install the required dependencies:`pip install -r requirements.txt`



## Dataset
The dataset comprises multiple versions of the Linux kernel, totaling over 15 million lines of code. It was compiled from the official Linux kernel repository, focusing on the latest stable versions to ensure relevance and modernity.

## Model Architecture
The project experiments with Char RNN models, specifically focusing on variations in architecture to identify the most effective setup, including:
- An embedding layer to map characters to high-dimensional vectors.
- Recurrent layers (using either LSTM or GRU units) to capture dependencies and patterns in the code.
- A dense output layer to predict the next character in a sequence.

## Hyperparameter Tuning
Hyperparameter tuning was conducted using both manual experimentation and automated optimization tools like Keras Tuner. The optimal configuration was determined to be 512 LSTM units, an embedding dimension of 256, sequence lengths of 100 characters, and a learning rate of 0.001.

## Evaluation
The generated code's quality was evaluated based on syntactical correctness, thematic relevance, and practical usability, with contributions from subject matter experts in Linux kernel development.

## Contributing
We welcome contributions to the AutoGenKernel project. Please read `CONTRIBUTING.md` for more details on submitting pull requests to us.

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.



