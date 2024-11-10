# AHJL at Qur'an QA 2023 Shared Task: Enhancing Passage Retrieval using Sentence Transformer and Translation

This project is part of the **Qur’an QA 2023 Shared Task**, specifically focused on **Task A: Passage Retrieval (PR)**. The goal of the project is to enhance passage retrieval for questions posed about the Holy Qur’an, using a combination of Sentence Transformer models and translation techniques. This approach improves the model's ability to understand Arabic queries, providing more accurate and contextually relevant passages from the Qur’an as answers.

## Project Description

The Holy Qur’an, with its linguistic richness and spiritual significance, serves as a central text for nearly two billion Muslims worldwide. The task we addressed in the Qur’an QA 2023 Shared Task involves retrieving relevant passages in response to questions asked in Modern Standard Arabic. Our approach leverages advanced natural language processing (NLP) and information retrieval (IR) techniques to optimize the accuracy and relevance of these retrieved passages.

### Key Components

1. **Sentence Transformer Model**: We employ a Sentence Transformer model that transforms the search query into embeddings, allowing for effective similarity-based retrieval.
2. **Translation Module**: To overcome the model’s limitations with Arabic, we integrate a translation step that converts Arabic queries to English before retrieval and converts results back to Arabic, enhancing performance.
3. **Paraphrasing**: An additional paraphrasing module enriches the query interpretation process by creating multiple versions of the question, leading to improved retrieval outcomes.

### Highlights

- **Translation-Enhanced Retrieval**: By translating Arabic queries, the model better interprets the linguistic nuances of the original question, leading to higher retrieval accuracy.
- **Semantic and Dense Retrieval**: Our model uses dense retrieval techniques, allowing it to capture deeper contextual relationships beyond simple keyword matching.
- **No-Answer Detection**: For questions without an answer in the Qur’an, our model effectively filters irrelevant passages by applying a similarity threshold.

## Methodology

- **Dataset**: The project uses a Qur’anic passage collection (QPC) and questions from the AyaTEC dataset. The dataset includes relevance assessments to gauge how well passages respond to various questions.
- **Model Architecture**: Our cross-lingual architecture uses a Sentence Transformer model combined with OpenAI embeddings for document retrieval, as well as a cross-encoder re-ranker for additional filtering.
- **Evaluation Metrics**: Mean Average Precision (MAP) and Mean Reciprocal Rank (MRR) were used to evaluate retrieval accuracy. All experiments were conducted in a zero-shot setup without further fine-tuning.

## Results

- **Performance**: Our model incorporating translation outperformed the non-translation model across all metrics, achieving higher MAP and MRR scores.
- **Top Results**: The highest-performing model achieved an MRR of 0.389 and MAP of 0.343 on the development set.


### Conclusion
Our approach successfully integrates translation to improve passage retrieval accuracy in Arabic question-answering systems. By participating in the Qur’an QA 2023 Shared Task, we demonstrate how translation and paraphrasing can enhance understanding and retrieval quality for complex religious texts.

### Authors
Hessa A. Alawwad - Imam Mohammad Ibn Saud Islamic University
Lujain A. Alawwad - Saudi Electronic University
Jamilah Alharbi - King Abdulaziz University
Abdullah I. Alharbi - King Abdulaziz University

### Citation
If you use this code in your research, please cite our work presented at the First Arabic Natural Language Processing Conference (ArabicNLP 2023).

```bash
Alawwad, H., Alawwad, L., Alharbi, J., & Alharbi, A. (2023, December). AHJL at Qur’an QA 2023 Shared Task: Enhancing Passage Retrieval using Sentence Transformer and Translation. In Proceedings of ArabicNLP 2023 (pp. 702-707).‏


### License
This project is licensed under the MIT License - see the LICENSE file for details.

