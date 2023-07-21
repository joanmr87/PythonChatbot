# PythonChatbot
Chatbot with custom data using Langchain and gpt-3.5-turbo-0301 model

# ChatWithYourData_Bot

Welcome to ChatWithYourData_Bot! This is a simple interactive chatbot that uses conversational AI to answer your questions based on a loaded database of documents. The bot is designed to provide concise answers to your queries using the information available in the database.

## Setup and Environment

To run this chatbot, you need to make sure you have the required dependencies installed. The code uses the `panel`, `param`, `datetime`, `dotenv`, `langchain`, `openai`, and `os` libraries. Before running the code, make sure to set up the necessary environment variables, including the OpenAI API key.

### Loading Environment Variables

The code uses the `dotenv` library to load environment variables from a `.env` file. Make sure you have the required API key for OpenAI and store it in the `.env` file as follows:

```plaintext
OPENAI_API_KEY=your_openai_api_key_here
```

Please replace `your_openai_api_key_here` with your actual OpenAI API key.

## Model and Database

The chatbot uses an OpenAI conversational model called `gpt-3.5-turbo` or `gpt-3.5-turbo-0301`, depending on the current date. The model is set to a temperature of 0, which means it provides deterministic responses.

The chatbot's database is loaded from a PDF file provided during initialization. The loaded documents are split into chunks, and embeddings are created for efficient similarity search.

## User Interaction

### Conversation Tab

In the "Conversation" tab, you can enter your questions or queries in the input field. The chatbot will then process your question and respond with concise answers based on the information available in the loaded database. The chat history will be displayed below the input field, showing your interactions with the bot.

### Database Tab

The "Database" tab provides information about the most recent database query made by the chatbot. The chatbot generates queries to the database to retrieve relevant information based on user questions. The results of the database lookup are displayed below this section.

### Chat History Tab

The "Chat History" tab displays the current chat history. It shows all the exchanges between the user and the chatbot during the current session.

### Configure Tab

In the "Configure" tab, you can load a new database in PDF format by using the "Load DB" button. The button allows you to upload a PDF file, and the chatbot will initialize the database based on the newly uploaded file. The "Clear History" button clears the chat history, allowing you to start a new topic or conversation.

## Disclaimer

Please note that the information provided by the chatbot is based on the loaded database of documents. The accuracy and relevance of the answers are dependent on the data available in the database. The chatbot may not always have access to the latest or most comprehensive information.

For any critical or sensitive queries, always verify the information from reliable and official sources.

