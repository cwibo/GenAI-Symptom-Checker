# GenAI-Symptom-Checker
This repository showcases the development of GenAI Symptom Checker, a prototype system that leverages Retrieval-Augmented Generation (RAG) and large language models (LLMs) to deliver real-time, AI-powered preliminary medical assessments. Developed as a capstone project, the system addresses critical issues in healthcare such as misdiagnosis, emergency room overcrowding, and limited access to timely triage by enabling patients to input symptom descriptions in natural language and receive medically grounded, context-aware guidance.

# Key Features

    Natural Language Processing Pipeline: Utilizes NLTK and SciSpaCy to extract medical entities from free-text symptom input.
    Semantic Retrieval: Pinecone-based vector search over a synthetic medical knowledge base containing 15,000+ annotated symptom reports.
    LLM-Powered Synthesis: Uses OpenAI’s GPT via LangChain to generate human-readable responses grounded in retrieved documents.
    Urgency Classification: Implements a scikit-learn classifier to assess whether a case is urgent or non-urgent, with 100% recall on emergency scenarios.
    Streamlit UI: Provides an intuitive, conversational interface with consent mechanisms, follow-up prompts, and user feedback logging.

# Tools & Technologies
    Python, Streamlit, SQLite, SciSpaCy, Pinecone, OpenAI API, LangChain, scikit-learn, Pickle

# Evaluation Highlights

    75–80% triage accuracy, 100% emergency recall, 75% diagnostic precision
    Safe, interpretable output for ambiguous or rare conditions
    Modular design supports scaling, auditing, and future multi-modal inputs (e.g., image, voice)
