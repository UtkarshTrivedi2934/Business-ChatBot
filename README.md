# README for Running the Business ChatBot

- Requirements
Before running the application, ensure you have the following installed:
Python 3.7 or higher
## Required libraries:
streamlit
langchain
PyPDF2
langchain-google-genai
You can install the required libraries using pip:
bash
Copy code
## pip install streamlit langchain PyPDF2 langchain-google-genai

Setup Instructions
Clone the Repository: If applicable, clone the repository containing the app.py file.
bash
Copy code
## git clone repository-url
## cd repository-directory

- Prepare the PDF: Ensure you have a PDF file named Corpus.pdf located in the /content/ directory or adjust the file path in the code to point to your PDF.
- API Key: Replace the placeholder Google API key in app.py with your actual API key:
python
## Copy code
llm = ChatGoogleGenerativeAI(model='gemini-1.5-pro', temperature=0, google_api_key="YOUR_API_KEY")

- Run the Application: Execute the following command in your terminal to start the Streamlit application:
bash
## Copy code
streamlit run app.py


- Access the App: Open your web browser and go to http://localhost:8501 to access the ChatBot.

## Usage Instructions
- Ask a Question: In the input box, type your query related to the wine business.
- Get a Response: The ChatBot will return a quick answer based on the content of the PDF.
