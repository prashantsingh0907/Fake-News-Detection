📰 Fake News Detection using Machine Learning
This project is a machine learning-based application that detects whether a news article is real or fake using Natural Language Processing (NLP) techniques and a Passive Aggressive Classifier.

It leverages a cleaned dataset from Kaggle containing thousands of real and fake news articles. The raw text is preprocessed and converted into numerical features using TF-IDF vectorization, then fed into the classifier to learn patterns and detect misinformation.

The goal is to provide a lightweight, interpretable model that can be deployed as a web app using Streamlit, allowing users to input a news headline or paragraph and get a prediction instantly.

This project showcases:

End-to-end pipeline: from data cleaning and model training to deployment
A simple GUI for user interaction
Easy customization for any text classification problem


📌 Features
Cleaned dataset from Kaggle (Fake.csv and True.csv)
TF-IDF Vectorization for feature extraction
Passive Aggressive Classifier for classification
Model saved using pickle
GUI built with Streamlit
Easy to use, train, and extend


📂 Project Structure
Fake News Detection/
├── app.py # Streamlit web app
├── data/
│ ├── True.csv
│ └── Fake.csv
├── models/
│ ├── fake_news_model.pkl
│ └── tfidf_vectorizer.pkl
├── fake_news_detection.ipynb # Jupyter Notebook with full training steps
├── predict.py # CLI-based usage (optional)
├── requirements.txt # Project dependencies
├── README.md # Project documentation
└── venv/ # Virtual environment (excluded from GitHub)


🔍 Dataset
Source: Kaggle: Fake and Real News Dataset
Fake.csv: Fake news articles
True.csv: Real news articles


🚀 How to Run the App
✅ Step 1: Clone the Repository
git clone https://github.com/Prashantsingh0907/Fake-News-Detection.git
cd Fake-News-Detection
✅ Step 2: Create and activate a virtual environment
For Windows:
python -m venv venv
venv\Scripts\activate
For macOS/Linux:
python3 -m venv venv
source venv/bin/activate
✅ Step 3: Install required Python libraries
pip install -r requirements.txt
✅ Step 4: Launch the Streamlit GUI
streamlit run app.py
