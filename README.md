# Investigation of the Annual Revenue Trend of the Movie Industry

<img src="movie.png" alt="movies pic" style="max-width: 100%;">

<center>Photo by Moview</center>

## Overview
The movie industry is a thriving billion-dollar sector that consistently generates substantial revenue for its stakeholders. Despite debates suggesting its decline, it is essential to examine the industry objectively. To address any concerns and provide valuable insights to prospective investors, this project delves into a comprehensive analysis of 55 years' worth of movie metadata from TMDb. By meticulously studying this extensive dataset, we aim to uncover trends and patterns that shed light on the industry's revenue generation potential. The outcomes of this analysis will serve as a valuable guide for investors, empowering them to make informed decisions about investing in the movie industry.

## Dataset Description 
The dataset examined in this project comprises a rich collection of features from approximately 10,000 movies sourced from The Movie Database (TMDb) [1](https://docs.google.com/document/d/e/2PACX-1vTlVmknRRnfy_4eTrjw5hYGaiQim5ctr9naaRd4V9du2B5bxpd8FEH3KtDgp8qVekw7Cj1GLk1IXdZi/pub?embedded=True). TMDb, a community-driven platform established in 2008, has been a trusted resource for movie enthusiasts and industry professionals alike. With a dedicated community supporting its growth, TMDb has garnered significant traction over the years, currently boasting a user base of over 400,000 developers leveraging its extensive metadata [2](https://www.themoviedb.org/about). This vast community involvement and usage reflect the reliability and relevance of the dataset, making it an invaluable resource for conducting in-depth analysis and deriving meaningful insights in this project.

## Data Wrangling 
During the dataset wrangling process, the following steps were taken:

1. Handling Missing Values: Several columns, including `imdb_id, cast, homepage, director, tagline, keywords, overview, genres, and production_companies`, contained missing values. However, since these features were not the primary focus of our analysis, the missing values were not imputed. The decision was made to leave them as they were.

2. Treatment of Outliers: Outliers in the dataset were identified, but they were not removed or modified. Instead, they were retained as possible values since they can provide valuable insights and contribute to the overall understanding of the data.

3. Renaming Features: The features `revenue_adj` and `vote_average` were renamed to more descriptive and reader-friendly names, ensuring clarity and ease of interpretation during analysis.

4. Filtering Zero Revenue Records: As the target feature of our analysis was revenue, all records with zero revenue were dropped. By excluding these records, we aimed to focus on meaningful data points and avoid any potential bias that zero-revenue instances might introduce.

By following this systematic approach to data wrangling, we ensured that the dataset was prepared appropriately for subsequent analysis, maintaining data integrity and aligning with the objectives of the project.


## Exploratory Data Analysis (EDA) 
Exploratory Data Analysis (EDA) was conducted on several key features, namely `popularity, runtime, vote_count,` and `release_year`, in relation to the target variable, `revenue_adj`. The purpose of this analysis was to uncover and understand the relationships between these variables. 

To examine the distributions of the features of interest, histograms were employed. These visualizations provided insights into the spread and frequency of values within each feature. By analyzing the shapes of the histograms, we gained an understanding of the data's distribution characteristics.

Additionally, scatter plots were utilized to investigate the relationship between the features of interest and the target variable, revenue. This allowed for a visual exploration of any potential correlations or patterns between these variables. By plotting the data points on a scatter plot, we could assess the strength and direction of the relationship.

Furthermore, a line chart was employed to examine the annual revenue trend within the dataset. This visualization enabled us to observe any notable patterns or fluctuations in revenue over time, providing valuable insights into the overall revenue trajectory of the movies.

By leveraging these various visualizations during the EDA process, we gained a comprehensive understanding of the relationships, distributions, and trends within the dataset. These insights would serve as a foundation for further analysis and decision-making throughout the project.

## Conclusions
The analyses reveal a significant correlation between popularity and annual revenue generation in the movie industry. The moderate positive correlation indicates that movies with higher popularity tend to generate higher revenue. This suggests that audience preferences and engagement play a crucial role in driving revenue.

Furthermore, the line chart depicting the annual revenue trend illustrates the overall growth of the movie industry over time. While there may be occasional dips in revenue, the chart demonstrates a consistent upward trajectory. This indicates that despite temporary declines, the industry has experienced substantial growth, evolving into a lucrative market for investors.

Notably, the data showcases a remarkable increase in revenue from 950 million USD in 1960 to an impressive 24 billion USD in 2015. This significant growth reinforces the notion that the movie industry holds immense potential for generating substantial returns on investment.

Considering the positive correlation between popularity and revenue, coupled with the consistent growth observed in the industry over the years, it becomes evident that investing in the movie industry can be a promising opportunity. The data supports the notion that the movie industry offers a favorable environment for investment, making it an attractive choice for prospective investors seeking potential financial success.

