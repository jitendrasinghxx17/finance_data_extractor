# Financial Data Extractor

An AI-powered financial data extraction application built using Streamlit, LangChain, and Groq LLM.

## Overview

This project extracts important financial metrics such as:

* Revenue (Actual vs Expected)
* EPS (Actual vs Expected)

from financial news articles using Large Language Models (LLMs).

The extracted data is displayed in a clean tabular format using Streamlit.

---

# Tech Stack

* Python
* Streamlit
* LangChain
* Groq API
* Pandas
* dotenv

---

# Features

* Financial data extraction from news articles
* AI-powered JSON parsing
* Interactive Streamlit UI
* Revenue and EPS comparison table
* Environment variable support using `.env`

---

# Project Structure

```bash
finance_data_extractor/
│
├── main.py
├── data_extractor.py
├── requirements.txt
├── .gitignore
├── .env
└── README.md
```

---

# Installation

## 1. Clone Repository

```bash
git clone https://github.com/jitendrasinghxx17/finance_data_extractor.git
```

## 2. Navigate to Project Folder

```bash
cd finance_data_extractor
```

## 3. Create Virtual Environment

```bash
python -m venv venv
```

## 4. Activate Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

### Mac/Linux

```bash
source venv/bin/activate
```

---

# Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Setup Environment Variables

Create a `.env` file in the root directory.

```env
GROQ_API_KEY=your_api_key_here
```

Get your API key from:

[https://console.groq.com/](https://console.groq.com/)

---

# Run the Application

```bash
streamlit run main.py
```

The application will open in your browser at:

```text
http://localhost:8501
```

---

# Example Input

```text
Tesla reported revenue of $25 billion compared to expectations of $24 billion. EPS came in at $1.20 versus expected $1.10.
```

---

# Example Output

| Measure | Estimated   | Actual      |
| ------- | ----------- | ----------- |
| Revenue | $24 billion | $25 billion |
| EPS     | $1.10       | $1.20       |

---

# How It Works

1. User enters a financial news paragraph.
2. Streamlit sends the text to LangChain.
3. Groq LLM processes the article.
4. Financial metrics are extracted in JSON format.
5. Pandas creates a dataframe.
6. Streamlit displays the extracted information.

---

# Future Improvements

* PDF upload support
* CSV export
* Multi-article analysis
* Real-time financial APIs
* Data visualization charts
* RAG integration

---

# Author

Jitendra Singh

GitHub:
[https://github.com/jitendrasinghxx17](https://github.com/jitendrasinghxx17)

---

# License

This project is for educational and learning
