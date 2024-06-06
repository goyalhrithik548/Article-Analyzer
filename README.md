# Article Analyzer

## Objective
This project involves extracting textual data from a set of URLs and performing text analysis to compute various linguistic metrics. The URLs are provided in an Excel file (`input.xlsx`), and the extracted data is analyzed to generate outputs in the format specified by the `Output Data Structure.xlsx` file.

## Data Extraction
The goal is to extract the article title and article text from each URL, ignoring headers, footers, and other non-article content. The extracted text for each article is saved in a text file named after the URL_ID.

## Data Analysis
Textual analysis is performed on the extracted article text to compute the following variables:
- POSITIVE SCORE
- NEGATIVE SCORE
- POLARITY SCORE
- SUBJECTIVITY SCORE
- AVG SENTENCE LENGTH
- PERCENTAGE OF COMPLEX WORDS
- FOG INDEX
- AVG NUMBER OF WORDS PER SENTENCE
- COMPLEX WORD COUNT
- WORD COUNT
- SYLLABLE PER WORD
- PERSONAL PRONOUNS
- AVG WORD LENGTH

## Requirements
- Python 3.x
- Libraries: BeautifulSoup, requests, nltk, textstat, openpyxl, pandas

## Output
- The results will be saved in `output.xlsx` in the format specified by `Output Data Structure.xlsx`.

## File Structure
- `input.xlsx`: Contains the URLs for the articles to be analyzed.
- `extract_articles.py`: Script for extracting article text from the given URLs.
- `text_analysis.py`: Script for performing textual analysis on the extracted texts.
- `output.xlsx`: The final output containing the computed variables for each article.

## Variables Explanation
Detailed definitions of the variables computed during text analysis can be found in the `Text Analysis.docx` file.

## Notes
- Ensure proper handling of exceptions for failed URL requests.
- The extraction script uses BeautifulSoup for web scraping. Depending on the structure of the target websites, adjustments may be needed.

## Acknowledgments
This project leverages multiple Python libraries for web scraping and text analysis. Special thanks to the developers of BeautifulSoup, requests, nltk, textstat, openpyxl, and pandas for their contributions to the Python ecosystem.
