# Shakespeare Search Engine

## Overview
This Python script implements a search engine for all of Shakespeare's 44 books. It allows users to input queries and retrieves relevant files from Shakespeare's works based on the words in the query, supporting logical operators like 'and' and 'or'. It also provides a mechanism to handle misspelled words by finding the closest match using Levenshtein distance.

## Prerequisites
- Python 3.x
- NLTK (Natural Language Toolkit)

## Installation
1. Clone this repository:
    ```
    git clone https://github.com/Yasu1s/shakespeare-search-engine.git
    ```
2. Navigate to the project directory:
    ```
    cd shakespeare-search-engine
    ```
3. Install NLTK:
    ```
    pip install nltk
    ```
4. Download NLTK resources:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    nltk.download('wordnet')
    ```

## Usage
1. Ensure you have the Shakespeare text files in a directory named 'BOOKS' within the project directory.
2. Run the script:
    ```
    python search_engine.py
    ```
3. Enter your query when prompted.
4. The script will display the matching files from Shakespeare's works based on your query.

## How it Works
1. **Preprocessing**: The script tokenizes, removes stopwords, lemmatizes, and stems the words in Shakespeare's texts to prepare them for indexing.
2. **Indexing**: It builds a mapping from each word to the files in which it appears.
3. **Query Processing**: It processes user queries, supporting logical operators 'and' and 'or' to retrieve relevant files.
4. **Closest Word Handling**: If a word in the query is not found in the index, it finds the closest match using Levenshtein distance to provide relevant results.

## Limitations
- The search engine may not handle complex queries effectively.
- Performance may vary based on the size of Shakespeare's texts and the hardware resources available.

## License
This project is licensed under the [MIT License](LICENSE).

---

Feel free to customize this README to better fit your project structure and details.
