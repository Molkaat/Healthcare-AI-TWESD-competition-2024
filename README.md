# 🩺 Chest X-ray Report Generation with ViT-GPT2  

This project was developed for the **TWESD Healthcare AI Competition 2024**.  
It focuses on **automatically generating diagnostic reports from chest X-ray images** by combining **computer vision** and **natural language processing** in a multimodal encoder–decoder architecture.  

👉 The trained model is available on Hugging Face: [Molkaatb/ChestX](https://huggingface.co/Molkaatb/ChestX)  

---

## 🚀 Project Overview  
- **Objective:** Assist radiologists by generating **medical text reports** directly from chest X-rays.  
- **Approach:**  
  - **Vision Transformer (ViT)** as the **image encoder**.  
  - **GPT-2** as the **text decoder**.  
  - Connected in a **VisionEncoderDecoderModel** architecture.  
- **Training:** Fine-tuned on the **Indiana University Chest X-ray dataset** (findings + corresponding images).  
- **Evaluation:** Used **BLEU score** to assess generated report quality.  

---

## 🧠 Key Features  
- End-to-end **encoder–decoder multimodal learning**.  
- Fine-tuned **transformer models** for healthcare.  
- Data preprocessing and dataset handling from Indiana X-ray dataset.  
- Report generation pipeline with **training, evaluation, and inference**.  
- Model checkpoint pushed to Hugging Face for reuse.  

---

## 📂 Repository Structure  
.
├── MedAI_team.py # Competition submission script
├── report_gen_vit_gpt2.py # Full training & evaluation pipeline
└── README.md # Project documentation

---

## 🛠️ Technologies Used  
- Python  
- PyTorch  
- Hugging Face Transformers  
- Vision Transformer (ViT)  
- GPT-2  
- Scikit-learn / Pandas / NLTK  

---

## ⚙️ Usage  

### 1️⃣ Installation  
```bash
pip install torch torchvision transformers datasets nltk
