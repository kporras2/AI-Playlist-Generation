# Spotify Playlist Generation using Machine Learning 🎶  

This project explores how **machine learning** can be applied to **playlist generation**, combining both **audio features** (danceability, tempo, valence, etc.) and **lyrics-based mood clustering**. The goal is to recommend songs by predicting musical attributes and grouping them by emotional similarity.  

Developed as part of **UTEP CS 5361 – Machine Learning**.  

---

## 🚀 Features
- Preprocessing of **Spotify audio features** and **song lyrics**  
- Lyrics vectorization using **TF-IDF**  
- Mood-based clustering with **KMeans**  
- Prediction of music attributes using:
  - **K-Nearest Neighbors (KNN)**
  - **Dense Neural Network (DNN)**
- Model performance comparison (MAE & MSE)  
- Simple feedback logging system for refining results  

---

## 📂 Project Structure
- `PlaylistGenerationUsingML.ipynb` → Jupyter notebook with full workflow  
- **Sections inside notebook**:
  1. Load datasets  
  2. Clean and preprocess audio + lyrics  
  3. Feature extraction & clustering  
  4. Model training (KNN, DNN)  
  5. Evaluation & visualization  
  6. User feedback logging  

---

## 📊 Datasets

This project requires **two CSV datasets**:

1. **Music Dataset (Spotify Audio Features)**  
   - Contains numerical/audio attributes from Spotify’s API.  
   - Example columns:
     ```
     track_name, track_artist, danceability, energy, key, loudness,
     mode, speechiness, acousticness, instrumentalness, liveness,
     valence, tempo
     ```

2. **Lyrics Dataset**  
   - Contains the corresponding **lyrics** for songs.  
   - Example columns:
     ```
     track_name, track_artist, text
     ```

> ⚠️ **Note**: Due to copyright, datasets are **not included in this repository**.  
You will need to provide your own Spotify audio features (via the Spotify API or Kaggle datasets) and a lyrics dataset.  

When running in **Google Colab**, you’ll be prompted to upload both CSV files.  

---

## 🛠️ Installation
Clone the repo and install dependencies:  
```bash
git clone https://github.com/yourusername/playlist-generation-ml.git
cd playlist-generation-ml
pip install -r requirements.txt
