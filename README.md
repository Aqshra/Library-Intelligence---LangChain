# Library-Intelligence---LangChain

**Library Intelligence**: A conversational AI-powered library assistant that helps users with general queries, find books, provides recommendations, and handles book requests via automated emails to library staff. Built with LangChain, LLaMA LLM, Flask and Streamlit for a seamless library experience.

This project is an AI-powered chatbot designed to enhance the library experience. The chatbot helps users find books, provide personalized recommendations, handle book requests via automated emails, and analyze user feedback.

## Features
- **Book Search & Recommendations**: Allows users to search for books and get recommendations based on their queries.
- **Book Request Form**: Automatically sends book requests via email to library administration.
- **Feedback Analysis**: Visualizes user feedback using some basic charts.

## File Structure

- **`APP1.py`**: Main Streamlit file that runs the chatbot interface.
- **`chat_with_docs.py`**: Handles the upload and processing of PDF files for document-based chatbot queries. It uses LangChain for the retrieval chain and question-answering functionality.
- **`flask_app.py`**: Contains the book request form and email-sending feature.
  - **Note**: The email in the code is set as `xxx@gmail.com` and the password is `"passwrod"`. You need to change these to your own credentials before deploying.
- **`visualisation.py`**: Manages feedback analytics and generates basic visualizations.
- **`groq_api_key.py`**: Contains the API key for the required APIs. You have to change it to your own API key.

### Run the three main components

To start all parts of the application, run the following commands in separate terminals:

1. **Start the chatbot interface**:
   ```bash
   streamlit run APP1.py
