# Team 1 Major Project
# Enhancing Medical Diagnostics with Vision-Language Models

## Overview

This project leverages Vision-Language Models (VLMs) to enhance medical diagnostics through automated interpretation of radiographs. It uses a fine-tuned Llama model to provide expert-level radiographic analysis.

## Features

- **AI-Powered Radiograph Analysis**: Utilizes a fine-tuned Llama model for accurate medical image interpretation
- **Interactive Web Interface**: Built with Gradio for easy upload and analysis of radiographs
- **Expert-Level Descriptions**: Generates detailed, professional descriptions of radiographic findings

## Model Architecture

The project uses a fine-tuned version of Llama 11B with the following components:

- Base Model: Llama 3.2 11B Vision
- Training Dataset: ROCOv2-Sampled
- Fine-tuning Method: LoRA (Low-Rank Adaptation)
- Special Features: Optimized for medical imaging interpretation

## Resources

### Hugging Face Integration

- **Dataset**  
  [Shriyans/ROCOv2-Sampled](https://huggingface.co/Shriyans/ROCOv2-Sampled)  
  A curated dataset of radiographs with expert annotations.

- **Model (Merged)**  
  [Shriyans/Llama-11B-Rad](https://huggingface.co/Shriyans/Llama-11B-Rad)  
  The complete fine-tuned model for production use.

- **LoRA Adapter**  
  [Shriyans/Llama-11B-Rad-LORA](https://huggingface.co/Shriyans/Llama-11B-Rad-LORA)  
  The LoRA weights for efficient fine-tuning.

## Getting Started

1. **Installation**
   ```bash
   pip install -r requirements.txt
   ```

2. **Running the Interface**
   ```python
   python gradio_inference.py
   ```
   This will start the Gradio interface on localhost:7860

## Usage

1. Open the Gradio interface in your web browser
2. Upload a radiograph image
3. Click "Generate" to receive an expert-level description
4. The model will provide a detailed analysis of the radiographic findings

## Project Structure

- `gradio_inference.ipynb`: Implementation of the web interface using Gradio
- `finetune.ipynb`: Notebook containing the model fine-tuning process
- `README.md`: Project documentation

## Technical Requirements

- Python 3.8+
- CUDA-capable GPU for inference
- Required packages:
  - gradio
  - torch
  - transformers
  - unsloth

## License

Please refer to the model licenses on Hugging Face for usage terms.

## Acknowledgments

- Base Llama model from Meta AI
- ROCOv2 dataset contributors
- Hugging Face for model hosting


