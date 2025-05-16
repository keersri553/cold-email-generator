# Cold-email-generator
## 🚀 Job Matcher & Email Automation

This project automates the process of matching resumes to job descriptions and composing tailored emails to recruiters. It leverages LLMs, ChromaDB vector store, and resume parsing to streamline cold outreach for job seekers.

---

## 📌 Features

- 🔍 Extracts key information from job descriptions (role, skills, experience).
- 📄 Matches the job with relevant resumes based on skill vectors.
- ✉️ Generates professional cold emails tailored to the job.
- 🌐 Provides links to the most relevant resume.
- 🧠 Uses LLMs (LLaMA3 via Langchain-Groq) for intelligent reasoning and text generation.
- 🗂 Stores resume data in a ChromaDB vector store.

---

🔧 Setup Instructions
Clone this repository to your local system.

Ensure Python 3.8+ is installed.

Install dependencies using pip install -r requirements.txt, or manually install: chromadb, langchain, langchain-core, python-dotenv, and pandas.

Create a .env file in the root directory.

Inside .env, add GROQ_API_KEY=your_api_key_here (replace with your Groq API key).

Ensure you have a CSV file named resumes.csv containing columns Skills and Resume_Link.

Run the script using python app.py (or your script file name).

🧠 How to Get a Groq API Key
Visit https://console.groq.com/

Sign in or sign up for an account.

Go to the API section and create a new API key.

Copy the key and paste it in your .env file under GROQ_API_KEY.

📁 Project Contents
app.py – Main Python script for running the pipeline.

resumes.csv – Input file with resume skill data and links.

.env – Hidden file for storing the Groq API key (not to be committed).

vectorstore/ – Directory created by ChromaDB for persistent storage.

🔒 Security Best Practices
Never commit .env or your Groq API key to version control.
