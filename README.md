# 🎬 Movie Recommendation System

A simple movie recommendation system built with **Streamlit** and deployed on **Hugging Face Spaces**.

## 🚀 Features
- Select a movie from dropdown
- Get top 5 recommended movies with posters
- Uses TMDB API to fetch movie posters

## 📦 Run Locally
```bash
streamlit run app.py

---

### 4. Deploy on Hugging Face
1. Go to [Hugging Face Spaces](https://huggingface.co/spaces).
2. Click **New Space**.
   - Name: `movie-recommendation-system`
   - SDK: **Streamlit**
   - Visibility: Public (or Private if you prefer)
3. Upload these files:
   - `app.py`
   - `movie_list.pkl`
   - `similarity.pkl`
   - `requirements.txt`
   - (optional) `README.md`
4. Hugging Face will automatically install dependencies and run your app.

---

### 5. Check Logs if Error
If it doesn’t run, go to **Settings → Logs** and check for missing libraries. Then just add them to `requirements.txt`.

---

⚠️ One thing: your `app.py` uses **TMDB API Key**. Since it’s written directly in the code, anyone can see it.  
👉 Hugging Face lets you store **API keys securely** using **Secrets**. You can go to:
- **Settings → Repository secrets** → Add `TMDB_API_KEY`
- Then replace your code with:

```python
import os

API_KEY = os.getenv("TMDB_API_KEY")
response = requests.get(f'https://api.themoviedb.org/3/movie/{movie_id}?api_key={API_KEY}')
