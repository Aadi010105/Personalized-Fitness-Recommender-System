# 🧠 Personalized Fitness Recommender System

This repository contains a **data-driven personalized fitness recommendation system** built using **Python** and **Jupyter Notebook**.  
The project is designed to suggest the **best and most relevant exercises** for users based on their **fitness level**, **target muscle groups**, and **individual fitness goals**.

---

## 🚀 Project Overview

### 🎯 Goal:
Recommend tailored workout routines for each user based on:

- Fitness experience level  
- Target muscle group  
- Personal fitness goals  
- Workout difficulty  
- Body part focus  
- Workout frequency  
- Estimated calories burned  

---

### 📥 Input Features:
| Feature | Description |
|----------|--------------|
| **Experience Level** | Beginner / Intermediate / Advanced |
| **Target Muscle Group** | Chest, Legs, Back, Core, Full Body, etc. |
| **Difficulty Level** | Easy / Medium / Hard |
| **Body Part** | Upper / Lower / Core / Full |
| **Workout Frequency** | Days per week |
| **Calories Burned** | Estimated calories per session |

---

### 📤 Output:
A **personalized workout plan** containing:

- Exercise Name  
- Target Muscle Group  
- Difficulty Level  
- Estimated Calories Burned  
- *(Optionally: Equipment used and exercise benefits)*

---

## 🏗️ How It Works

### 🧹 Data Cleaning:
- Cleans and standardizes exercise names, target muscles, and difficulty labels.  
- Removes duplicates and missing values for accurate similarity scoring.  
- Normalizes calorie and muscle group data for uniformity.

### 🧩 Feature Engineering:
- Combines exercise metadata (target muscle, difficulty, calories) into structured features.  
- Generates textual and numerical embeddings for similarity computation.

### 💪 Recommendation Logic:
- Uses **TF-IDF vectorization** and **Cosine Similarity** to recommend exercises similar to a user’s input.  
- Allows user-based filters (goal, difficulty, muscle group).  
- Includes a **fuzzy matching** fallback for broader recommendations.  
- Adds variety based on **calorie intensity** (light, medium, intense).  
- Ensures diversity in results through randomized tie-breaking.

### 💾 Model Export:
- Supports exporting the trained recommender model as a `.pkl` file using Python’s pickle library.  
- Enables easy deployment or integration into web apps or APIs.

---
