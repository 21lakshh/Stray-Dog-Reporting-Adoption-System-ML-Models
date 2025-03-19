# 🐶 AI-Based Hotspot Detection & Dog Condition Verification - Stray Dog Reporting System

This module is responsible for detecting and prioritizing hotspots where multiple stray dog reports are received. Additionally, it includes an AI-based system for verifying the presence of a dog in an image and assessing its condition. It also integrates a RAG-based QnA bot for assisting users in filling out adoption forms.

---

## 🚀 How It Works?
### 🔥 Hotspot Detection:
- The system monitors all reported stray dog incidents in real-time.
- If multiple reports originate from a specific location, it is classified as a **hotspot**.
- A **hotspot priority system** ensures urgent cases are flagged:
  - High-priority hotspots are marked when multiple reports appear in a short period.
  - Uses **DBSCAN clustering algorithm** to detect high-density areas.
- Shelters & hospitals can visualize hotspots using a **live heatmap**.

### 🐶 Dog Verification & Condition Assessment:
- AI model verifies whether an uploaded image contains a dog.
- If a dog is detected, its condition is classified into one of four categories:
  - 🟢 **Healthy**
  - 🟡 **Mildly Injured/Sick**
  - 🟠 **Moderately Injured/Sick**
  - 🔴 **Critical Condition**
- The model is trained using deep learning (CNN-based) to assess visible injuries and overall health.

### 🏡 RAG-Based QnA Bot regarding Adoption form:
- **LangChain** (Retrieval-Augmented Generation framework)
- **OpenAI / Hugging Face Models** (For NLP-based QnA)
- **Vector Database (ChromaDB)** (Stores FAQs for adoption assistance)
---
