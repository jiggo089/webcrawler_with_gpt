# OpenAI Embedding and Question Answering Script

This repository contains a Python script that leverages OpenAI's API to answer questions based on context retrieved from a pre-processed dataset of text embeddings. The script matches user queries with the most relevant information from the dataset and generates responses using a GPT model.

## Features

- **Load Pre-Computed Embeddings**: The script loads text embeddings from a CSV file and processes them for similarity comparison.
- **Contextual Question Answering**: Retrieves the most relevant context based on the query and generates an appropriate response using OpenAI's GPT-3.5-Turbo model.
- **Flexible Distance Metrics**: Supports various distance metrics (cosine, L1, L2, Linf) for embedding similarity comparison.

## Prerequisites

- **Python 3.6+**
- **OpenAI API Key**: Required to access OpenAI's GPT and embedding models.
- **Python Libraries**:
  - `openai`
  - `pandas`
  - `numpy`
  - `scipy`
  - `python-dotenv`

## Setup

### 1. Clone the Repository

Clone this repository to your local machine:

```sh
git clone https://github.com/yourusername/openai_embedding_qa.git
cd openai_embedding_qa
```
### 2. Install Dependencies
Install the necessary Python libraries using pip:

```sh
pip install openai pandas numpy scipy python-dotenv
```
### 3. Set Up OpenAI API Key
Create a .env file in the root directory with the following content:

```plaintext
OPENAI_API_KEY=your_openai_api_key_here
```
