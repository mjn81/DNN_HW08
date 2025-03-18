# Fine-Tuning GPT-2 for Short Story Generation

## Overview
This repository contains the implementation and analysis for Homework 08 of the **Deep Learning and Neural Computation** course. The goal of this project is to fine-tune the **GPT-2** model for short story generation and compare its performance with the pre-trained model.

## Contents
- **HW08.pdf**: The problem statement outlining the objectives, dataset, implementation steps, and evaluation criteria.
- **NN_HW08.ipynb**: A Jupyter Notebook containing the implementation of the fine-tuning process, including dataset preparation, model training, and evaluation.

## Project Objectives
1. **Fine-Tune GPT-2**: Train a fine-tuned version of GPT-2 using a dataset of short stories.
2. **Dataset Preparation**: Utilize a cleaned dataset in `.txt` format or use existing datasets such as `Stories Dataset` from **Hugging Face Datasets**.
3. **Model Training**:
   - Load the **GPT-2 (gpt2-small)** pre-trained model using `Hugging Face Transformers`.
   - Tokenize the dataset using the appropriate tokenizer.
   - Fine-tune the model using `Trainer API` in Hugging Face.
4. **Performance Evaluation**:
   - Compare the outputs of the fine-tuned model with the base GPT-2 model.
   - Use the following evaluation metrics:
     - **Diversity**
     - **Fluency**
     - **Coherence**
   - Conduct an analysis of early stopping techniques to assess their impact on model performance.

## Implementation Steps
### 1. Environment Setup
To run the notebook, ensure you have the required dependencies installed:
```bash
pip install transformers datasets torch numpy
```

### 2. Data Preprocessing
- The dataset is preprocessed and tokenized using `Hugging Face Tokenizers`.
- The text is converted into input sequences suitable for GPT-2 fine-tuning.

### 3. Model Fine-Tuning
- The `Trainer API` is used to fine-tune the GPT-2 model.
- Hyperparameters such as batch size, learning rate, and epochs are adjusted to optimize performance.

### 4. Evaluation
- The model’s generated text is compared against the base GPT-2 model.
- Metrics such as **diversity, fluency, and coherence** are used to assess improvements.

### 5. Early Stopping Analysis
- The effect of early stopping on fine-tuning performance is explored.
- The goal is to determine whether early stopping improves generalization and prevents overfitting.


