## Project Overview
This project detects abbreviation-related bad smells and subjective terms in Software Requirements Specification (SRS) documents.
It implements automated Natural Language Processing (NLP) methods to improve the clarity, consistency, and readability of requirement documents.

## Features
 Detects missing abbreviation definitions (e.g., “CPU” used before defining “Central Processing Unit”).
 
 Identifies inconsistent abbreviation usage (e.g., the same full form having multiple abbreviations).
 
 Flags vague or subjective terms like “user-friendly”, “fast”, “efficient”, and suggests clearer alternatives.
 
 Generates output CSV files containing detailed results and examples.

## Dataset Information
The analysis uses the PURE Dataset — a collection of real-world public Software Requirements Specifications (SRS).
Dataset Reference:
Ferrari, A., Spagnolo, G. O., & Gnesi, S. (2017, September).
PURE: A Dataset of Public Requirements Documents.
In 2017 IEEE 25th International Requirements Engineering Conference (RE) (pp. 502–505). IEEE.
📎 Dataset Link: https://zenodo.org/records/1414117

After downloading, extract the dataset and convert files to text format andplace all .txt SRS files in:
/content/data/txt

## Setup Instructions
## 1. Clone this repository
<pre>  git clone https://github.com/Akula-Jyoshnavi/PURE-SRS-AbbreviationCompleteness-Checker.git </pre>

cd PURE-SRS-AbbreviationCompleteness-Checker
## 2. Install dependencies
<pre> pip install nltk pandas </pre>
## 3. Download NLTK resources
<pre>!pip install nltk --quiet
 
import nltk
 
nltk.download('punkt')
 
nltk.download('punkt_tab') </pre>
## 4. To run missing abbrevation script
1.Place all SRS .txt files (from the PURE dataset) inside:
     /content/data/txt
     
2.Run the Python script:

python abbreviation_inconsistency.ipynb

## 5. To run subjective terms script 
To run subjective terms script first get gemini api key get it from :  https://aistudio.google.com/app/apikey

and then run the each cell of SubjectiveTermsRewriter.ipynb script sequentially.



