# -Semantic-Book-Recommender
An intelligent book recommendation system that understands your descriptions and emotions. Just describe the type of story you're looking for — and get personalized book suggestions based on semantic similarity and emotional tone. Powered by embeddings, natural language processing, and Gradio for an interactive UI.
Project Details
This project consists of several key components and Jupyter notebooks that showcase the data processing, machine learning, and application development steps behind the Semantic Book Recommender:

Text Data Cleaning:
Data preprocessing and cleaning are performed in data-exploration.ipynb. This notebook handles preparing the raw book description data for further analysis.

Semantic (Vector) Search and Vector Database Construction:
The vector-search.ipynb notebook demonstrates how to build a vector database using book descriptions' embeddings. This enables searching for books that are semantically similar to natural language queries, such as "a book about a person seeking revenge."

Text Classification with Zero-Shot Learning:
In text-classification.ipynb, zero-shot classification using large language models is applied to categorize books as fiction or non-fiction. This creates an additional filter facet for users.

Sentiment Analysis and Emotion Extraction:
The sentiment-analysis.ipynb notebook performs sentiment analysis with LLMs to extract emotional tones from book descriptions. This allows sorting and filtering books by emotions such as joy, sadness, suspense, and more.

Interactive Web Application:
The gradio-dashboard.py script creates a user-friendly web interface using Gradio. It lets users input a description and select filters to receive personalized book recommendations.

Requirements
This project was initially developed using Python 3.11. The following dependencies are required and included in the requirements.txt file:

kagglehub

pandas

matplotlib

seaborn

python-dotenv

langchain-community

langchain-opencv

langchain-chroma

transformers

gradio

notebook

ipywidgets


## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/Semantic-Book-Recommender.git
   cd Semantic-Book-Recommender

  2.Create and activate a virtual environment

    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
3.Install dependencies:
   pip install -r requirements.txt


4.Create a .env file in the root directory and add your API keys:

OPENAI_API_KEY=your_openai_api_key_here
HUGGINGFACEHUB_API_TOKEN=your_huggingface_token_here




   

