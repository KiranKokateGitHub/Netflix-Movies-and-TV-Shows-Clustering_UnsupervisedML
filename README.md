# UnsupervisedML2
Project Name - Netflix Movies and TV Shows Clustering
Contribution - Individual
Name - Kiran


Problem Statement
Write Problem Statement Here.

The objective of this undertaking is to examine the collection of movies and TV shows on Netflix, sourced from the third-party search engine Flixable, and categorize them into meaningful clusters. This effort aims to improve user satisfaction and reduce subscriber attrition for Netflix, the leading online streaming service provider globally, with a subscriber base exceeding 220 million as of the second quarter of 2022. By delving into the dataset, encompassing content available up to 2019, we intend to reveal fresh perspectives and patterns in the swiftly expanding domain of streaming entertainment.

The dataset encompasses TV shows and movies accessible on Netflix up until 2019, sourced from the third-party Netflix search engine, Flixable. In 2018, an intriguing report from Flixable highlighted a remarkable trend: the count of TV shows on Netflix had nearly tripled since 2010. During the same period, the collection of movies had diminished by over 2,000 titles, while TV show availability had experienced a nearly threefold increase. Exploring this dataset promises to reveal a wealth of additional insights awaiting discovery.

Furthermore, the potential for enriching this dataset by integrating it with external data sources like IMDB ratings

Project Summary -
The objective of the Netflix Movies and TV Shows Clustering project is to categorize similar content available on Netflix into distinct clusters based on their attributes. The project starts with data sourced from a third-party Netflix search engine, encompassing details about over 7,000 movies and TV shows offered on the platform.

This dataset comprises information about movies and TV shows on Netflix. The analysis involves computing descriptive statistics for each variable and utilizing visualizations like scatterplots, distplots, count plots, bar plots, pair plots, heatmaps, pie plots, and box plots to explore relationships between variables.

The dataset consists of 12 columns and 7787 rows, with no duplicate values. Some attributes like director, cast, country, date added, and rating have null values. Most attributes are categorical, except for the numerical release year feature. Despite the date_added feature's incorrect data type, it still contains dates.

Null values constitute 30.68% for director, 9.22% for cast, 6.51% for country, 0.13% for date_added, and 0.09% for rating. To handle this, we replaced null values with placeholders, like "Unavailable," for director, cast, and country. Null values in date_added and rating were removed due to their low occurrence.

Outliers in the release year variable were addressed using the interquartile range. Date_added was converted to datetime and further transformed into year, month, and day features. The feature "listed in" was renamed "genres." The release year's data type was changed from float64 to int64.

After performing univariate, bivariate, and multivariate analyses, key insights were derived:

Netflix offers more movies (69.14%) than TV shows (30.86%). Most Netflix movies were released between 2015 and 2020, while TV shows peaked between 2018 and 2020. Highest numbers of movie and TV show releases occurred in 2017 and 2020, respectively. From 2006 to 2019, Netflix consistently introduced more new movies than TV shows. However, in 2020, the trend reversed, reflecting a shift toward TV content. 2020 and 2021 saw the highest TV show releases in Netflix's history. TV-MA is the predominant content rating, followed by TV-14. Content addition was significant in October and January, but consistent throughout the year. The majority of movies are from the United States, while India ranks second. The United States and the United Kingdom are the primary producers of Netflix TV shows. Raul Campos and Jan Suter directed most movies, while Alastair Fothergill directed most TV shows. Popular international movies and dramas are available on Netflix. Common actors in Netflix content include Lee, Michel, David, Jhon, and James. A slight correlation exists between movie/TV show release year and day added. Based on release_year and year_added plots, Netflix increasingly adds and releases content over time. Content is consistently added throughout the year, based on release_year and month_added. Text data in the description variable underwent processing, including removal of punctuation, stopwords, emails, html tags, urls, special characters, and digits. Lemmatization was performed, followed by vectorization using TFIDF, creating an input matrix for the model. Various clustering algorithms like KMeans, Hierarchical, and DBSCAN were trained.

The K-Means Clustering model exhibits the highest Silhouette Score (0.039880), suggesting relatively better clustering compared to Hierarchical and DBSCAN models with negative scores. However, none of the models perform exceptionally well, indicating challenges in separating clusters. The Calinski-Harabasz and Davies-Bouldin Scores are relatively consistent across models.


