FE595-Final Project (Restaurant NLP Service)
About:
This project is to create an NLP web service for 50 restaurants on Hoboken. There are 7 returned services per input, they are sentimental analysis, translation service, 10 most common adj words, 10 most common noun words, top 10 positive words and top 10 negative words, and SKlearn.

Usage
We have connectted the whole project on our AWS and keep Flask app alive.

Just copy port address (http://18.216.18.200:5001/yelpsearch) into browser.

Follow the instructions, select interested restaurant name, click submit

Now you get all services you want.

Contribution
Sijie Wen:

Draft a demo of this project

Program a function to collect restaurants’ names and business ids using Yelp business fusion API, test use the Yelp Review Search API, prepare for the following steps of building our database

Program the whole function of Flask app, adjust and arrange every member's services into this app as correct format

Write and beautify design corresponding HTML files with instructions

Create NLP service – translate the reviews of a restaurant into Chinese

Create NLP service – overall rating based on the sentiment score for a restaurant

Test and debug programs and web services

Xiaolu Li:

Propose the idea and flow of the project

Program a function to collect 5 areas restaurants’ names and business ids using Yelp business fusion API. This is the database for this project

Program a function to get input restaurant name from user, if there is a match with our database. The function will script the first page of reviews on Yelp (we didn’t use the Yelp Review Search API, because it only returns 3 reviews)

Create NLP service – most commonly used adjective words for a restaurant

Create NLP service – most commonly used noun words for a restaurant

Test and debug programs

Yamin Tang:

Create NLP service – top 10 positive noun phrases used for a restaurant

Create NLP service – top 10 negative noun phrases used for a restaurant

Update for Final Project
For final, we extent futher on HTML web design and Machine Learning based on our midterm project,
We created a dropdown for all available restaurants, users can select from the droplist for services

We centralized all the services on one retrun instead of seperate pages from the midterm

We used sentimental score(x) and yelp rating(y) fit a regression model, use this model to generate normalized rating from our service

We redesigned the webpage, it looks nicer and neat

Future Work
Increase the amount of restaurants in our database (current 50), so to increase the training data on our regression model. Due to the size limit of EC2 and loading speed for the service, we use 50 for now.
