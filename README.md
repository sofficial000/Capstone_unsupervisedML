# Capstone_unsupervisedML

This is an Unsupervised ML Project where we use clustering algorithms to make predictions on the target variable.

# Project Summary

The entertainment industry is highly competitive, and achieving success depends on various factors such as genre, rating, production budget, cast, and more. To understand what influences the popularity of movies and TV shows on Netflix, a study was conducted. This study utilized a dataset with about 12 variables to categorize movies and TV shows based on their popularity and audience preferences.

A) The first step of the analysis involved data wrangling, where missing values were addressed, and unique values were examined. The study found that there were 2389 missing values for the 'director' column, 718 for the 'cast' column, 507 for the 'country' column, and 10 for the 'date_added' column. To handle this, the missing values were removed by dropping the corresponding rows from the dataset.

B) In the exploratory data analysis (EDA) phase of the study, it was observed that the number of movies available on Netflix exceeds the number of TV shows, with 5372 movies and 2398 TV shows currently offered on the platform. TV-MA is the most common rating for TV shows, indicating a significant portion of adult-oriented content in Netflix's TV show collection. Interestingly, TV-MA is also the most prevalent rating for movies, suggesting that Netflix's content is primarily tailored to adult audiences, focusing on mature and potentially controversial themes.

C) The years 2017 and 2018 witnessed the highest number of movie releases on Netflix, while 2020 had the highest number of TV show releases. Notably, the growth rate of movie releases is considerably higher than that of TV shows, indicating a stronger emphasis on expanding the movie content on Netflix. Since 2015, there has been a substantial overall increase in the number of movies and TV show episodes available on the platform. However, after 2020, there was a noticeable decline in the production of both movies and TV show episodes, suggesting a potential shift in Netflix's content creation strategy.

D) Based on the count plot analysis, it is evident that Netflix tends to add the most movies and TV shows during the period spanning October to January. This timeframe appears to be the busiest season for Netflix, as it adds a significant amount of new content to its platform during these months. The United States is the country with the largest content library on Netflix, closely followed by India. Furthermore, India holds the distinction of having the highest number of movies available on Netflix among all the countries analyzed.

E) To cluster the shows, the study focused on six key attributes: director, cast, country, genre, rating, and description. These attributes were transformed into a 10,000-feature TFIDF vectorization, and Principal Component Analysis (PCA) was applied to reduce the components to 3000, capturing over 80% of the variance.

F) Next, two clustering algorithms, namely K-Means and Agglomerative clustering, were utilized to group the shows. K-Means analysis determined that the optimal number of clusters was 5, whereas Agglomerative clustering suggested 7 clusters. The resulting clusters were then visualized using a dendrogram, offering insights into the relationships between the grouped shows.

G) Lastly, a content-based recommender system was developed, utilizing a similarity matrix derived from cosine similarity. This system offers personalized recommendations to users based on the type of show they have previously watched. It presents them with a curated list of 10 top-notch suggestions to explore further.

In conclusion, the study uncovered significant trends within the Netflix dataset, such as the contrasting growth rates between movies and TV shows, the busiest content addition period, and the content demographics. By employing clustering and a content-based recommender system, the study successfully delivered personalized recommendations based on the user's viewing history. These findings offer valuable insights into the factors that drive the popularity of movies and TV shows on Netflix, providing a solid basis for future research and analysis in this domain.

# Problem Statement
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, and rotten tomatoes can also provide many interesting findings

In this project, you are required to do-

A) Exploratory Data Analysis.

B) Understanding what type content is available in different countries.

C) If Netflix has been increasingly focusing on TV rather than movies in recent years.

D) Clustering similar content by matching text-based features.

# Main Libraries Used
1. Pandas for data manipulation and agrregation.

2. Matplotlib and Seaborn for visualization and behavior with respect to the target variable.

3. Numpy for computationally efficient operations.

4. Scikit Learn for model training, model optimization and metrics calculation.
