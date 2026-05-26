# 🧠 PyTorch Natural Language Processing (NLP) Cookbook

Welcome to the **PyTorch NLP Cookbook**! This repository is a curated collection of Jupyter Notebooks demonstrating various core concepts, architectures, and tasks in Natural Language Processing. 

From implementing classic recurrent neural network architectures (RNNs, LSTMs, GRUs) and attention mechanisms completely from scratch to leveraging modern Transformer-based models (BERT, GPT-2), this repository serves as an educational and practical reference for building deep learning models for text.

---

## 🗺️ Repository Structure & Covered Tasks

The repository is organized by NLP task areas. Below is a detailed breakdown of each directory and the architectures implemented:

### 1. 🎭 Sentiment Analysis (`Sentiment/`)
*Classifying text comments/reviews as positive or negative.*
*   **`1_BiLSTM.ipynb`**: Bidirectional Long Short-Term Memory (BiLSTM) network.
*   **`2_FastText.ipynb`**: An efficient, fast bag-of-words and n-gram classifier.
*   **`3_WordAttention.ipynb`**: Custom Word-Level Attention mechanism over Recurrent States.
*   **`4_BERT+FFNN.ipynb`**: BERT feature extraction combined with a Feed-Forward Neural Network.
*   **`5_BERT+GRU.ipynb`**: BERT embeddings coupled with a GRU classification layer.

### 2. 📝 Language Modeling (`LM/`)
*Next-character or next-word token generation across various datasets.*
*   **Names Generator (`Names_generator/`)** *(Character-level generation)*:
    *   `1_RNN_manual.ipynb`: Core Recurrent Neural Network built manually.
    *   `2_GRU.ipynb`: Gated Recurrent Unit (GRU) generator.
    *   `3_GRU_batch.ipynb`: Batched GRU language model.
    *   `4_GRU_batch_bptt.ipynb`: Batched GRU with Backpropagation Through Time (BPTT).
*   **WikiText2 (`WikiText2/`)** *(Word-level language modeling & Transformers)*:
    *   `1_GRU.ipynb`: GRU-based language model.
    *   `2_Transformer_from_scratch.ipynb`: Full Transformer encoder-decoder built from scratch.
    *   `3_Transformer_from_scratch_position_encoding.ipynb`: From-scratch Transformer with custom positional encodings.
    *   `4_Transformer_module.ipynb`: Native PyTorch `nn.Transformer` implementation.
    *   `5_GPT2.ipynb`: Causal Language Modeling utilizing the GPT-2 architecture.

### 3. ⚖️ Natural Language Inference (`NLI/`)
*Determining whether a hypothesis is true (entailment), false (contradiction), or neutral given a premise.*
*   **`1_Linear.ipynb`**: Linear/Feed-Forward classifier.
*   **`2_BiLSTM.ipynb`**: Premise-hypothesis encoder using a Bidirectional LSTM.
*   **`3_Bahadanau.ipynb`**: BiLSTM equipped with a custom **Bahdanau Attention** layer.

### 4. 🏷️ Named Entity Recognition (`NER/`)
*Locating and classifying named entities (people, organizations, locations, etc.) in unstructured text.*
*   **`NER_BERT.ipynb`**: Named Entity Recognition leveraging contextual BERT embeddings.

### 5. 🌐 Sequence-to-Sequence Translation (`Translation/`)
*Machine translation of text between different languages.*
*   **`1_LSTM.ipynb`**: Classic Encoder-Decoder LSTM framework.
*   **`2_LSTM_Bahdanau1.ipynb`** / **`3_LSTM_Bahdanau2.ipynb`**: Encoder-Decoder models with customized Bahdanau attention.
*   **`4_Transformer.ipynb`**: Full Transformer sequence-to-sequence model for machine translation.

---

## 🛠️ Requirements & Tech Stack

This codebase is built using:
*   **Deep Learning Framework**: [PyTorch](https://pytorch.org/) (v2.x recommended)
*   **Hugging Face**: `transformers` & `tokenizers`
*   **Data & SciPy**: `numpy`, `scikit-learn`
*   **Visualization**: `matplotlib`, `seaborn`
*   **Environments**: Jupyter Notebooks / JupyterLab

---

## 🚀 Getting Started

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/pytorch_NLP.git
    cd pytorch_NLP
    ```

2.  **Set Up a Virtual Environment (Recommended)**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install Core Dependencies**:
    ```bash
    pip install torch torchvision torchaudio
    pip install transformers datasets scikit-learn matplotlib jupyter
    ```

4.  **Run the Notebooks**:
    Launch Jupyter Lab or Notebook and start exploring:
    ```bash
    jupyter lab
    ```

---

> [!NOTE]
> The comments, explanations, and annotations throughout these notebooks are constantly being expanded and updated to provide maximum clarity on NLP concepts. Feel free to explore, tweak parameters, and train your own custom models!
