
# Movie Recommendation System

A content-based and collaborative filtering recommendation system has been created in this notebook, followed by a combination of these models to create our ultimate recommendation system. 

## Content-Based Filtering

This method models user preferences only based on the qualities and description of the items that users have previously consumed.  The user's prior ratings of various potential goods are specifically compared, and the best-matching things are then recommended.

The content based recommenders was based on Movie Overviews and Taglines.  Cosine Similarity was used to calculate a numeric quantity that denotes the similarity between two movies.

The top 25 films based on similarity scores were selected, and the vote for the film with the 60th percentile rating was computed in order to return films that are well-liked by audiences and have received positive reviews. The weighted rating for each film was then determined using the IMDB algorithm, using this as the value of m.

Weighted Rating (WR) =  ((v/v+m).R)+((m/v+m).C)
 
where,
v is the number of votes for the movie
m is the minimum votes required to be listed in the chart
R is the average rating of the movie
C is the mean vote across the whole report

# Collaborative Filtering
By gathering preferences or taste information from numerous users, collaborative filtering creates automatic filtering regarding a user's interests. The collaborative filtering approach's fundamental premise is that if two people A and B share the same opinions on a group of things, then A is more likely to share B's view for a particular item than the opinion of a randomly selected individual.

The RMSE (Root Mean Square Error) was minimized and excellent recommendations were provided by a surprise library that employed incredibly potent algorithms like Singular Value Decomposition (SVD).

# Hybrid Filtering
Recent studies have shown that in some situations, a hybrid strategy that combines collaborative filtering with content-based filtering may be more successful than pure alternatives. These techniques can also be utilized to get around some of the issues that recommender systems frequently run into, such the sparsity and cold start issues.





