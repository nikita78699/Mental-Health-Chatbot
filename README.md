# 🧠 Mental Health Chatbot for Employee Well-being

This project aims to build an intelligent system that supports employee mental health by identifying stress indicators and offering empathetic responses and mood-based music recommendations using NLP and machine learning.

---

## 🎯 Objectives

The core goals of the system are:

- Identify mental health issues in employees based on behavioral and demographic data.
- Enable mental health prediction and classification using deep learning models.
- Develop a conversational AI assistant that can engage with users empathetically.
- Suggest music based on the user's emotional state to provide a calming experience.

---

## ✅ Phase I 

### 1. **Data Collection**
- Historical employee data collected, including:
    - Demographics
    - Job-related attributes (e.g., workload, role, hours)
    - Mental health indicators (e.g., stress levels, absenteeism)

### 2. **Data Preprocessing**
- Cleaned missing and duplicate values
- Normalized data for model compatibility

### 3. **Model Development**
- Built a BERT-based classification model to detect likelihood of:
    - **Depression**
    - **Anxiety**
    - **Frustration**
    - **Stress**

### 4. **Classification**
- Trained and tested the model to classify employees into mental health categories based on input features

---

## 🚧 Phase II 

- Build a basic NLP-based chatbot for mental health conversations
- Integrate sentiment analysis and song recommendation engine
- Combine prediction model and chatbot into a unified, user-friendly interface

---

## 🤖 Part 1: Mental Health Chatbot

### 🔹 Intent Recognition & Text Processing

- Uses a **pre-trained neural network model** (`chatbot_model.h5`) for intent classification
- Text preprocessing includes:
    - Tokenization
    - Lemmatization
    - "Bag of Words" vectorization

### 🔹 Prediction

- The bag-of-words input is passed to the neural network to predict the most likely **intent class**
- A **probability distribution** is returned and the highest scoring intent is selected

### 🔹 Response Generation

- Based on the predicted intent, a **random response** is chosen from the mapped list in `intents.json`
- Adds conversational variability while staying contextually relevant

---

## 🎵 Part 2: Music Recommendation Based on Mood

- Applies **sentiment analysis** using NLP on user input
- Suggests songs tailored to the detected emotional tone (e.g., calm, energetic, sad)
- Matches user mood with genres to enhance relaxation or motivation

---

## 📁 Dataset Description

The chatbot was trained on a **custom dataset** of mental health conversations that include:

- **Casual chats**
- **Common mental health questions**
- **Therapy-style conversations**
- **Supportive advice**

### Intent Structure

The dataset is based on **intent modeling**, where each intent includes:

| Key         | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `tag`       | Category of the intent (e.g., `greeting`, `sad`, `anxiety`)               |
| `patterns`  | Example user inputs for that intent (e.g., "Hi", "I'm feeling down")       |
| `responses` | Bot responses mapped to each intent (e.g., "I'm here for you", "Stay strong") |

This structure helps the chatbot provide **empathetic and intelligent replies**, mimicking basic therapeutic dialogue.

---

## 🔧 Tech Stack

- **Python**
- **TensorFlow / Keras** (for model training)
- **NLTK** (for preprocessing)
- **JSON** (for storing intents)
- **Sentiment Analysis** (for mood detection)
- **BERT** (for mental health prediction model)

---

## 🙋‍♀️ Author

**Nikita Singhal**  
Full-stack Developer | AI Enthusiast | Mental Health Advocate  
[GitHub Profile](https://github.com/nikita78699)

---

