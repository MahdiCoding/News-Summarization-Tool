# News Summarization Application

## Overview
This application retrieves news articles from NewsAPI, generates vector embeddings for semantic search, and provides personalized summaries based on user preferences. It supports both brief and detailed summaries.

## Features
- Fetch news articles from NewsAPI
- Store and retrieve article embeddings using ChromaDB
- Summarize articles using LangChain
- Track user preferences and search history
- Command-line interface for user interaction

## Setup Instructions

### Prerequisites
Ensure you have Python 3.8+ installed on your system.

### Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/MahdiCoding/News-Summarization-Tool.git
   cd News-Summarization-Tool
   ```

2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

4. Set up API keys:
   - Sign up for a free NewsAPI key at [NewsAPI](https://newsapi.org/register)
   - Open `news_retriever.py` and replace `your_newsapi_key_here` with your actual API key.

## Usage
Run the application:
```sh
python main.py
```

### Available Actions
1. **Fetch & Summarize News** – Retrieves articles based on user preferences and provides a summary.
2. **Update Preferences** – Modify topics of interest.
3. **View Search History** – See past searched topics.
4. **Search News on a Custom Topic** – Fetch and summarize articles based on a user-specified topic.

## Example Run
```
User preferences: ['technology', 'AI']
Choose action: [1] Fetch & Summarize News, [2] Update Preferences, [3] View Search History, [4] Search News on a Custom Topic: 1
Choose summary type: [brief/detailed]: brief

News Summary:
OpenAI releases a new AI model improving efficiency in generative tasks. Google announces an AI breakthrough in NLP research.
```


