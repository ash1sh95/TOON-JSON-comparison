# Token Consumption Comparison: JSON vs TOON Format for LLMs

This notebook demonstrates a practical comparison of token consumption between the standard JSON format and a custom TOON format, using a sample data structure. The goal is to help users understand how different serialization formats impact token usage when interacting with Large Language Models (LLMs).

## Key Steps

- Generate representative sample data
- Serialize the data to JSON and TOON formats
- Count tokens in each format using whitespace splitting (a simple proxy for LLM tokenization)
- Summarize the results and implications for LLM usage

## Results Summary

- **JSON format:** 18 tokens
- **TOON format:** 9 tokens

The TOON format resulted in fewer tokens for this sample, likely due to its more compact, flat representation.

## Implications for LLM Usage

- Fewer tokens can reduce LLM costs and improve performance, especially for large payloads or frequent API calls.
- The actual token count may vary depending on the LLM's tokenizer; this notebook uses whitespace splitting for simplicity.
- Custom formats like TOON may be beneficial for specific use cases, but always validate with your target LLM's tokenizer.

## Usage

Open the notebook `Untitled Notebook 2025-11-15 17_32_27.ipynb` in Jupyter Notebook or JupyterLab to run the code and see the comparison.

Feel free to adapt this notebook for your own data and LLM workflows.
