# 🌍 Task 1: Language Translation Tool

## 📋 Project Overview
This project implements a **Language Translation Tool** as part of my internship at **CodeAlpha (Artificial Intelligence Intern)**.  
The tool allows users to **translate text between multiple languages**, listen to the translated text using **Text-to-Speech (TTS)**, and conveniently copy translations using a **Copy to Clipboard** button.  

Built with:
- 🐍 **Python**
- 🔎 **Deep Translator** (Google Translate backend)
- 🎙 **gTTS (Google Text-to-Speech)**
- 🎨 **Gradio** (User Interface)

---

## 🚀 Features
- ✏️ Enter text and select **source** & **target** languages  
- 🔄 **Instant translation** with Deep Translator  
- 🔊 **Text-to-Speech (TTS)** support to listen translations  
- 📋 **Copy to Clipboard** button for convenience  
- 🌐 Simple and interactive **Gradio web interface**  

---

## 📂 Dataset / API
- This project **does not require a dataset**.  
- It uses **Google Translate API (via Deep Translator library)** for translations.  

---

## ⚙️ Installation & Setup
Run this project in **Google Colab** or your local environment.  

### 1. Install Dependencies
```bash
pip install deep-translator gTTS gradio




2. Run the App
import gradio as gr
from deep_translator import GoogleTranslator
from gtts import gTTS


Use the provided notebook/script to launch the Gradio interface.

🖥️ Usage

Select Source and Target languages.

Enter the text you want to translate.

Click Translate → translation appears.

Click 🔊 Text-to-Speech → listen to translated text.

Click 📋 Copy to Clipboard → copy translated text.

🎥 Demo

👉 Add Colab Notebook link or Screenshot here

📌 Example

Input (English → Urdu):

How are you?


Output:

آپ کیسے ہیں؟

📚 Technologies Used

Python

Deep Translator

gTTS (Google Text-to-Speech)

Gradio

✨ Optional Enhancements

🌐 Auto-detect source language

🎨 Enhanced UI styling

📱 Deploy as a web app