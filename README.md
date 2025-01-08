# NLP Trainer: A Virtual Assistant for Mastering NLP Basics and Interview Questions


## Overview

The **NLP Trainer** is an intelligent virtual assistant designed to enhance understanding of Natural Language Processing (NLP) concepts and assist with interview preparation. Leveraging a Retrieval-Augmented Generation (RAG) pipeline and advanced Large Language Models (LLMs), the assistant provides precise, context-aware answers to common NLP questions.

---

## Features

- **Interactive Q&A**: Provides answers to foundational NLP concepts and advanced interview-style questions.
- **Multi-Model Support**: Includes two powerful LLMs:
  - **Llama-3.2-3B-Instruct** for detailed responses.
  - **Flan-T5-Large** for concise answers.
- **Retrieval-Augmented Generation (RAG)**: Combines knowledge retrieval with generative capabilities for context-aware responses.
- **Gradio UI**: Intuitive web-based interface for seamless interaction.

---

## Objectives

1. **Knowledge Enhancement**: Strengthen user understanding of NLP concepts.
2. **Interview Preparation**: Provide clear, structured answers to frequently asked interview questions.
3. **Performance Optimization**: Deliver accurate, contextually relevant answers efficiently.

---

## Project Workflow

### 1. **Data Collection and Preprocessing**
   - Compiled a corpus of over 12,000 words from:
     - PDF of top 100 NLP interview questions.
     - Web scraping from authoritative sources.
   - Preprocessed using `PyPDF2` and `BeautifulSoup` to ensure data quality.

### 2. **RAG Pipeline Implementation**
   - **Embeddings**: Generated using `all-MiniLM-L6-v2` from Sentence Transformers.
   - **Retrieval**: Utilized FAISS for fast similarity searches and context retrieval.
   - **Context Integration**: Filtered results using a similarity threshold of 0.7 for precision.

### 3. **LLMs**
   - **Llama-3.2-3B-Instruct**: Chosen for contextual depth and efficiency.
   - **Flan-T5-Large**: Excels in question-answering with concise outputs.

### 4. **Optimization**
   - Fine-tuned RAG parameters and similarity thresholds.
   - Enhanced prompt engineering to handle diverse query formats.
   - Improved text cleanup for refined responses.

---

## Evaluation

- **Metrics**: Evaluated using BLEU and ROUGE on 30 common NLP questions.
- **Results**:
  - **Llama-3.2**: Higher scores, better for detailed responses.
  - **Flan-T5**: Slightly lower scores, ideal for brevity.

---

## UI Screenshots

- Llama-3.2 sample output
![Llama output](https://github.com/sudip0789/NLP_Trainer/blob/main/UI_images/llama_3.2_ui.png)

- Flan T5 sample output
![FlanT5 output](https://github.com/sudip0789/NLP_Trainer/blob/main/UI_images/flan_t5_ui.png)


---

## How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/sudip0789/NLP_Trainer.git
   cd NLP_Trainer
   ```
2. Add your Hugging Face token.
3. The code was originally ran on Google Colab, hence replace the imports of the input files.
