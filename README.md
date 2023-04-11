# Book Recommendation System - Unsupervised ML

**Problem Statement:**

The rise of internet services such as Youtube, Amazon, and Netflix has resulted in an increase in the popularity of recommender systems. Recommender systems are algorithms designed to suggest relevant items to users based on their preferences. They have become essential in various industries, including e-commerce, online advertising, and streaming services. In this project, we will develop a book recommendation system for users based on the Book-Crossing dataset. We will use unsupervised machine learning techniques such as exploratory data analysis, content-based filtering, collaborative filtering, and a hybrid approach that combines content-based and collaborative filtering.

**Book-Crossing Dataset:**

The Book-Crossing dataset contains three files: Users, Books, and Ratings. The Users file contains demographic information about users, including their location and age. The Books file provides information about books, including their ISBN, author, title, and publication year. The Ratings file contains information about the ratings given by users to books. Ratings range from 1 to 10, with higher values indicating higher appreciation. Some ratings are implicit and expressed by 0.5.

**Exploratory Data Analysis (EDA):**

Before developing our recommendation models, we will perform EDA to understand the characteristics of the dataset. EDA helps us to identify missing values, outliers, and correlations between variables. It also provides insights into the distribution of data, which can inform our modeling decisions.

**Content-Based Filtering:**

Our first ML model is based on content-based filtering.The ML model 1 is based on content-based filtering. It recommends books to users based on their past preferences. The model first cleans and preprocesses the dataset by removing unwanted columns and duplicating rows. It then vectorizes the text data by tokenizing and converting them into numerical data using TfidfVectorizer. After vectorizing the text data, it creates a cosine similarity matrix that measures the similarity between each book based on their textual features. Finally, the model recommends top-n similar books to a given book based on their cosine similarity score.

**Collaborative Filtering:**

ML Model 2:The ML model 2 is based on collaborative filtering. It recommends books to users based on the preferences of similar users. The model first cleans and preprocesses the dataset by removing unwanted columns and duplicating rows. It then sets a popularity threshold to select only popular books and creates a sparse matrix of user-item ratings. The model then computes pairwise cosine similarity between the rows of the sparse matrix to identify similar users. Finally, the model recommends top-n books to a given user based on the ratings of similar users.

**Hybrid Approach :**

ML Model 3:The ML model 3 is a hybrid approach that combines content-based and collaborative filtering. It recommends books to users based on both their past preferences and the preferences of similar users. The model first cleans and preprocesses the dataset by removing unwanted columns and duplicating rows. It then sets a popularity threshold to select only popular books and creates a sparse matrix of user-item ratings. The model then creates a content-based filtering approach by counting the number of ratings for each book title and selecting the books with total ratings greater than or equal to 50. The model then computes pairwise cosine similarity between the rows of the sparse matrix to identify similar users. Finally, the model recommends top-n books to a given user based on the combination of content-based and collaborative filtering.

Overall, all three ML models are designed to recommend books to users based on their preferences. Model 1 is based on the textual features of the books, Model 2 is based on the preferences of similar users, and Model 3 is a combination of both

**Conclusion:**

The development of recommender systems has become increasingly important in various industries, including e-commerce, online advertising, and streaming services. the book recommendation system developed using the Book-Crossing dataset has three ML models based on unsupervised learning techniques: content-based filtering, collaborative filtering, and a hybrid approach that combines both. These models use different approaches to recommend books to users based on their preferences. The content-based filtering approach recommends books based on the textual features of the books, while the collaborative filtering approach recommends books based on the preferences of similar users. The hybrid approach combines both and recommends books based on the combination of content-based and collaborative filtering.
