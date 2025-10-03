
# Medical-Evidence-Synthesizer
### A Multimodal Diagnostic RAG for Complex Patient Cases

---

### **Project Overview**
For our final semester long project, we will develop a comprehensive tutorial on building a clinical decision support tool called the "Medical Evidence Synthesizer." This project will guide users through the data science pipeline to create a Retrieval Augmented Generation (RAG) model. The model will ingest complex, de-identified patient data combining structured lab results and unstructured clinical notes to generate a differential diagnosis. A key feature of this tool is its ability to provide verifiable, citable evidence for each diagnostic possibility directly from the source data, showcasing an end-to-end data science solution with a focus on machine learning and explainability.

---

### **Course Information**
- **Course:** DATA 602: Principle of Data Science - Fall 2025
- **Instructor:** Dr. Fardina Alam
- **Section:** PSC2

---

### **Team Members**
- Shradha Anand
- Ryan Kemajou
- Lei Mao

---

### **Objectives**
- Develop a RAG model for differential diagnosis.
- Integrate multimodal data (structured and unstructured).
- Provide verifiable evidence for diagnoses.
- Create a comprehensive tutorial for the process.

---

### **Dataset**
- **Name:** MIMIC-IV (Medical Information Mart for Intensive Care IV)
- **Citation:**
  - **MIMIC-IV Dataset:** Wang, B., Chang, J., & Qian, Y. (2025). *MIMIC-IV-Ext-DiReCT* (version 1.0.0). PhysioNet. RRID:SCR_007345. [https://doi.org/10.13026/yf96-kc87](https://doi.org/10.13026/yf96-kc87)
  - **PhysioNet Platform:** Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P. C., Mark, R., ... & Stanley, H. E. (2000). *PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals*. Circulation [Online], 101(23), e215–e220. RRID:SCR_007345.
- **Rationale:**
  - **Richness and Complexity:** Large-scale, real-world ICU patient data ideal for advanced analysis.
  - **Multimodal Data:** Contains both structured (e.g., `labevents`) and unstructured (e.g., `noteevents`) data.
  - **Direct Project Alignment:** Enables the core research question of synthesizing multimodal clinical data for evidence-backed diagnosis.
  - **Ethical Considerations:** Utilizes a de-identified dataset, addressing patient privacy concerns.

---

### **Tools & Libraries**
- **Programming Language:** Python
- **Data Science Libraries:** pandas, numpy, scikit-learn
- **LLM & RAG Libraries:** Hugging Face Transformers, LangChain, LightRAG
- **Deep Learning Frameworks:** PyTorch
- **Notebook Environment:** Jupyter
- **Data Source:** MIMIC-IV

---

### **Proposed Project Structure**
```
├── data/
│   ├── raw/
│   │   └── MIMIC-IV/
│   ├── processed/
│   │   └── preprocessed_data.csv
│   └── external/
├── notebooks/
│   ├── 1_data_exploration.ipynb
│   ├── 2_preprocessing.ipynb
│   ├── 3_model_development.ipynb
│   ├── 4_rag_implementation.ipynb
│   └── 5_evaluation.ipynb
├── scripts/
│   ├── download_data.py
│   ├── preprocess_data.py
│   ├── train_model.py
│   └── evaluate_model.py
├── src/
│   ├── __init__.py
│   ├── data/
│   │   ├── __init__.py
│   │   └── MIMIC_loader.py
│   ├── models/
│   │   ├── __init__.py
│   │   ├── rag_model.py
│   │   └── llm_integration.py
│   ├── utils/
│   │   ├── __init__.py
│   │   └── text_processing.py
│   └── main.py
├── tests/
│   ├── __init__.py
│   ├── test_data.py
│   └── test_models.py
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```
