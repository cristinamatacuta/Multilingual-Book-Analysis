# Multilingual-Book-Analysis

This project conducts a comprehensive analysis of books in three different languages: Spanish, Romanian, and English. It explores linguistic characteristics, visualizes key metrics, and performs sentiment analysis on selected texts. The analysis is implemented using Python and leverages various natural language processing (NLP) libraries.

## Table of Contents
- Installation
- Usage
- Features
- Contributing
- License



## Installation

If you are using this notebook in Google Colab, you don't need to install the libraries separately. Colab provides a pre-configured environment.

However, if you are running this notebook locally, make sure you have the required libraries installed. Open a terminal and run the following command:

```bash
pip install pandas seaborn transformers matplotlib nltk
            
```
## Features
1.read_book(filename)
  Description: Reads the content of a book from a given file.
  Parameters:
            filename: The filename of the book.
  Returns: A string containing the text of the book.

2. vocabulary_richness(text)
   Description: Calculates the vocabulary richness of a given text.
   Parameters:
              text: The text for which vocabulary richness is calculated.
   Returns: An integer representing the vocabulary richness.

3. word_frequency(text, language)
   Description: Counts the 10 most used words in a given text.
   Parameters:
              text: The text to be analyzed.
              language: The language of the text.
   Returns: A DataFrame containing the words and their frequency.
   
5. visualization_bar_chart(top_ten_original, top_ten_translation, figure_name, language)
   Description: Creates a bar chart visualization of the top 10 most used words in the original and translated versions.
   Parameters:
              top_ten_original: DataFrame with top 10 words in the original version.
              top_ten_translation: DataFrame with top 10 words in the translated version.
              figure_name: The name under which the figure will be saved.
               language: The language of the original book.
   
7. emotion_analysis_first_sentence(text, language)
   Description: Performs sentiment/emotion analysis on the first sentence of a given text.
   Parameters:
              text: The text to be analyzed.
              language: The language of the text.
   Returns: Emotion analysis results.
   
9. main()
  Description: The main function that orchestrates the analysis for different language/book pairs.

## Usage

1.Open FinalPython.ipynb in a Jupyter Notebook environment/Google Colab environment.
2.Execute the cells sequentially.
# Feel free to adapt the notebook according to your specific requirements and datasets.

## Acknowledgments

- [DAVENI](https://huggingface.co/daveni/twitter-xlm-roberta-emotion-es): For providing the Spanish Emotion Model.
- [Savani](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion): For the English Emotion Model.
- [Alexandra Ciobanu](https://github.com/Alegzandra): For providing the datasets used in this project.

Note: The Romanian emotion model used in this project was created based on Alexandra Ciobanu's dataset but trained independently.

### Note on Data Files
The notebook assumes the existence of specific data files in the data directory, namely:

english_text.txt: English version of the book.
romanian_english.txt: Romanian translation of the English book.
spanish_text.txt: Original Spanish version of the book.
romanian_spanish.txt: Romanian translation of the Spanish book.
If your data files have different names or are located in a different directory, please modify the file names and paths accordingly in the notebook.

### Contributing
Contributions are welcome! If you find any bugs, have suggestions for improvements, or want to add new features, please open an issue or create a pull request.

### License
This project is licensed under the MIT License - see the LICENSE file for details.
   
