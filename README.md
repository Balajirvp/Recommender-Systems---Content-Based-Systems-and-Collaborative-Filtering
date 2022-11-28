# Recommender Systems - Content Based Systems and Collaborative Filtering

## I) Overview

Created Recommender systems using TMDB movie dataset by leveraging the concepts of Content Based Systems and Collaborative Filtering.

## II) Contents of the Jupyter Notebook

### Section 1 - Exploratory Data Analysis
- 1.1 Dropping Features
- 1.2 Updating Features
- 1.3 Feature Engineering

### Section 2 - Simple Recommender System
- 2.1 Creating a simple recommender system to show the top N movies at an overall level
- 2.2 Creating a simple recommender system to show the top N movies based on genre

### Section 3 - Content Based Recommender System
- 3.1 Movie Overview Based Recommender
- 3.2 Movie Metadata Based Recommender

### Section 4 - Collaborative Filtering System
- 4.1 Memory-Based Systems
  - 4.1.1 User-Based Collaborative Filtering
  - 4.1.2 Item-Based Collaborative Filtering
- 4.2 Model-Based Systems
  
## III) Key Packages/Functions used
 
- pandas - 1.4.4
- numpy - 1.21.5
- SentenceTransformer (from sentence_transformers) - 2.2.2
  - Model used: all-mpnet-base-v2
- cosine_similarity (from sklearn.metrics.pairwise) - 1.0.2
- SVDpp (from surprise) - 1.1.3
- Reader, Dataset (from surprise) - 1.1.3
- cross_validate (from surprise.model_selection) - 1.1.3

## IV) Predicted Recommendations

### 1) Simple Recommender System

Top 15 movies at an Overall level

![image](https://user-images.githubusercontent.com/104417912/203612892-4bb74b0a-2f0b-4dbb-8e4f-ae7f5666cc9b.png)

Top 15 movies based on 'Horror' genre 

![image](https://user-images.githubusercontent.com/104417912/203615171-cd6a97d1-22ba-4ad3-9811-b2cd501b7de4.png)

### 2) Content Based Recommender System

#### 2.1) Movie Overview Based Recommender 

- Top 15 movies recommended to a user who has watched 'The Godfather'

![image](https://user-images.githubusercontent.com/104417912/203613803-ed43dce0-1489-417a-b154-c8ed47958d1c.png)

- Top 15 movies recommended to a user who has watched 'The Notebook'

![image](https://user-images.githubusercontent.com/104417912/203614064-45e34bf1-965c-4f8f-904e-f1b6de15ec6f.png)

#### 2.2) Movie Metadata Based Recommender

- Top 15 movies recommended to a user who has watched 'The Godfather'

![image](https://user-images.githubusercontent.com/104417912/203614858-7d3babc8-f8e8-408a-8a22-5fafd95ab9e5.png)

- Top 15 movies recommended to a user who has watched 'The Dark Knight'

![image](https://user-images.githubusercontent.com/104417912/203614558-277061d6-a616-4a14-8d27-6c6a19e32c7c.png)

- Top 15 movies recommended to a user who has watched the movies in the below movie list

movie_list = ['The Lion King', 'Se7en', 'Toy Story', 'Blade Runner', 'Quantum of Solace', 'Casino Royale', 'Skyfall']

![image](https://user-images.githubusercontent.com/104417912/203616491-6bbba44f-a76d-4325-a075-0c0ff4998ad9.png)




### 3) Collaborative Filtering System

#### 3.1) Memory-Based Systems

- User-Based Collaborative Filtering

  - Top 15 movies recommended for user number 39
  
  ![image](https://user-images.githubusercontent.com/104417912/203617503-a3a6c9a1-b805-46d5-9214-54de675d6cd6.png)

- Item-Based Collaborative Filtering

  - Top 15 movies recommended for user number 39
  
  ![image](https://user-images.githubusercontent.com/104417912/203617620-3adc3627-6034-4658-acc9-55bc81eb6e5e.png)

#### 3.2) Model-Based Systems

- Top 15 movies recommended for user number 39

![image](https://user-images.githubusercontent.com/104417912/203617712-402b0b40-c15f-43ed-bdeb-b68a934098c4.png)

## V) References 

http://infolab.stanford.edu/~ullman/mmds/ch9.pdf 

https://www.kaggle.com/code/rounakbanik/movie-recommender-systems 

https://medium.com/grabngoinfo/recommendation-system-user-based-collaborative-filtering-a2e76e3e15c4 

https://towardsdatascience.com/building-and-testing-recommender-systems-with-surprise-step-by-step-d4ba702ef80b 

https://github.com/NicolasHug/Surprise/tree/master/examples
