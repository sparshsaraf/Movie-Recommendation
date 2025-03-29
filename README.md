# Movie Recommendation System

This repository contains a simple movie recommendation system built using Python. It leverages natural language processing (NLP) concepts to recommend movies based on user input. The project utilizes essential libraries like **NumPy**, **Pandas**, **Matplotlib**, and **NLTK**.

## Dataset
The dataset used contains movie details, including columns like:
- `budget`
- `genres`
- `homepage`
- `id`
- `keywords`
- `original_language`
- `original_title`
- `overview`
- `popularity`
- `production_companies`

## Project Workflow
### 1. Data Preprocessing
- Imported the dataset using **Pandas** from a CSV file.
- Dropped **null values** and **duplicate values**.
- Selected only the necessary columns required for model training.
- Converted dictionary data (like `ids` and `names`) to extract the relevant names only.

### 2. Natural Language Processing (NLP)
- Used **NLTK** for text preprocessing, including:
  - **Tokenization**: Breaking down sentences into words.
  - **Stemming**: Reducing words to their root form.

### 3. Vectorization
- Applied vectorization to convert text into binary code using **CountVectorizer**.

### 4. Similarity Calculation
- Used **Cosine Similarity** to measure the similarity between movie overviews and user input.

### 5. Recommendation Function
- Implemented a function that takes a movie name or keyword as input and returns movie recommendations based on similarity.

## Installation
Make sure you have Python and the following libraries installed:
```bash
pip install numpy pandas matplotlib nltk scikit-learn
```


## Example
```plaintext
Input: Interstellar
Output:
1. Gravity
2. The Martian
3. Inception
```

## Future Improvements
- Implementing additional models for better accuracy.
- Adding user rating-based recommendations.
- Enhancing the UI for a better user experience.



