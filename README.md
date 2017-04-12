# HomeworkADA
Homework assignments for the Applied Data Analysis course taught by Catasta Michele (http://ada.epfl.ch)

## Homework 01 - Pandas and Data Wrangling
This homework tests the skills in using the Pandas library for a few basic Data Transformation and Data Wrangling tasks.

## Homework 02 - Data from the Web
Extract interesting information from [IS-Academia](http://is-academia.epfl.ch/page-6228.html), the educational portal of EPFL. Specifically, focus on the part that allows [public access to academic data](http://is-academia.epfl.ch/publicaccess-Bachelor-Master).
The list of registered students by section and semester is not offered as a downloadable dataset, so you will have to find a way to scrape the information. 

To download all the tables, it is first required to understand what parameters the server accepts, and
generate accordingly the HTTP requests. For this task, [Postman](https://www.getpostman.com) with the [Interceptor extension](https://www.getpostman.com/docs/capture) can help.

1. How many months it took each Informatic Bachelor students to go from the first to the sixth semester. Is the difference between male and female students in average statistically significant?

2. How much time an Informatic Master student spent at EPFL? And compute the "average stay" per specialization.

3. *BONUS*: perform the gender-based study as in 1. on Informatic Master students.

## Homework 03 - Interactive Viz
Work with the P3 database of the [SNSF](http://www.snf.ch/en/Pages/default.aspx) (Swiss National Science Foundation).
The P3 database is formed by entries which assign a grant (and its approved amount) to a University name.

1. Build a [Choropleth map](https://en.wikipedia.org/wiki/Choropleth_map) which shows intuitively (i.e., use colors wisely) how much grant money goes to each Swiss canton. Find a way to go from University to Canton name. The [Geonames Full Text Search API in JSON](http://www.geonames.org/export/web-services.html) can help.

2. *BONUS*: using the map built, and the geographical information contained in it, give a *rough estimate* of the difference in research funding between the areas divided by the [Röstigraben](https://en.wikipedia.org/wiki/R%C3%B6stigraben)?

## Homework 04 - Applied ML
Gain experience on Applied Machine Learning, exploring an interesting dataset about soccer players and referees.

1. Train a `sklearn.ensemble.RandomForestClassifier` that given a soccer player description outputs his skin color. Show how different parameters passed to the Classifier affect the overfitting issue. Perform cross-validation to mitigate the overfitting of your model and inspect the `feature_importances_` attribute.
*BONUS*: plot the learning curves against at least 2 different sets of parameters passed to your Random Forest. 

2. ggregate the referee information grouping by soccer player, and use an unsupervised learning technique to cluster the soccer players in 2 disjoint clusters. Remove features iteratively, and at each step perform again the clustering and compute the silhouette score.

## Homework 05 - Taming Text
explore a relatively large corpus of emails released in public during the [Hillary Clinton email controversy](https://en.wikipedia.org/wiki/Hillary_Clinton_email_controversy).

1. Generate a word cloud based on the raw corpus. With the help of `nltk`, implement a standard text pre-processing pipeline (e.g., tokenization, stopword removal, stemming, etc.) and generate a new word cloud.

2. Find all the mentions of world countries in the whole corpus, using the `pycountry` utility. Perform sentiment analysis on every email message. Aggregate the polarity information of all the emails by country, and plot a histogram that summarizes the perception of the different countries. 

3. Using the `models.ldamodel` module from the [gensim library](https://radimrehurek.com/gensim/index.html), run topic modeling over the corpus.

4. *BONUS*: build the communication graph (unweighted and undirected) among the different email senders and recipients using the `NetworkX` library.
