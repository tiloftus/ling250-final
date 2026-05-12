# Syntactic Complexity in the State of the Union Address (1900–2026)

This project investigates how the syntactic complexity of the annual State of the Union address has changed over time. The central research question asks: how has the syntactic complexity of presidential language changed over time?

To answer this, the project measures multiple well-established indicators of syntactic complexity across more than 120 years of speeches and analyzes long-term trends using statistical modeling and Principal Component Analysis (PCA).

The core finding is that, across a wide range of syntactic metrics, State of the Union speeches show a consistent historical shift toward structurally simpler sentences.

## Introduction

The State of the Union address, delivered annually as an address from the president to Congress, is one of the most recognizable, standard, and public rituals in American politics. The president reports on the condition of the nation, outlines priorities, and communicates policy to both Congress and the public. While the political content of these speeches has changed dramatically from George Washington’s 1790 address to Donald Trump’s 2026 speech, the genre itself has remained remarkably stable: a formal, recurring address intended to explain complex national issues to a broad audience. State of the Union records serve as a 236-year time capsule, allowing us to analyze political speech over time.

We computationally analyze presidential addresses to discern how political speech has changed over time. Politicians aim to meet people where they are; in other words, they attempt to match the tone and language of public discourse. Assessing how they communicate reveals how people process and engage with politics, and how they receive information through the media landscape.

## Respository Structure

The repository for this project follows a very simple structure. The images folder contains the image files used in the paper. The file final_analysis.ipynb contains all code used for the project. 

## Data

This project combines speeches from two sources:

NLTK State of the Union Corpus (1945-2006 speeches) (https://www.nltk.org/install.html)
American Presidency Project (1900-1944, 2007-2026) (https://www.presidency.ucsb.edu/documents/presidential-documents-archive-guidebook/annual-messages-congress-the-state-the-union#Table%20of%20SOTU)

These were merged into a single dataset covering 1900–2026.
This data is not published as part of this repository. It can be downloaded through the links above. To download the TAPP data, simply access the linked speech for each year and copy the results into a plain text (.txt) file. For the NLTK data, final_analysis.ipynb can be used to download the speeches.
The data contains over 900,000 words across 125 speeches.

## Code

The code for the project is contained in a single file: final_analysis.ipynb. This file downloads the data, performs PCA dimensionality reduction, and creates charts and regression models to answer the research question.
Once the data is properly downloaded, all code cells can easily be run cleanly from top to bottom.

This code:
* Loads the State of the Union speech corpus from NLTK and organizes speeches by year and president
* Uses spaCy to perform part-of-speech tagging and linguistic parsing
* Computes readability metrics for each speech using textstat (e.g., Flesch Reading Ease, grade level)
* Builds a structured pandas DataFrame containing linguistic features and  readability scores
* Visualizes trends over time with matplotlib
* Fits statistical models in statsmodels: an OLS regression model to test trends over time and a mixed-effects models to account for clustering by president
* Outputs tables and figures used in the paper

## License
This research project and the associated code is licensed under the MIT License - see LICENSE for more details.
