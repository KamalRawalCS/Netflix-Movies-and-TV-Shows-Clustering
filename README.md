# Netflix-Movies-and-TV-Shows-Clustering

**PROBLEM STATEMENT**

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service's number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

![6](https://github.com/KamalRawalCS/Netflix-Movies-and-TV-Shows-Clustering/assets/138231554/33eb407b-ee0f-4a4d-8639-172daed8cbfe)


**Approaches:-**

Step 1 - We began by loading the required libraries, mounting the drive, and saving the data in variables in order to derive useful insights. Viewing and cleaning the data was our primary goal. The next phase was data analysis and visualisation, where we analysed the distribution of our data using univariate, bivariate, and multivariate plots. A check for multicollinearity was done.


![2 0](https://github.com/KamalRawalCS/Netflix-Movies-and-TV-Shows-Clustering/assets/138231554/c7039201-cf41-46b6-8780-b8ba3ec99730)


![3](https://github.com/KamalRawalCS/Netflix-Movies-and-TV-Shows-Clustering/assets/138231554/801d316f-1e6e-4c12-940e-e2919f82a8e3)


![4](https://github.com/KamalRawalCS/Netflix-Movies-and-TV-Shows-Clustering/assets/138231554/1056a39a-a9e8-4fca-b682-88329ee2d064)


![5](https://github.com/KamalRawalCS/Netflix-Movies-and-TV-Shows-Clustering/assets/138231554/e5df9e18-df03-46af-937a-174855947df0)



**Step 2 -** We performed 3 hypothesis testing one comparing means for two variavles using T-test , second was asssociation of target age and country using chi_square test, last was asssociation of target age and duration using chi_square test.

**Step 3 -** Presence of null values would have created possible errors in the further steps, so we replaced few values with null, few with the word "unknown" few were dropped.

**Step 4 -** As a part of feature engineering we have done textual data processing which includes:expand contraction, lower casing, removing punctuations and stopwords, normalization,and vectoriztion. We performed data scaling using standardscalar, and dimensionality reduction using PCA.

**Step 5 -** Last step was to perform clustering using different algorithms, we tried K-Means, ElbowCurve, DBSCAN, Dendogram, Agglomerative Clustering. Recommendation system function was also developed.

# Conclusion of EDA:

1. Netflix have ~70% of movies and 30% of TV_shows in 2019.
3. Comedy is most popular genre in Netflix, across all content.
4. Netflix focuses to add new content majorly towards end of current year and start of new year.
5. A sudden drop was obserbed after 2020 in count of new content, Which is because of covid pandemic.
6. India is on 2nd place as compared to content availability, maximum content is available for United states.
7. There are almost ~30% of netflix original movies and ~50 % TV-shows.
9. Content category and countries:

   •	Maximum adult content is from Spain.

   •	Maximum teen content is from India.

   •	Maximum older kids content is from Japan.

    •	Maximum kids content is from Canada.
9. All of this insights will be neccesary for business development and SWOT analysis.

# Conclusion for clustering.
1. We tried 5 models for ML i.e.

   •	K-means clustering

   •	Elbow curve

   •	DBSCAN

   •	Hierarchical clustering

   •	Agglomerative clustering
3. K-means clustering shows that '4' will be optimum no of clusters with the silhoutte score of 0.45. But we selected Optimum cluster number as 6 after Elbow curve cross validation.
4. Thus K-means clustering will be best for this data set.
5. Cosine based recommender system was working really well.
