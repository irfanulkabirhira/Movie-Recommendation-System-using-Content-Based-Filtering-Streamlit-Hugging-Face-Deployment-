# Movie-Recommendation-System-using-Content-Based-Filtering-Streamlit-Hugging-Face-Deployment-
A content-based Movie Recommendation System built with Streamlit and deployed on Hugging Face Spaces. Uses a similarity matrix with MovieLens dataset and fetches movie posters via TMDB API to provide Top-5 personalized movie suggestions.

# 🎬 Movie Recommendation System (Streamlit + Hugging Face)

## 📌 Overview
This is a **Movie Recommendation System** built with **Streamlit** and deployed on **Hugging Face Spaces**.  
It recommends **Top-5 movies** similar to a selected movie using a **content-based filtering approach** powered by a **similarity matrix**.  
Posters are fetched dynamically via the **TMDB API**.

🔗 Live Demo: [Hugging Face Space](https://huggingface.co/spaces/erfanulkabirhira/DataSynthis_Job_task)

---

## 🚀 Features
- Content-based recommendation (similarity matrix)
- Movie posters fetched from TMDB API
- Interactive UI built with Streamlit
- Lightweight and fast deployment on Hugging Face Spaces

---
pip install -r requirements.txt

📂 Project Structure
├── app.py              # Streamlit application
├── similarity.pkl      # Precomputed similarity matrix
├── movie_list.pkl      # Movie metadata
├── requirements.txt    # Dependencies
├── README.md           # Project documentation

## 🛠️ Installation & Setup
Clone the repository:
```bash
git clone https://github.com/<your-username>/movie-recommendation-system-streamlit.git
cd movie-recommendation-system-streamlit

