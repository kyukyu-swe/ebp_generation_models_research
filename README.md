# EBP Generation Models Research

This repository contains the research and evaluation of various text generation models for the EBP-bot's Retrieval-Augmented Generation (RAG) method. The focus is on comparing the performance of different models when generating responses based on provided labor law contexts.

## Repository Structure

- **data/**

  - `formatted_data_ebp.json`: Contains the labor law contexts used for testing the models.

- **notebooks/**

  - Jupyter notebooks for each model tested, detailing the evaluation process and results.

- **results/**
  - `Comparison of Generation Models.docx.pdf`: A PDF summarizing the comparison results of the tested models.

## Models Tested

We evaluated several text generation models from HuggingFace, including:

- `TinyLlama/TinyLlama-1.1B-Chat-v1.0`
- `openai-community/gpt2-large`
- `unsloth/tinyllama`
- `unsloth/tinyllama-chat`
- `unsloth/mistral-7b-v0.3`

## Evaluation Method

Each model was given the same set of questions and contexts extracted from the `formatted_data_ebp.json` file. The generated responses were then compared based on coherence, accuracy, and relevance to the provided context.

## Conclusion

Based on our evaluation, the `unsloth/tinyllama-chat` model provided the most accurate and contextually appropriate answers, making it the preferred choice for EBP-bot's RAG framework.

## Usage

To run the evaluations yourself, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/kyukyu-swe/ebp_generation_models_research.git
   cd ebp_generation_models_research
   ```

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebooks in the `notebooks/` directory to see the evaluation process and results for each model.

## Acknowledgements

We acknowledge the use of models and tools provided by HuggingFace in this research.

---
