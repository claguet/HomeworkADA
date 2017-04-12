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

## Homework 05 - Taming Text
