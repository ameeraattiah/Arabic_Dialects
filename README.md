# Arabic Dialect Classification & Dialectness Scoring

This repository contains the code, datasets, and models developed during my internship at **KAUST’s Center of Excellence for Generative AI**.  
The project focuses on **multi-task learning for Arabic dialect identification and continuous dialectness scoring**.

---

## 📌 Project Overview

- **Goal**: Improve Arabic NLP by developing multi-label dialect classifiers with integrated dialectness scoring.  
- **Approach**:  
  - Sentence-level classification  
  - Token-level classification with MARBERT  
  - Multi-task learning: classification (discrete labels) + regression (continuous dialectness score)  
- **Results**:  
  - Sentence-level F1 ≈ 0.90  
  - Token-level F1 ≈ 0.71  
  - Continuous scoring aligned with human-annotated AOC-ALDi dataset

---

## 📂 Repository Structure

```
├── Arabic_Dialects.ipynb        # Main notebook with full pipeline
├── Sentence_Level_v2.ipynb      # Sentence-level experiments
├── Token_Level_v3.ipynb         # Token-level experiments
├── dialect_documents.json       # Synthetic dialect dataset (5 dialects)
├── marbert_sentence_model.pt    # Trained MARBERT (sentence-level)
├── marbert_token_model.pt       # Trained MARBERT (token-level)
├── marbert_token_model_mixed.pt # Token-level model with mixed-dialect data
├── Poster.pdf                   # Internship poster
└── README.md                    # This file
```

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. Install dependencies (recommend using virtual environment):
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebooks in order:
   - `Arabic_Dialects.ipynb` (end-to-end pipeline)
   - `Sentence_Level_v2.ipynb` (sentence-level classification)
   - `Token_Level_v3.ipynb` (token-level classification)

---

## 📊 Datasets

- **QADI** – 18 dialects  
- **EMINES** – MSA baseline  
- **AOC-ALDi** – Human-annotated dataset with 5 dialects + dialectness scoring  
- **Synthetic dialect documents** (`dialect_documents.json`) – 500 documents across 5 dialects  

---

## 🏆 Results

- **Sentence-Level (MARBERT)**:  
  - F1 (Micro/Macro): **0.898 / 0.899**  
  - MSE / MAE: **0.258 / 0.504**

- **Token-Level (MARBERT)**:  
  - F1 (Micro/Macro): **0.717 / 0.708**  
  - MSE / MAE: **0.099 / 0.253**

---

## 📜 Citation

If you use this work, please cite the internship poster:

```
Ameera Attiah, Zaid Alyafeai, Bernard Ghanem.
Multi-Task Learning for Arabic Dialect Classification & Scoring.
KAUST Center of Excellence for Generative AI, 2025.
```

---

## 👩‍💻 Author

**Ameera Attiah**  
Intern @ KAUST – Center of Excellence for Generative AI
