# 🎬 Movie Recommender System

A personalized **Movie Recommender System** built using Python, Streamlit, and machine learning. This project suggests movies based on user preferences using content-based filtering and vector similarity techniques.

> 🚀 **Live Demo:** [Click here to try it!](https://movierecommendersystem-mszxnh7pxaovfae8azxrmd.streamlit.app/)

---

## 📌 Features

- Recommend similar movies based on your favorite selection
- Search functionality to find and explore movie details
- Clean and interactive **Streamlit web interface**
- Lightweight and fast — perfect for demos and academic purposes

---

## 🛠️ Tech Stack

- **Python 3.11**
- **Streamlit**
- **Pandas, Scikit-learn**
- **Numpy**
- **Pickle** (for loading precomputed similarity matrix)
- **NixOS** (for development environment)

---

## 📁 Project Structure

movie_recommender_system/
├── .gitattributes
├── .gitignore
├── app.py # Main Streamlit app file
├── gitignore # (Duplicate, optional to delete)
├── movies_dict.pkl # Pickled dictionary of movies
├── requirements.txt # Python dependencies
├── shell.nix # Nix environment file (for NixOS users)
└── similarity.pkl # Pickled cosine similarity matrix.

---

## ⚙️ Installation

### For Any OS (using Python virtual environment):

```bash
# Clone the repo
git clone https://github.com/PrateekKumarH/movie_recommender_system.git
cd movie_recommender_system

# Create and activate virtual environment
python3 -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py

---
##If you're using Nix/NixOS:
nix-shell shell.nix
streamlit run app.py

---

##How it Works

Uses a cosine similarity matrix based on movie descriptions or genres

Loads this matrix using pickle for performance

When a user selects a movie, the app fetches the most similar movies from the matrix

---

##💡 Future Improvements

Add collaborative filtering

Integrate external APIs (e.g., TMDb) for richer movie data

Enable user ratings and feedback loop

---

## 📄 License

This project is for academic/demo purposes. Feel free to fork and adapt!
