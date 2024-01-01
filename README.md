<h1 align="center">Web Scraping and Text Processing Report</h1>

<h3 align="left">Introduction:</h3>
This report outlines the implementation and utilization of Python code for web scraping and text processing tasks. The primary focus is on extracting information from online articles, cleaning text data, and performing various linguistic and sentiment analyses.

<h3 align="left">Web Scraping:</h3>
The web scraping process is facilitated by two main functions. The former function navigates to a given URL using the Selenium library, extracts HTML content, and utilizes BeautifulSoup for parsing. The latter function iterates through a list of URLs stored in an Excel file, employs the extraction function, and saves the obtained text into individual text files. The code is configured to handle errors, such as timeouts and exceptions during scraping.

<h3 align="left">Stopwords Processing:</h3>
Stopwords, common words excluded in natural language processing, are processed using a function. This function reads a list of stopwords from a specified file path, strips any leading or trailing whitespaces, and returns a set of stopwords. To accommodate multiple folders containing stopwords, the code is enhanced to combine stopwords from various folders into a single set, fostering a comprehensive dataset for language processing applications.

<h3 align="left">Text Cleaning:</h3>
Text cleaning is performed through the functions. The former function removes stopwords from article text, while the latter checks and reports the cleaning status of text files within a specified root folder. This ensures the effectiveness of the stopwords removal process.

<h3 align="left">Word Extraction from Word Documents:</h3>
The code extracts positive and negative words from separate Microsoft Word documents using the python-docx library. Positive and negative word sets are created and combined, providing valuable resources for sentiment analysis and text processing tasks.

<h3 align="left">Linguistic and Sentiment Analysis:</h3>
A comprehensive set of linguistic and sentiment features is calculated for articles in subfolders within a root folder. Sentiment scores (positive and negative), polarity, subjectivity, readability scores (average sentence length, percentage of complex words, Fog Index), and additional linguistic features (average words per sentence, syllables per word, personal pronouns count, average word length, complex word count, total word count) are calculated. All features are aggregated into a structured DataFrame named df_scores, offering detailed insights into the linguistic characteristics and sentiment composition of each article.

<h3 align="left">Data Export:</h3>
Finally, the processed data is saved to an Excel file named 'Output Data Structure 2.xlsx'. This file serves as a structured and shareable format for further analysis and visualization of the extracted information.

<h3 align="left">Execution Instructions:</h3>
<h3 align="left">To run the provided Python script:</h3>

Ensure that you have the required dependencies installed, including Selenium, BeautifulSoup, pandas, python-docx, and other relevant libraries.
Modify the file paths in the script according to your system configuration.
Execute the script using a Python interpreter.
The script will perform web scraping, stopwords processing, text cleaning, word extraction, linguistic and sentiment analysis, and save the processed data to an Excel file.

<h3 align="left">Conclusion:</h3>
This Python script provides a comprehensive solution for web scraping, text processing, and linguistic analysis. It can be customized and extended to suit specific requirements in natural language processing tasks, sentiment analysis, and other text-based applications. The structured output facilitates further exploration and insights into the content extracted from online articles.
