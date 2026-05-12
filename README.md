# Syntactic Complexity in the State of the Union Address (1900–2026)

This project investigates how the syntactic complexity of the annual State of the Union address has changed over time. The central research question asks: how has the syntactic complexity of presidential language changed over time?

To answer this, the project measures multiple well-established indicators of syntactic complexity across more than 120 years of speeches and analyzes long-term trends using statistical modeling and Principal Component Analysis (PCA).

The core finding is that, across a wide range of syntactic metrics, State of the Union speeches show a consistent historical shift toward structurally simpler sentences.

## Data

This project combines speeches from two sources:

NLTK State of the Union Corpus (1945-2006 speeches) (https://www.nltk.org/install.html)
American Presidency Project (1900-1944, 2007-2026) (https://www.presidency.ucsb.edu/documents/presidential-documents-archive-guidebook/annual-messages-congress-the-state-the-union#Table%20of%20SOTU)

These were merged into a single dataset covering 1900–2026.
This data is not published as part of this repository. It can be downloaded through the links above.

## Code

The code for the project is contained in a single file: final_analysis.ipynb. This file downloads the data, performs PCA dimensionality reduction, and creates charts and regression models to answer the research question.
Once the data is properly downloaded, all code cells can easily be run cleanly from top to bottom.
