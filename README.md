# AI Email Assistant

An AI assistant that finds the right contacts from your data and writes personalized emails for them. You describe who you want to reach in plain English, and it searches your contacts by meaning, drafts the email with an LLM, and sends and logs it.

## What it does

- **Semantic contact search.** Ask for people in natural language and get ranked matches, even when your words don't appear in the data.
- **Adapts to your data.** It detects whether an uploaded file looks like contacts, company, school or sales data and weights the right fields (name, company, location) accordingly.
- **AI email writing.** Generates personalized emails with Groq-hosted LLMs, in the tone you choose (for example professional or friendly).
- **Bulk outreach.** Select several contacts and generate and send a personalized email to each one.
- **Multiple data sources.** Use contacts from CSV or Excel uploads, a MongoDB collection, or both, with per-source enable and priority settings.
- **Templates and history.** Save reusable email templates and keep a log of every email sent.
- **REST API and web UI.** A FastAPI backend with a Streamlit front end.

## Keywords

Generative AI · LLM · Groq · NLP · Semantic search · Sentence embeddings · Email automation · AI agent · FastAPI · Streamlit · MongoDB · Python

## Tech Stack

- Python
- [FastAPI](https://fastapi.tiangolo.com/) for the REST API
- [Streamlit](https://streamlit.io/) for the web UI
- [Groq](https://groq.com/) LLMs for email generation
- [sentence-transformers](https://www.sbert.net/) (`all-MiniLM-L6-v2`) for semantic search
- [MongoDB](https://www.mongodb.com/) via PyMongo for contact storage
- pandas and openpyxl for CSV and Excel import
- SMTP for sending email

## Project Structure

| Path | Purpose |
| :--- | :--- |
| `app.py` | Streamlit web app |
| `main.py` | FastAPI backend: search, generation, sending, templates, history |
| `nlp_engine.py` | Data-type detection and hybrid semantic search |
| `utils/` | Email generation, sending and logging helpers |
| `requirements.txt` | Python dependencies |

## Author

**Amar Chaurasiya**, Data Scientist working as an AI Engineer. Open to full-time roles and freelance work.

- Email: [amarchaurasiya124@gmail.com](mailto:amarchaurasiya124@gmail.com)
- LinkedIn: [linkedin.com/in/amar-chaurasiya-163788262](https://www.linkedin.com/in/amar-chaurasiya-163788262)
- Portfolio: [amarchaurasiya.vercel.app](https://amarchaurasiya.vercel.app)
