# Sentiment Analysis of Amazon Alexa Reviews

This is a Flask-based web application for sentiment analysis of Amazon Alexa product reviews. Users can input text manually or upload CSV files for batch analysis. The application processes the reviews using a trained machine learning model and displays sentiment results with visualizations.

## Features
- 🌟 **Sentiment Classification:** Classifies reviews as Positive 😊, Negative 😠, or Neutral 😐.
- 📂 **CSV Upload Support:** Allows bulk analysis by uploading CSV files.
- 📊 **Sentiment Visualization:** Generates bar charts to show sentiment distribution.
- 🎯 **User-Friendly Interface:** Built with HTML, CSS, and Flask.

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Flask (Python)
- **Machine Learning:** Pre-trained sentiment analysis model (Naive Bayes / SVM / Logistic Regression)
- **Data Visualization:** Matplotlib / Chart.js
- **Deployment:** Render / Heroku

## Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/sentiment-analysis-alexa.git
cd sentiment-analysis-alexa
```

### 2️⃣ Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application
```bash
python app.py
```
Access the app at **http://127.0.0.1:5000/**

## Usage
1. **Manual Input:** Enter text in the input box and get sentiment results.
2. **CSV Upload:** Upload a CSV file containing reviews. The app will detect the review column and analyze sentiments.
3. **Visualization:** View sentiment distribution in a bar chart.

## Deployment
### 🚀 Deploy on Render (Recommended)
1. **Push your code to GitHub.**
2. **Create an account on [Render](https://render.com/)**.
3. Click **"New Web Service"** → Connect GitHub repository.
4. Set:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `gunicorn app:app`
5. Click **"Deploy"** → Your app will be live!

### Deploy on Heroku (Alternative)
```bash
heroku login
heroku create sentiment-analysis-alexa
heroku git:remote -a sentiment-analysis-alexa
git push heroku main
heroku open
```

## Future Enhancements
- ✅ Improve UI with Bootstrap or React
- ✅ Add authentication for user-specific analysis
- ✅ Store results in a database (SQLite / PostgreSQL)

## Contributing
Feel free to submit issues or pull requests. Contributions are welcome!

## License
This project is licensed under the MIT License.

