# Multi-Modal-RAG-for-Clinical-Analysis-with-Role-Based-Access-Control
A secure, multimodal healthcare analysis system using Retrieval-Augmented Generation (RAG) and Role-Based Access Control (RBAC). It enables authenticated access to clinical data like X-rays, reports, and notes, powered by FLAVA, FAISS, and LLMs for smart medical insights.

---

## Features

- Role-based access to sensitive medical data
- Multimodal embedding using FLAVA (image + text)
- Fast similarity search with FAISS
- Summarized output using LLMs (e.g., Gemini)

---

## Tech Stack

- Python 3.8+
- PyTorch
- Transformers
- FAISS
- OpenAI/Gemini API
- Jupyter Notebook

---

##  Setup Instructions

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/multimodal-rag-clinical.git
   cd multimodal-rag-clinical
    ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/macOS
   venv\Scripts\activate     # For Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the notebook**

   ```bash
   jupyter notebook RAG_Multi_modal_Implementation.ipynb
   ```

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

### Output

```json
{
  "summary": "The patient shows signs of pulmonary fibrosis. Historical data reveals prior TB infection. Recommended to conduct CT scan for confirmation. Prescribed: Inhaled corticosteroids."
}
```

---

##  Directory Structure

```
├── RAG_Multi_modal_Implementation.ipynb
├── requirements.txt
└── README.md
```

---

## License

This project is licensed under the MIT License.

---

## Authors

* Prahalyaa A
* Mogitha S M
* Harini Priyanka W

Department of Computer Science and Engineering,
Amrita Vishwa Vidyapeetham, Coimbatore


