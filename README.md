# AI_BookRecommender
A content-based book recommendation engine built in Python. The goal is to recommend similar books using natural language processing techniques and present the results in a simple user interface built with Streamlit.

## Project status
Currently in early development. The structure is in place, and the logic is to be implemented.

## Planned Features

- Vectorization of book descriptions
- Cosine similarity for matching similar books
- Streamlit interface for book selection and results display
- Clean, modular codebase with a possibility to expand to use a Neural Network

## Data source
Book metadata is retrieved using the free and open [Open Library API](https://openlibrary.org/developers/api), which provides real-time access to book titles, descriptions, and subjects.

## Tools & Libraries

- Python
- Pandas
- scikit-learn
- spaCy
- Streamlit (UI)

## Project structure

- main.py: Entry point of the app
- data_loader.py: reads the book data, handles data validation, and returns a Data Frame
- text_cleaner.py: cleans and preprocesses book descriptions
- recommender_engine.py: vectorized cleaned text and calculates similarity between books, given a book title it returns the top N most similar books
- streamlit_ui.py: displays dropdowns, results tables, and user inputs
- result_writer.py: saves recommendation results to csv, may also handle logging or report generation in the future.

There is a models_package which is a placeholder for future machine learning models. In the future this may include Neural Networks and deep learning-based recommenders.
