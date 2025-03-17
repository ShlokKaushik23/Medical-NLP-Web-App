# LIVE LINK: https://tips-louis-lawn-card.trycloudflare.com/
# Code Link: https://colab.research.google.com/drive/1bbrMyBQusXFzy8lozRgANfcAJIBQUAFi?usp=sharing

# Medical-NLP-Web-App
This project focuses on developing an AI-based system that converts medical transcripts into structured SOAP (Subjective, Objective, Assessment, Plan) notes. By leveraging Natural Language Processing (NLP) techniques, the model extracts key medical details such as symptoms, diagnoses, treatments, and prognoses from physician-patient conversations.


--> Instructions on Setting Up and Running the Application
1. Install Dependencies
Ensure you have Python installed, then install the required libraries:

bash
Copy
Edit
pip install streamlit transformers spacy torch
python -m spacy download en_core_web_sm
2. Run the Streamlit Application
Execute the following command in the terminal:

bash
Copy
Edit
streamlit run app.py
3. Access the Application
Once the server starts, you’ll see a local URL (e.g., http://localhost:8501/). Open this in your browser to interact with the app.

--> Methodologies Used
1. Named Entity Recognition (NER) for Medical Information Extraction
Algorithm: SpaCy's en_core_web_sm model is used for NER.
Reasoning: Detects key medical entities (symptoms, diagnosis, treatment) efficiently.
2. Sentiment & Intent Analysis
Algorithm: Transformer-based model (distilbert-base-uncased-finetuned-sst-2-english).
Reasoning: Classifies patient sentiment as Anxious, Neutral, or Reassured and detects intent (e.g., Seeking reassurance).
3. SOAP Note Generation
Algorithm: Rule-based mapping of extracted medical details.
Reasoning: Ensures structured clinical documentation based on standard SOAP formatting.
<img width="956" alt="NLPWEb" src="https://github.com/user-attachments/assets/57e5f494-93e3-4638-9b03-bb4af1b575a8" />
<img width="959" alt="NlpWeb2" src="https://github.com/user-attachments/assets/06c5621c-d880-4886-90ba-95e8aba3ed37" />
<img width="956" alt="NLPweb3" src="https://github.com/user-attachments/assets/f5d3a6e9-c1f2-45fa-baf8-8f3808d3d2d8" />
