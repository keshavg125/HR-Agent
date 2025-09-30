ChickoHR: An AI-Powered HR Assistant

ChickoHR is a multi-functional, interactive web application built with Streamlit and powered by Google's Gemini family of models. It serves as an all-in-one toolkit for HR professionals, automating and enhancing key tasks like resume screening, new employee onboarding, policy inquiries, and interview simulations.

The application leverages Retrieval-Augmented Generation (RAG) with a hybrid search mechanism (FAISS for semantic search and BM25 for keyword search) to provide accurate, context-aware answers from your company's own documents.

✨ Features

ChickoHR is organized into four distinct modules, each designed to tackle a specific HR challenge:

1. 📝 Policy Query

A conversational AI assistant that can answer questions about company policies.

Hybrid Search: Combines semantic vector search (FAISS) and keyword search (BM25) to find the most relevant document snippets for any query.

Contextual Answers: Uses the retrieved information as context for the Gemini LLM to generate accurate, source-based answers.

Transparency: Displays the source text used to generate the answer, allowing for easy verification and trust in the system.

2. 📄 Resume Scoring

A two-stage automated pipeline for screening and scoring candidate resumes against a job description.

Stage 1: Minimum Qualification Screening:

Automatically extracts structured data from resumes (e.g., CGPA, graduation year, years of experience).

Compares the extracted data against the minimum requirements defined in the job description.

Filters out candidates who do not meet the baseline criteria, saving significant manual review time.

Stage 2: Detailed Scoring:

Scores the qualified resumes on a scale of 100 based on experience, achievements, and overall relevance to the job description.

Ranks the candidates, allowing recruiters to focus on the most promising applicants first.

3. 👋 Onboarding Assistant

A personalized onboarding tool to welcome new employees and get them up to speed.

Automated Account Creation: Generates a mock company email and a temporary password for the new hire.

Personalized Welcome: Creates a warm, welcoming message that includes the new hire's credentials, department, and a summary of key company policies.

Text-to-Speech: Converts the welcome message into audio for a more engaging and accessible experience.

Onboarding Q&A: Allows new hires to ask questions about company policies in a conversational manner, with both text and audio responses.

4. 🎙️ Interview Simulator

An AI-powered agent that conducts a simulated interview based on a provided job description.

Dynamic Question Generation: The Gemini model generates relevant technical questions based on the skills and requirements listed in the JD.

Structured Interview Flow: Covers an introduction, multiple technical questions, and a project deep-dive to provide a comprehensive assessment.

AI-Powered Evaluation: Evaluates the candidate's answers in real-time, providing a score and constructive feedback for each response.

Final Report: Generates a complete transcript of the interview along with a final score breakdown.

🛠️ Tech Stack

Core Framework: Streamlit

AI & LLM: Google Gemini (gemini-2.0-flash)

NLP & Search:

LangChain

FAISS (for vector similarity search)

rank_bm25 (for keyword search)

Hugging Face Sentence Transformers (all-mpnet-base-v2 for text embeddings)

Data Processing: pdfplumber, NumPy

Text-to-Speech: gTTS
