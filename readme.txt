*Movie recommendater webapp*
      Demo video of the webapp- 
      https://github.com/kumarUjjawal3621/movie_recommendation/assets/136676393/22a580ad-5fdc-4c8f-9162-bde732d25982

Workflow:
  Data collection  - (Web scraping + API + Kaggle)
      Webscraped the IMDB advanced search page
      Took data from kaggle: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata
      For movie images to show on webpage, I used the TMDB website's API.

  Data wrangling and feature engineering:
      From json like columns, extracted meaningful features
      Final data to be given to for NLP contains only three features: movie id + movie Title + sentiment
          sentiment = keywords + genres + top 3 cast names + director name + short description of movie

  Model building: 
      Used Bag of words and TF-IDF for document embedding.
      For any query, return the top 20 movies with highest value of cosine similarity.

  Deployement:
      Database: 
          Stored the data in mysql server and built a cursor in app.py to fetch the data according to query
      UI:
          Used streamlit to built the UI and local deployement of the webpage
          
      

      
  
      
  
