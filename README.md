# NY Times Topic Modelling Approach Note

Firstly, I extracted the news using the New York Times archive api for the month of January,2019. There are about 7,000 headlines along with the URL to the pages of the articles.
Secondly, I used beautiful soup to extract the news articles correponding to each headline and concatenated it with the headlines.After that I did some cleaning like taking only news in english language and created a custom list of stopwords.
Thirdly, I ran a topic model on the cleaned text using the sklearn LDA package and got the top words relating to each topic and also allocated topics on every article.
Finally, I used flask to create an api of the whole code and deployed it on heroku.
In the website the user has to choose the number of topics and a date from 1st to 31st of January,2019 and it displays the top words related to each topic and also 50 news on that given date along with topics.
