# Scientific Papers Reads Prediction


## TEAM
- Maryam Omar 
- [Sara Altamimi](https://github.com/saraaltamimi12)

## OVERVIEW
in this project we'll be building a model to predicit the number of reads of scientific articles from different social science departments on researchgate, then we'll build a content-based recommender system that recommends popular articles to users based on the topic they are interested in. 

## STEPS
- Topic modeling: first we'll extract the topics from the papers abstract, using NMF and LDA, then we'll compare the results.
- Calculate number of words and scentences in the titles and abstracts, and add these info as new feauteres.
- Create a regression model to predict the number of reads.
- Create a contend-based recommender system to recommend articles to users based on thier favorite topic.
- Create a website.
- Deploy the website to heruko.


## DATA
The data is scraped form researchgate.net, it will includes information about all publications from  different . we chose social sciences becuase topics in social science do not need domian-experties to understand, and have a solid number of publications and diverse topics. 

### source:
https://www.researchgate.net/

### Description 
the scraped dataset will consist of 1,365 rows and 12 intial columns.

| col | Description | Type |
| --- | --- | --- |
| title | article's title | string 
| auther| auther name | string 
| abstract | abstract's full-text  | string
| category| article, literature review, conference paper..etc | string
| date_published | date the article was puplished | date
| date_added | date the article was uploaded to researchgate | date
| figuers | 1 if there're figures & 0 if not | int
| full_text? | avilability of full text ( using download or Request full-text as keywords) | string
| citation | number of times that paper was cited | int
| reads | number of views (target variable)| int



## TOOLS  

### Data collection, Preprocessing & Modeling  
- **Scraping:** beautifulsoup, selenium. 
- **Text Preprocessing & Mining:** NLTK.
- **Modeling:** scikit-learn.
- **Plotting:** matplotlib, plotly, seaborn.

### Collaboration Tools
- Trello.
- Google Colab.
