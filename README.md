# Conversational Agent with Text-to-Speech (TTS), Speech-to-Text (STT), and Emotion Detection

## Overview
This project implements an advanced conversational agent with the following features:

- **Document-based query answering** using FAISS and Sentence-BERT embeddings.
- **Text-to-Speech (TTS)** for generating spoken responses.
- **Speech-to-Text (STT)** for recognizing user queries via voice.
- **Emotion detection** to analyze the tone of the bot’s response.

## Steps to Run the Project

### Step 1: Create a Conda Environment (Optional but Recommended)

If you're using Conda, it is recommended to create a new environment for the project. This helps to isolate dependencies for this project:

```bash
conda create --name conversational_agent python=3.8
conda activate conversational_agent
```

### Step 2: Install Dependencies

Clone the project repository or navigate to the directory containing the project files. Then, install the required libraries using the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

This will install all the necessary libraries listed in the `requirements.txt` file, including the ones needed for NLP, speech processing, and web interaction.

### Step 3: Run the Streamlit Application

Once the dependencies are installed, you can run the application using Streamlit by executing the following command in the terminal:

```bash
streamlit run app.py
```

This will launch the web interface in your default browser, where you can interact with the conversational agent.

## Tools, Frameworks, and APIs Used

This project uses a combination of tools, libraries, and APIs to enable the various functionalities. Below are the main components:

- **Streamlit**: For building the web interface and interaction flow.
- **FAISS**: For fast similarity search and efficient document retrieval based on vector embeddings.
- **Sentence-BERT**: For generating sentence embeddings used to represent documents and queries.
- **Hugging Face Transformers**: For emotion detection using the DistilRoBERTa model.
- **Google Text-to-Speech (gTTS)**: For converting the chatbot’s text responses into speech.
- **SpeechRecognition**: For converting voice inputs into text queries.
- **NumPy**: For numerical operations on embeddings.
- **SciPy**: For distance calculations in FAISS.
- **PyTorch**: Required for some models used in transformers.

## Challenges Faced and How They Were Addressed

### Challenge 1: Synchronizing Speech-to-Text (STT) and Text-to-Speech (TTS) components effectively.
**Solution**: Integrated the gTTS library for speech generation and SpeechRecognition for accurate voice input. Ensured seamless communication between these components by using Streamlit for real-time updates.

### Challenge 2: Handling large document collections efficiently in FAISS for similarity search.
**Solution**: Optimized document indexing with FAISS to support fast, real-time queries. Added features like vector embedding caching to reduce redundant calculations and improve system performance.

## Future Improvements

### Improvement 1: Implementing a more sophisticated emotion detection model that can recognize a broader range of emotions.
**Recommendation**: Use advanced sentiment analysis or multimodal emotion detection models to capture deeper nuances in both text and speech.





https://github.com/user-attachments/assets/1b519ac4-f06c-4975-b824-35a847d2b61a


