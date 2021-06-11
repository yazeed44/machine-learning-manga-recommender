# machine-learning-manga-recommender
Ann item-item manga recommender. Manga is a type of comic. The recommender relies on a Myanimelist, which is a website that hosts Japanese animation and mangas catalogues. It also includes users’ review and rating for each entry.

I scrapped the data from Myanimelist using BeautifulSoup and cleaned the data of misinputs such as null values, misconfigured encoding. After that I reduced the features to only the ones that are necessary for recommendation like genres, authors, how many people liked it, rating score.

After, we ask the user to input an account’s username in Myanimelist, and the recommender will scrape all the ratings by this user. After that, the ratings are passed to the recommendation engine, which will output 10 mangas and a predicted score for each one of them. The engine calculates the predicted score by relying on the sim
