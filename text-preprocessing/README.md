# Text Pre-Processing & Feature Generation 

## Description
`text-pre-processing.ipynb`:

This project focus on the extraction of data from nonstructured format and conversion into a proper format suitable for a downstream modelling task. It consists of a Python code to preprocess a set of published papers and convert them into numerical representations.

The main steps are:

1. Use the given URLs in `paper-ids.pdf` to programmatically download the PDF files.
2. Read the PDF files into text and extract the required entities to complete the above tasks.
3. Text Preprocessing (tokenization, stop words removal, stemming, rare tokens removal, sentence segmentation, bigrams, etc).
4. Statistics Generation.

## Data
There is a data-set containing 200 URLs for papers published in a popular AI
conference. The  pdf file from this link.The pdf file `paper-ids.pdf` contains a table in which each row contains a paper unique id and a URL where it can be downloaded.

## Output
1. Sparse representation for Paper Bodies (i.e. paper text without Title, Authors,
Abstract and References). The sparse representation consists of two files:

   a. Vocabulary index file `vocab.txt`

   b. Sparse count vectors file `count_vectors.txt`
2. CSV file, `stats.csv` containing three columns:

<div align="left">
    <img src="https://i.imgur.com/GhdETul.png" width="400px"</img> 
</div>

    a. Top 10 most frequent terms appearing in all Titles

    b. Top 10 most frequent Authors

    c. Top 10 most frequent terms appearing in all Abstract
