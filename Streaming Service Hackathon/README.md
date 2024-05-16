Presentation and my slides:

Netflix Presentation.pdf, slides 10-15

My Notebooks; their inputs and outputs:

1. netflix_preproc:

   input:
     - netflix_titles.csv - raw dataset that was provided
   
   output:
     - netflix_clean.csv - cleaned data

2. netflix_data_engineering:
  
    input:
      - netflix_clean.csv - cleaned data
      - Netflix Tv Shows and Movies.csv - kaggle dataset of IMDB data
      - title.basics.tsv.gz - publicly available IMDB data
      - title.ratings.tsv.gz - publicly available IMDB data
              
      *Kaggle data available @https://www.kaggle.com/datasets/thedevastator/netflix-imdb-scores*
      *imdb data available @https://developer.imdb.com/non-commercial-datasets/*

    output:
      - netflix_both.csv - netflix_clean with as many imdb scores appended
      - imdb_10k_votes.csv - 10,000 most voted for pieces of media from IMDB
     
3. netflix_analysis

   input:
     - netflix_clean.csv
     - netflix_both.csv
     - imdb_10k_votes.csv
  
   output:
     - imdb_not_netflix.csv - list of movies and tv shows not on Netflix

