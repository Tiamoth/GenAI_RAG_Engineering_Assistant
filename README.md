# 🤖 GenAI RAG Engineering Assistant (OCI Certified Skill)

## Project Overview

This project implements a secure, end-to-end **Retrieval-Augmented Generation (RAG) system** to solve the common engineering problem of information retrieval from massive documents. The goal is to eliminate **Large Language Model (LLM) hallucinations** by grounding all answers in a specific, trusted technical document (a 900+ page Arduino Reference PDF).

***

## 🛠️ Technology Stack & Achievements

This application is a direct showcase of integrating skills relevant to the **OCI Certifications** (Generative AI, Vector Search) with a real-world engineering challenge.

| Feature | Technology/Skill | Engineering Value |
| :--- | :--- | :--- |
| **Grounding & Accuracy** | LangChain, Custom Prompt Engineering | **Eliminates hallucinations.** System returns "Answer not found" if source data is insufficient, proving reliability. |
| **Vector Database** | **FAISS (Vector Search)**, HuggingFace Embeddings | Efficiently indexes 2,586 PDF chunks, enabling near-instantaneous semantic search. |
| **LLM Integration** | **Google Gemini API** (`gemini-2.5-flash`) | Synthesizes complex, technical answers into human-readable text. |
| **Security Best Practice** | Python `getpass` | **Crucial:** Demonstrates adherence to **API Key security** (credentials never hardcoded). |

***

## 📊 Final Results (Proof of Integrity)

This table summarizes your successful output, showcasing both accurate retrieval and integrity checks.

| Test Query | Output Answer | Proof |
| :--- | :--- | :--- |
| **Q1:** What is the correct syntax and function of the digitalRead command? | **A:** The `digitalRead()` function reads the value from a specified pin, returning either HIGH or LOW. Its syntax is `digitalRead(pin);`. | **Accurate Retrieval & Synthesis** |
| **Q2:** Can I use the analogWrite function on all digital pins? | **A:** The `analogWrite()` function **can only be used on certain digital pins** that are marked with a PWM symbol (~). | **Accurate Retrieval & Synthesis** |
| **Integrity Check:** (Question not in PDF) | **A:** `The specific answer could not be found in the provided Arduino reference documentation.` | **Proof of Reliability** |

***

## 🧑‍💻 Getting Started (How to Run Securely)

### Execution Steps
1.  **Prerequisites:** Obtain a **Gemini API Key** from [Google AI Studio](https://ai.google.dev/gemini-api/docs/api-key).
2.  **Run:** Open the `GenAI_RAG_Chatbot.ipynb` notebook in Google Colab.
3.  **Install Dependencies:** Run the cell containing the `!pip install` commands.
4.  **Set API Key (Securely):** The notebook will automatically use the secure `getpass` function to prompt you for your API key. **Enter it when prompted.**
