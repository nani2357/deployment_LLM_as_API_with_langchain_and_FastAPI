# Langchain API Server with LLAMA3 and OpenAI Integration

## Overview

This project demonstrates a simple yet powerful implementation of a language processing API using FastAPI, Langchain, LLAMA3, and OpenAI's GPT models. The server is designed to provide endpoints for generating text based on user inputs, specifically focused on writing essays and poems. This setup is ideal for educational tools, creative writing aids, and other applications where automated text generation can be beneficial.

## Features

- **API Server**: Built with FastAPI, the server is robust, fast, and easy to deploy. It serves as the backbone of the application, managing requests and responses.
- **Langchain Integration**: Utilizes the Langchain library to orchestrate language model operations, making it easier to implement complex language tasks.
- **LLAMA3 and OpenAI Models**: Incorporates LLAMA3 and OpenAI's models to handle specific text generation tasks:
  - **Essays**: Uses OpenAI's models to generate essays based on a given topic.
  - **Poems**: Employs LLAMA3 to create simple poems suitable for children, based on a specified topic.
- **Streamlit Frontend**: A simple and interactive frontend created with Streamlit, allowing users to input topics and receive generated text.

## Project Structure

- `app.py`: The main FastAPI application file where the server is defined along with its routes.
- `client.py`: A Streamlit application that acts as the client interface to the FastAPI server, sending requests and displaying responses.
- `.env`: Contains environment variables such as the OpenAI API key.

## Usage

To run the server, navigate to the project directory and execute the following command:

```bash
uvicorn app:app --host localhost --port 8000
```
## For the client side, ensure the server is running and execute:
```bash
streamlit run client.py
```
## Installation
### To set up the project, clone the repository and install the dependencies:
```bash
git clone [<repository-url](https://github.com/nani2357/deployment_LLM_as_API_with_langchain_and_FastAPI.git)>
pip install -r requirements.txt
```

### Ensure to create a .env file with your OpenAI API key:

```bash
OPENAI_API_KEY='your_openai_api_key_here'

```

## API Documentation
Once the server is running, the API documentation is available at http://localhost:8000/docs. This page provides an interactive interface where you can test the API endpoints directly.

