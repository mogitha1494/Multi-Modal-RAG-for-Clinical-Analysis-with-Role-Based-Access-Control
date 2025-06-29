
# Multi-Modal RAG for Clinical Analysis with RBAC

A secure, multimodal healthcare analysis system using Retrieval-Augmented Generation (RAG) and Role-Based Access Control (RBAC). It enables authenticated access to clinical data like X-rays, reports, and notes, powered by FLAVA, FAISS, and LLMs for smart medical insights.

---

## Features

- Role-based access to sensitive medical data
- Multimodal embedding using FLAVA (Image + Text)
- Fast similarity search with FAISS
- Summarized output using LLM (Gemini)
- Evaluated using stakeholder survey and benchmark models

---

## Model Comparison

| Model | Text-Image Embedding Accuracy | Multimodal Alignment | Response Relevance |
|-------|-------------------------------|----------------------|--------------------|
| **FLAVA** | ⭐⭐⭐⭐☆ | Strong | High |
| CLIP  | ⭐⭐⭐☆☆ | Moderate | Medium |

FLAVA outperformed CLIP in generating accurate and relevant embeddings for multimodal medical data (X-ray + report) .

---

## User Satisfaction Survey

A usability survey was conducted with **50 stakeholders** (doctors, nurses, patients).

- 80% found the system **easy to use**
- 76% agreed access control was **robust and secure**
- 84% rated the summaries as **clinically useful**
- Feedback guided **future enhancements** like broader modality support and audit logging

---

## Tech Stack

- Python 3.8+
- PyTorch
- FAISS
- Transformers
- Google Colab
- FLAVA (Meta AI)
- Gemini (LLM API)
- Indiana Chest X-ray dataset (Kaggle)

---

## Setup Instructions (Google Colab)

1. **Open the file in Colab**
   
2. **Upload the dataset**  
   Download the [Indiana University Chest X-ray dataset](https://www.kaggle.com/datasets/nih-chest-xrays/data) from Kaggle and upload it to your Colab session or mount from Google Drive.

3. **Install dependencies**
   ```python
   !pip install faiss-cpu transformers torch
   ```

4. **Run the cells and follow instructions**
   The notebook guides you through loading embeddings, running FAISS search, and generating secure summaries.

---

## Sample Input/Output

### Input

```json
{
  "username": "dr.susan",
  "role": "doctor",
  "aadhar_id": "XXXX-XXXX-1234",
  "input": "Chest X-ray image + recent symptoms"
}
```

###  Output

```json
{
  "summary": "The patient shows signs of pulmonary fibrosis. Historical data reveals prior TB infection. Recommended to conduct CT scan for confirmation. Prescribed: Inhaled corticosteroids."
}
```

---

##  Directory Structure

```
├── RAG_Multi_modal_Implementation.ipynb
├── requirements.txt       # For local use (optional)
└── README.md
```

## Authors

* Prahalyaa A
* Mogitha S M
* Harini Priyanka W

Department of Computer Science and Engineering,
Amrita Vishwa Vidyapeetham, Coimbatore

---

## License

This project is licensed under the MIT License.




