# DqSalience — Question Salience in Dialogue

**Dialogue Analysis · Question Under Discussion (QUD) · LLMs · Transformer Models**

This repository presents the work carried out as part of our supervised M1 NLP group project at **IDMC, Université de Lorraine**, entitled *"Extracting topical information from real-life conversations based on the notion of potential question."*

## Project Overview

How can we identify the most salient questions arising from real-life conversations?

This project investigates **question salience in dialogue**, drawing on the linguistic framework of **Questions Under Discussion (QUD)**. The goal is to generate contextually relevant questions from conversational exchanges and evaluate their importance for discourse understanding and conversational continuity.

## Methodology

The project combines computational linguistics, human annotation, and machine learning through several stages:

1. **Dialogue processing:** Corpus exploration, preprocessing, and analysis of conversational turns.
2. **Question generation:** Context-aware generation of potential questions using Large Language Models.
3. **Human annotation:** Evaluation of generated questions on a 0–8 salience scale.
4. **Inter-annotator agreement:** Analysis of annotation consistency using Cohen's Kappa.
5. **Salience prediction:** Experiments with Transformer-based classifiers and fine-tuned LLMs.
6. **Model evaluation:** Comparison of predictions against human annotations using classification and agreement metrics.

## Models and Techniques

The repository includes experiments involving:

- **Longformer:** Question salience classification using conversational context, class-weighted training, and stratified cross-validation.
- **Llama 3, Qwen, and Mistral:** LLM-based salience prediction and fine-tuning experiments.
- **LoRA and 4-bit quantization:** Parameter-efficient fine-tuning configurations.
- **Evaluation:** Accuracy, F1-score, MAE, Pearson correlation, and weighted Cohen's Kappa.

## Tech Stack

**Python · PyTorch · Hugging Face Transformers · PEFT/LoRA · scikit-learn · pandas · NumPy · Jupyter Notebook**

## Repository Structure

- `LLM questions generation/` — Context-based question generation.
- `Annotations/` — Human annotation data.
- `IAA/` — Inter-annotator agreement analysis.
- `DQsalience/` — Neural-network and LLM-based salience prediction.
- `Mistral_Annotations/` — Additional annotation materials.
- `Stats/` — Corpus statistics and exploratory analysis.

## Reproducibility

This repository contains research code and experimental materials developed during the project. Reproducing individual experiments may require additional corpus resources, pretrained model weights, and local environment configuration.

## Authors

This project was developed collaboratively by:

**Mario Jakimoski · Axel Felten · Hao Meng · Jinane Harchal**


## License

MIT License. See [LICENSE](LICENSE) for details.
