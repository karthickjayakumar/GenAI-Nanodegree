# SMS Spam Classification using PEFT

This project demonstrates how to perform spam classification on SMS messages using a pre-trained transformer model and a Parameter-Efficient Fine-Tuning (PEFT) technique. The goal is to fine-tune a pre-trained model for binary classification to distinguish between spam and non-spam SMS messages.

## Steps Involved

### 1. Loading and Evaluating a Foundation Model
- We use the `DistilBERT` model from Hugging Face's transformers library (`distilbert-base-uncased`) as the foundation model.
- The `SMS Spam` dataset is used for training and evaluation. The dataset is split into training and testing sets for this purpose.
- We load a tokenizer to tokenize the SMS messages, which helps in preparing the dataset for training.
- The pre-trained model is then fine-tuned on the SMS spam dataset to perform the binary classification task.

### 2. Performing Parameter-Efficient Fine-Tuning
- To achieve a more efficient fine-tuning process, we use the `LoRA (Low-Rank Adaptation)` technique from the PEFT library.
- We fine-tune only specific layers (low-rank matrices) while keeping most of the model's weights frozen. This significantly reduces the number of trainable parameters and computation, making it easier to train.
- The Hugging Face `Trainer` is used to train the model efficiently with an accuracy evaluation metric.

### 3. Performing Inference with the PEFT Model
- After training, the model is saved and loaded again for inference.
- The fine-tuned model is used to make predictions on sample messages from the test dataset.
- A DataFrame is created to show the predictions, true labels, and SMS messages, and the accuracy is computed to evaluate the model's performance.

## Technique
This project utilizes **LoRA (Low-Rank Adaptation)** as a Parameter-Efficient Fine-Tuning (PEFT) method. This technique allows efficient training by freezing most of the parameters while adding a few trainable ones, thus reducing the computational cost and memory usage.

## Details
- **Fine-tuning Dataset**: SMS Spam Dataset
- **Model**: DistilBERT (`distilbert-base-uncased`)
- **Evaluation Approach**: Hugging Face Trainer with accuracy metrics
- **PEFT Technique**: LoRA (Low-Rank Adaptation)

## Requirements
Refer to the `requirements.txt` file for dependencies to run the code.

## Usage
1. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
2. Run the Python script to load the foundation model, fine-tune using LoRA, and evaluate the model on the test dataset.


