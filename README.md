# 🤖 AI-Assent Healthcare Chatbot  

A healthcare-focused chatbot that helps users by:  
- 🩺 Analyzing symptoms  
- 📖 Providing information about diseases  
- 💊 Suggesting medicines for treatment  

The goal is to create a **simple yet effective chatbot** that reduces typing effort for users. Instead of long conversations, users can quickly select options and provide only the necessary information to get results.  

---

## 📌 Project Overview  

The chatbot is built with **Python, Natural Language Processing (NLP), and Machine Learning**.  
While it does not use specialized healthcare APIs or datasets like MIMIC-III, it serves as a **beginner-friendly prototype** for exploring how chatbots can be developed from scratch.  

It offers **three main features**:  

---

### 1️⃣ Symptom Analysis  
- Users can enter their health symptoms.  
- The chatbot uses a **machine learning model** to predict the possible disease.  
- Dataset: doctor–patient conversations labeled with diagnoses.  
- **Preprocessing**: tokenization, stopword removal, and keyword extraction using NLP.  
- **Voting Classifier** implemented to improve accuracy:  
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - Multinomial Naive Bayes  
  - Random Forest Classifier  
- Final prediction = **majority voting** among classifiers.  
- Achieved **98.3% accuracy**.  
- A **word cloud visualization** shows the most common terms in the dataset.  

---

### 2️⃣ Disease Information  
- Users can look up any disease to get detailed information.  
- Uses the **Wikipedia Python library**, which supports:  
  - Searching articles  
  - Fetching summaries  
  - Extracting specific page sections  
- Input = disease/symptom query → results displayed → users select page to see **symptoms, treatments, precautions**, etc.  

---

### 3️⃣ Medicine Information  
- Users can search for medicines related to a disease.  
- Dataset: **11,000+ medicine details** (sourced from Kaggle, provided by 1mg pharmacy).  
- Each entry includes:  
  - Medicine composition  
  - Side effects  
- **TF-IDF Vectorizer + Nearest Neighbors (cosine similarity)** used to match diseases with medicines.  
- Nearest Neighbors ensures relevant medicines are found by comparing similarity in vector space.  

---

## 🖥️ User Interface  

- Built with **Streamlit** (Python framework for interactive web apps).  
- Provides a **chat-like interface** with buttons and sections.  
- Fast, simple, and user-friendly.  

---

## 🛠️ Tech Stack  

- **Python**  
- **NLP** → NLTK, Spacy  
- **Machine Learning** → Scikit-learn  
- **Wikipedia API**  
- **TF-IDF + Nearest Neighbors**  
- **Streamlit (GUI)**  

---

## 🚀 Conclusion  

This chatbot is not a production-level medical assistant but a **proof-of-concept project**.  
It demonstrates how **Machine Learning and NLP** can be combined to:  
- Analyze symptoms  
- Retrieve disease information  
- Suggest medicines  

It’s a starting point for building **more advanced healthcare chatbots** with real-world datasets and APIs.  

---

## 👉 Documentation Links  

- [Streamlit Docs](https://streamlit.io)  
- [Wikipedia Python Library](https://pypi.org/project/wikipedia/)  


---
The screenshots attached below demonstrate the working of the chatbot
<img width="1904" height="1035" alt="Screenshot 2025-09-02 204646" src="https://github.com/user-attachments/assets/229b7cd8-165c-4467-a7fb-6aacc963d1ec" />
<img width="1902" height="1030" alt="Screenshot 2025-09-02 204908" src="https://github.com/user-attachments/assets/8bdb76f0-710c-46a9-81b6-f507272ab6a7" />
<img width="913" height="530" alt="Screenshot 2025-09-02 205241" src="https://github.com/user-attachments/assets/b84dd1b2-db02-483d-b63e-9ac0f7d938fe" />


