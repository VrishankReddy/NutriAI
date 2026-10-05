# NutriAI

NutriAI is a simple AI application that scans food package photos to read the ingredients and tell you how healthy they are.

---

## How It Works

1. **Object Detection**: A YOLOv8 model finds and crops the ingredient list from your photo.
2. **Text Extraction**: EasyOCR reads the text from the cropped image.
3. **AI Analysis**: A local AI model (Mistral via Ollama) reviews the ingredients, gives it a health score, and highlights any risks.
4. **Web App**: A clean Streamlit interface shows you the results instantly.

---

## Setup Guide

1. **Install requirements**:
   ```bash
   pip install -r requirements.txt

2. **Run Ollama (make sure Mistral is installed)**:
   ```bash
   ollama run mistral

3. **Start the app:**:
   ```bash
   streamlit run app.py