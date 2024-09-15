# Multilingual News Semantic Similarity (Russian, Ukrainian, English, Polish)

This repository contains code to replicate the crowdsourcing pipeline for gathering a multilingual news semantic similarity dataset.

The dataset is available on [HuggingFace](https://huggingface.co/datasets/tum-nlp/multilingual_news_SS_uk_ru_en_pl).

## Requirements

To fully replicate the pipeline, you'll need the following accounts and API tokens:

- [Toloka Self-Service platform](https://toloka.ai/)
- [HuggingFace API token](https://huggingface.co/docs/api-inference/en/quicktour#get-your-api-token)
- [DeepL API token](https://developers.deepl.com/docs/getting-started/auth)
- [Cohere AI API token](https://docs.cohere.com/docs/chat-api)

## Files in this Repository

- **Thesis.pdf**: Contains all the details for gathering and benchmarking the dataset using modern transfer-based models.
- **Sampling_based_on_SemEval.ipynb**: Initial pre-sampling of news pairs from the SemEval22 Task8 Challenge in Russian, English, and Polish.
- **Searching_for_news.ipynb**: Scraping news from Google News and summarizing them.
- **Acceptance_rejection_script.ipynb**: Automated LLM-based quality control for the crowdsourcing solution.
- **Gather, anonymize & analyze dataset.ipynb**: Provides statistics for the dataset along with embedding-based and prompting-based benchmarking.
- **training_project_config.json**: Configuration file for the training project on the Toloka platform.
- **main_project_config.json**: Configuration file for the main project on the Toloka platform.
- **training_ukr_en.tsv**: Training data for labelers working on cross-lingual news pairs (Ukrainian, English).
- **training_ukr_pl.tsv**: Training data for labelers working on cross-lingual news pairs (Ukrainian, Polish).
- **training_ukr_rus.tsv**: Training data for labellers working on cross-lingual news pairs (Ukrainian, Russian).
- **training_ukr_ukr.tsv**: Training data for labellers working on news pairs in Ukrainian.

## Usage

Refer to the Jupyter notebooks provided to replicate each stage of the crowdsourcing pipeline. Ensure that you have configured the necessary API tokens and platform accounts before running the scripts.
