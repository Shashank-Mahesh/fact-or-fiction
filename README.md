# Fact-or-Fiction

**Shashank Mahesh**\
**Sahil Gupta**\
**Pranav Atreya**

## What it does
Our app Fact or Fiction allows a user to paste the URL of an article they wish to read the news from, and classifies the article's credibility. It makes use of multiple factors to give the user this final credibility rating, such as biases of the publisher, recency of the article, and fact checking with other news sources. The users get an explanation to which factors led to the credibility of the article, and can visually compare these different factors with a graph of the results.

## How we built it
In order to build the app's fact checking, article bias, and timestamp capabilities, we wrote networking and HTML file parsing algorithms in a Java Android platform. We made API calls to a library known as JSoup that allowed us to extract text from HTML files. Finally with these algorithms in place, we built a rule based AI that gave weights to each of these individual factors and outputted an overall article credibility score for the user. We built an elegant UI using Android that would allow the data to be displayed along with a pie chart of the data.

## Challenges we ran into
We attempted to use an online database of article publishers using firebase, but we ran into difficulties accessing the data from the database. We thus reverted to using a local database. In the future we plan on implementing a database into one of our own web servers, and allowing the app to access the database through this.

## Inspiration
Over the past few months, the epidemic of "fake news" has spread across the nation, with countless people believing falsified information. False news websites are often built in fashions that seem as if they give credible and correct information, and it is very easy to believe these website articles. Furthermore even news publishers that usually give credible information may one day spout false facts. Realizing that this issue currently has no solution, we decided that a software with capabilities to classify news articles has the potential to be very useful for the general public.

## What's next for Fact or Fiction?
Our future plans for this app include transporting the publisher database onto a cloud location such that it can be constantly updated and scaled. We plan on adding a feature into our UI such that users can themselves give ratings on credibilities of news sources.

## Accomplishments that we are proud of
Algorithms for predicting the credibility of a source have not been written before, and it has been always up to the user to judge the article's credibility. Our app implements this technology into an easy to use app, making it extremely convenient for users to check the credibility as they read news on their phone. Finally we are proud of how we were able to build this app with its multiple algorithms in under 20 hours.
