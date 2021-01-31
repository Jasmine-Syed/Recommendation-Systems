# Recommendation-Systems

Recommender system becomes very popular and has important role in an information system or webpages nowadays. A recommender system tries to make a prediction of which item a user may like based on his activity on the system. There are some familiar techniques to build a recommender system, such as content-based filtering and collaborative filtering. 

# 1. Weighted Hybrid Approach in Recommendation Method.

Content-based filtering does not involve opinions from human to make the prediction, while collaborative filtering does, so collaborative filtering can predict more accurately. However, collaborative filtering cannot give prediction to items which have never been rated by any user. In order to cover the drawbacks of each approach with the advantages of other approach, both approaches can be combined with an approach known as hybrid technique. Hybrid technique used in this work is weighted technique in which the prediction score is combination linear of scores gained by techniques that are combined.The purpose of this work is to show how an approach of weighted hybrid technique combining content-based filtering and item-based collaborative filtering can work in a movie recommender system and to show the performance comparison when both approachare combined and when each approach works alone. There are three experiments done in this work, combining both techniques with different parameters. The result shows that the weighted hybrid technique that is done in this work does not really boost the performance up, but it helps to give prediction score for unrated movies that are impossible to be recommended by only using collaborative filtering.


# **Steps to follow:**

1. Import required libraries.

2. Import credits and movies dataset.

3. Rename credits dataframe "movieID" column to "Id" to merge credits dataframe with moves dataframe on "Id" column.

4. Merge Movies and credits dataframe on "id" column.

5. Drop the columns which are not important.

6. Check for NA values.

7. As per the weighted average formula, assign  corresponding variable names to the  required columns.

8. Calculate the weighted average using the formula.

9. Find the top 10 movies for recommendation based on the weighted average by sorting the weighted average values in descending order. Plot a bar graph to see the top 10 movies.

10. Find the top 10 movies for recommendation based on the popularity by sorting the popularity values in descending order. Plot a bar graph to see the top 10 movies.

11. Find the top 10 movies for recommendation based on the popularity and weighted_average. Create a new column which gives equal importance to both popularity and weighted average. Sort the new column values in descending order. Plot a bar graph to see the top 10 movies.
