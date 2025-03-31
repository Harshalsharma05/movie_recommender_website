# Movie Recommendation Engine

This project is a movie recommendation engine built using **Streamlit**. It allows users to select a movie and receive recommendations based on similarity scores. The application fetches movie posters and displays them alongside the recommended movie titles.

🚀 **Live Demo:** [Click Here](https://movie-recommendation-system-ae6f.onrender.com/)

## 📂 Project Structure

- **`app.py`**: Main application code for the movie recommendation system.
- **`requirements.txt`**: Lists dependencies required for the project.
- **`README.md`**: Documentation with setup and deployment instructions.
- **`movies.pkl`**: Serialized file containing movie data.
- **`similarity_matrix.pkl`**: Serialized file storing similarity scores (loaded dynamically).

---
## 🚀 Local Setup Instructions

Follow these steps to run the application locally:

### 1️⃣ **Clone the Repository**
```bash
git clone <repository-url>
cd Movie_recommendation_engine
```

### 2️⃣ **Install Dependencies**
Ensure you have **Python 3.8+** installed. Then, install the required packages:
```bash
pip install -r requirements.txt
```

### 3️⃣ **Run the Application**
```bash
streamlit run app.py
```
This will start a local development server and open the application in your default browser.

---
## 🌍 Deployment on Render

You can deploy this project on **Render**, a free cloud platform for web applications.

### 1️⃣ **Create a Render Account**
- Sign up at [Render](https://render.com/).
- Verify your email and login.

### 2️⃣ **Create a New Web Service**
- Click on **"New"** → **"Web Service"**.
- Connect your **GitHub repository**.
- Select **Python** as the runtime.
- Choose the **region** closest to your audience.

### 3️⃣ **Configure Build Settings**
- **Build Command:**
  ```bash
  pip install -r requirements.txt
  ```
- **Start Command:**
  ```bash
  streamlit run app.py --server.port=10000 --server.address=0.0.0.0
  ```
- Set **Python version** (under environment settings) to **3.8+**.

### 4️⃣ **Deploy the Application**
- Click **"Deploy"** and wait for the process to complete.
- Open the **Render Live Link** to access your deployed app.

### 5️⃣ **Enable Auto-Deploy (Optional)**
- Navigate to **Settings**.
- Enable **Auto-Deploy** to update the app automatically when you push new changes.

---
## 🛠 Troubleshooting

- If the app **keeps downloading `similarity_matrix.pkl` on every request**, check if the file exists before downloading.
- If deployment **fails on Render**, ensure that:
  - Your **GitHub repository is public** (or use Render's private repo access).
  - `requirements.txt` has all dependencies.
  - Your **Start Command** is correctly set.

---
## 📜 License
This project is for educational purposes. Feel free to use and modify it!

For any issues, create an **issue** on GitHub or reach out!
