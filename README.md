The AI Fake News Detection and News Aggregator is a web-based intelligent system that automatically collects news from online sources, analyzes the credibility of news articles, and classifies them as Real or Fake using state-of-the-art NLP and Machine Learning models.

This project combines news aggregation, AI-based fake news detection, and confidence scoring into a single platform, making it useful for students, researchers, journalists, and the general public.

Objectives

To detect fake news using Natural Language Processing (NLP) and Deep Learning models

To provide confidence scores and credibility labels

To aggregate and display news articles from multiple online sources

To compare predictions from different models (Admin view)

To build an easy-to-use Flask-based web interface

Key Features

🔍 Fake News Detection (Real / Fake classification)

📊 Confidence Score & Credibility Label

🌐 News Aggregation from URLs

🤖 Pre-trained Transformer Models

👤 User Dashboard (HF Model)

🛠️ Admin Dashboard (BERT vs HF Comparison)

⚡ Fast prediction with optimized inference

🔐 Secure authentication for admin access

🧠 Technologies Used
Programming & Frameworks

Python

Flask

HTML, CSS, JavaScript

Machine Learning & NLP

BERT (Local Model – Admin)

RoBERTa (Pre-trained Hugging Face Model)

Hugging Face Transformers

NLTK

Libraries & Tools

Pandas, NumPy

Torch (PyTorch)

BeautifulSoup

Newspaper3k

Requests

MongoDB (for user/admin data, if enabled)

🏗️ System Architecture

User inputs a news URL or text

News content is extracted and cleaned

Text preprocessing & tokenization

Prediction using AI models

Confidence score calculation

Credibility label generation

Results displayed on dashboard

📂 Project Structure
AI-Fake-News-Detection/
│
├── app.py
├── model_utils.py
├── config.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── Fake.csv
│   ├── True.csv
│
├── models/
│   ├── bert_model/
│   ├── tokenizer/
│
├── templates/
│   ├── index.html
│   ├── user_dashboard.html
│   ├── admin_dashboard.html
│   ├── login.html
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/

🔑 Models Used
1️⃣ Hugging Face RoBERTa Model (User Dashboard)

Model: hamzab/roberta-fake-news-classification

Advantages:

High accuracy

Fast inference

No local training required

2️⃣ BERT Model (Admin Dashboard)

Locally trained BERT model

Used for comparison and evaluation

Provides insight into model behavior differences

📊 Output Details

Prediction: Real / Fake

Confidence Score: Percentage probability

Credibility Score: Numerical reliability measure

Credibility Label:

High (Real)

Medium (Uncertain)

Low (Suspicious)

🧪 Dataset Used

WELFake Dataset

Combined datasets:

Fake.csv

True.csv

Preprocessed to remove noise, duplicates, and missing values

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/Divya-Gupta17/AI-Fake-News-Detection-System.git
cd ai-fake-news-detection

2️⃣ Create Virtual Environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Run the Application
python app.py

5️⃣ Open in Browser
http://127.0.0.1:5000

🧑‍💻 Usage

Users:

Paste a news URL or text

View prediction, confidence, and credibility

Admin:

Login with admin credentials

View HF vs BERT prediction comparison

Analyze model performance

📈 Results & Performance

High accuracy on benchmark fake news datasets

Hugging Face model provides faster inference

BERT model useful for detailed evaluation and comparison

🔮 Future Enhancements

Multilingual fake news detection

Real-time social media news analysis

Explainable AI (XAI) visualization

Browser extension integration

Improved credibility scoring using source reputation
