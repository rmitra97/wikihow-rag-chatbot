# A User Facing RAG Assistant for Your Daily “How-To” Questions

This project explores a lightweight, product-facing **Retrieval-Augmented Generation (RAG)** assistant using open data from WikiHow to answer common "how-to" queries grounded in factual, real-world content.

## 1. Project Goal

To reduce hallucinations in LLMs by grounding everyday instructional questions in WikiHow content.  
Example: “How to clean a hermit crab tank?” or “How to sanitize cloth diapers?”

## 2. Techniques Used
- **Sentence-Transformers** (`all-MiniLM`) for embedding answers
- **FAISS** for fast vector-based retrieval
- **FLAN-T5 (base)** for grounded response generation
- **RAG Pipeline**: query → retrieve → prompt → generate

## 3. Dataset
- Source: [`Lurunchik/WikiHowNFQA`](https://huggingface.co/datasets/Lurunchik/WikiHowNFQA)
- Subset used: 500 “how-to” QA pairs

## 4. Evaluation

| Metric              | RAG Answer | Baseline |
|---------------------|------------|----------|
| Manual accuracy     | 3/3        | 1/3      |
| Avg. tokens used    | 76         | 39       |
| Fluency             | High       | Med–Low  |

The RAG responses were more accurate and grounded in actual procedural steps from WikiHow.

## 5. Files Included

| File                      | Description                              |
|---------------------------|------------------------------------------|
| `wikihow_rag_bot.ipynb`   | Fully executable Colab notebook          |
| `technical_summary.pdf`   | Architecture, implementation, evaluation |
| `business_brief.pdf`      | Value prop, user need, product framing   |

## 6. How to Run
1. Open `wikihow_rag_bot.ipynb` and hit Run.
No API keys, no GPU required. Everything runs in-browser.

## 7. Connect with me!
[Rashmila Mitra - GitHub](https://github.com/rmitra97)

[Rashmila Mitra - LinkedIn](https://www.linkedin.com/in/rashmilamitra/)

