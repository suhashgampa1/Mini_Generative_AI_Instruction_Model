# Mini GenAI: Instruction Fine-Tuning with T5

This project demonstrates a complete end-to-end pipeline for fine-tuning a Large Language Model (LLM) to follow specific instructions. Using the `t5-small` architecture, the system is trained on custom instruction-input-output datasets to generate contextually relevant text responses.

## 🚀 Features
* **Instruction Fine-Tuning:** Uses Hugging Face `Trainer` API to adapt T5-small for specialized tasks.
* **Text Processing:** Includes a demonstration of tokenization and word embeddings using DistilBERT.
* **Interactive UI:** Built-in Gradio interface for testing the model with custom instructions and inputs.
* **Automated Pipeline:** Handles data preprocessing, training, and model saving/exporting in a single workflow.

## 🛠️ Tech Stack
* **Python 3.11+**
* **Hugging Face Transformers:** For model loading and fine-tuning.
* **PyTorch:** Underlying deep learning framework.
* **Datasets:** For efficient data handling and mapping.
* **Gradio:** For creating the web-based inference UI.

## 📸 Technical Workflow

1. **Tokenization:** Converts raw text into numerical `input_ids` that the model can process.
2. **Fine-Tuning:** The T5 model is trained using a supervised approach where it learns to map `Instruction + Input` to a specific `Output`.
3. **Inference:** The saved model is loaded into a Hugging Face `pipeline` for text-to-text generation.
4. **Deployment:** A Gradio interface provides a user-friendly way to interact with the model.

