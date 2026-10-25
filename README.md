# domofine-clinical-llm

## Fine-tuning Llama-3 with QLoRA to extract ICD-10 codes from clinical notes
# DomoFine: Clinical Entity Extraction with QLoRA

Fine-tuning Llama-3-8B (4-bit QLoRA via Unsloth) to turn unstructured
clinical notes into structured JSON containing symptoms and ICD-10 codes.

## Status
- [x] Environment setup (Kaggle T4 GPU, Hugging Face, WandB)
- [x] Data pipeline (synthetic notes, ChatML, 80/10/10 split)
- [ ] QLoRA training
- [ ] Evaluation (base vs fine-tuned)
- [ ] GGUF export and Ollama deployment
- [ ] Rerun on MIMIC data

## Dataset
Synthetic clinical notes with ICD-10-labelled JSON answers in ChatML format.
Split: 800 train / 100 validation / 100 test. Placeholder for MIMIC-IV.
No real patient data is stored in this repository.

## Stack
Python, Hugging Face (Transformers, PEFT, TRL), Unsloth, PyTorch, WandB, Ollama.
