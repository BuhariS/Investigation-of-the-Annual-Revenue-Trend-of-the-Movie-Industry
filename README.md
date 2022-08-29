# Investigation of the Annual Revenue Trend of the Movie Industry

<img src="movie.png" alt="movies pic" style="max-width: 100%;">

## Overview
The movie industry is a billion-dollar industry that generates enormous revenue for stakeholders. However, there are debates that claim that the movie industry is dying. This may discourage prospective investors from investing in the industry.
In this project, I analyze the 55-year record of the movies' metadata in TMDb to uncover trends in the industry's revenue generation. This will guide the decision-making process of prospective investors.

## Dataset Description
The dataset investigated in this project is a collection of features of about 10,000 movies in The Movie Database (TMDb). [1](https://docs.google.com/document/d/e/2PACX-1vTlVmknRRnfy_4eTrjw5hYGaiQim5ctr9naaRd4V9du2B5bxpd8FEH3KtDgp8qVekw7Cj1GLk1IXdZi/pub?embedded=True) TMDb is built by community and for community since 2008 and there are currently more than 400,000 developers using the metadata. [2](https://www.themoviedb.org/about)

## Data Wrangling
The following is the process taken in wrangling the dataset:
- `imdb_id, cast, homepage, director, tagline, keywords, overview, genres, and production_companies have missing values.` However, the missing values were not imputed because they were not our features of interest.
- The outliers will be left intact because they are possible values.
- The features `revenue_adj and vote_average` were renamed to more readable features
- a function that drops rows equal to some certain values was defined for code reusability
- all records with zero revenue , which is our target feature, will be dropped using the function mentioned above.

## Exploratory Data Analysis (EDA)
EDA was carried on the features: `popularity, runtime, vote_count, relaese_year` was carried out with respect to the target variable, `revenue_adj` to explore the relationships between them.