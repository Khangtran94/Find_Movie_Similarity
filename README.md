# ***Find Movie Similarity from Plot Summaries (Source: IMDb and Wikipedia)***

## Project Objective:
* Quantify the similarity of movies based on their plot summaries available on IMDb and Wikipedia, then separate them into groups, also known as clusters.   
* Create a dendrogram to represent how closely the movies are related to each other.

## Methods Used:
* Data Visualization
* Clustering
* NLP (Tokenize & Stemming)

## Libraries Used:
* Pandas
* Numpy
* Matplotlib
* NLTK
* Regex
* sklearn
* scipy

# Dataset information:
The dataset contains the titles of the top 100 movies on IMDb as well as each movie's plot summary from both IMDb and Wikipedia.

The dataset has **100 rows** and **5 columns**

![Untitled](https://github.com/Khangtran94/Find_Movie_Similarity/assets/146164801/624955b6-247e-4c42-88be-d960a2419760)

## Step by step:
### 1. Combine plot summary from IMDb and Wikipedia
### 2. Tokenine:
* Tokenization: the process we break down articles into individual sentences or words, as needed.
* Perform additional filtration to remove tokens which are entirely numeric values or punctuation.
### 3. Stemming:
* Stemming: The process we bring down a word from its different forms to the root word.
* ==> Establish meaning to different forms of the same words without having to deal with each form separately.
### 4. Create TfidfVectorizer:
* Convert our textual plot summaries to numbers for the computer to be able to extract meaning from them.
* ==> TfidfVectorizer: The Term Frequency of a word is the measure of how often it appears in a document, while the Inverse Document Frequency is the parameter which reduces the importance of a word if it frequently appears in several documents.
* ==> TF-IDF helps us recognize words which are unique and important to any given document.
### 5. Cluster the movies:
* Clustering: the method of grouping together a number of items such that they exhibit similar properties.




