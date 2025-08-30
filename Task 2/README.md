# 🤖 Task 2: FAQ Chatbot

## 📋 Project Overview
This project implements an **FAQ Chatbot** that automatically answers user queries by matching them to the most relevant **Frequently Asked Questions (FAQs)**.  
It uses **TF-IDF vectorization** and **cosine similarity** to find the closest matching question and return the correct answer.  

Additionally, it provides an **interactive Gradio interface** where users can:
- View a list of FAQs  
- Ask their own questions  
- Get instant responses from the chatbot  

---

## 🚀 Features
- 📌 Predefined list of FAQs and answers  
- 🧠 NLP-based similarity matching using **TF-IDF** and **cosine similarity**  
- ✅ Handles unknown questions gracefully  
- 🎨 User-friendly **Gradio interface** with:
  - Left panel showing available FAQs  
  - Right panel with input box and chatbot response  

---

## 🛠️ Tech Stack
- **Python**  
- **NLTK** → for text preprocessing  
- **Scikit-learn** → for TF-IDF & cosine similarity  
- **Gradio** → for interactive web interface  

---

## 📂 Dataset
The chatbot uses a small predefined FAQ dataset, for example:

| Question | Answer |
|----------|--------|
| What is CodeAlpha? | CodeAlpha is an organization offering internships in AI, ML, and web development. |
| How can I apply for an internship at CodeAlpha? | You can apply through the official CodeAlpha website or via internship platforms. |
| Is the internship paid? | CodeAlpha internships are generally unpaid, but they provide valuable learning experience and certificates. |
| What skills do I need for the AI internship? | You should know Python, basic ML, and libraries like pandas, numpy, sklearn. |
| Do I get a certificate after internship? | Yes, CodeAlpha provides an official certificate after successful completion of the internship. |

---

## ▶️ How to Run
1. Install dependencies:
   ```bash
   pip install nltk scikit-learn gradio


Run the script:

python faq_chatbot.py


A Gradio app will launch in your browser.

Left panel → FAQs list

Right panel → Ask questions & get answers

📽️ Demo (Google Colab Recommended)

This project can be easily executed in Google Colab.
Just upload the notebook and run all cells to interact with the chatbot in real-time.

✨ Optional Enhancements

Add chat history for a conversational feel

Include text-to-speech (TTS) responses

Expand FAQ dataset

Integrate with a database or API for dynamic FAQs

🏆 Outcome

A lightweight and interactive FAQ Chatbot that helps users quickly find answers to common questions while showcasing NLP + Gradio integration.