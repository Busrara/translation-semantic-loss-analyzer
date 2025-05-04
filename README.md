# translation-semantic-loss-analyzer

This is a toolkit for analyzing how well machine translation preserves meaning in different languages.  
Built on Hugging Face's Transformers, it evaluates the **semantic fidelity** of translations by comparing BERT embeddings between source and translated texts.

## What Problem Does It Solve?

> How much meaning is lost when translating between languages?
It handles this fundamental question in translation technology. By computing **cosine similarity** between multilingual BERT embeddings, the tool quantifies how much semantic content is protected when translating and back-translating text between English and other languages.

## Key Features

- Translation using state-of-the-art transformer models (via Hugging Face)
- Semantic similarity analysis using multilingual BERT embeddings
- Visual comparison of translation quality across language pairs
- Batch processing support for multiple source texts

## Methodology

1. Input English sentence(s)
2. Translate into target language (e.g., French, German, etc.)
3. Back-translate into English
4. Extract sentence embeddings using `sentence-transformers`
5. Calculate **cosine similarity** between original and back-translated embeddings
6. Visualize semantic preservation with bar plots

## Supported Languages

- English ↔ Spanish  
- English ↔ French  
- English ↔ German  
- English ↔ Italian  
- English ↔ Portuguese  

## Ideal For

- NLP researchers
- Linguists
- AI engineers evaluating machine translation quality
- Anyone interested in going beyond BLEU scores or traditional evaluation metrics

For deeper understanding, you can read my Medium writing on this project: https://medium.com/@busraracoban/understanding-semantic-preservation-in-machine-translation-building-semantic-loss-analyzer-0ddd6cf26eb8


