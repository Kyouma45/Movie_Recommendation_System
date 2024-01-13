# Movie Recommendation System

### About this project:
This is a streamlit web application that can recommend various kinds of similar movies based on an user interest. Here are some screenshots:
![Screenshot from 2024-01-13 19-49-08](https://github.com/Kyouma45/Movie_Recommendation_System/assets/67496078/a9638c40-56db-44f4-a99a-360325c64e3a)

![Screenshot from 2024-01-13 19-50-20](https://github.com/Kyouma45/Movie_Recommendation_System/assets/67496078/498d35c6-c8c0-444b-afaa-c461ba7a87c8)
![Screenshot from 2024-01-13 19-51-44](https://github.com/Kyouma45/Movie_Recommendation_System/assets/67496078/d724272b-58bb-4b47-acb2-e8ede2f14bda)


This model uses content-based filetring algorithm.

 Content Based :

 + Content-based systems, which use characteristic information and takes item attriubutes into consideration.

  + Twitter, Youtube.

  + Which music you are listening, what singer are you watching. Form embeddings for the features.

  + User specific actions or similar items reccomendation.

  + It will create a vector of it.

  + These systems make recommendations using a user's item and profile features. They hypothesize that if a user was interested in an item in the past, they will once again be interested in it in the future

  + One issue that arises is making obvious recommendations because of excessive specialization (user A is only interested in categories B, C, and D, and the system is not able to recommend items outside those categories, even though they could be interesting to them).



### Data
Data used from https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/data

### Concept used to build the model.pkl file : cosine_similarity

1. Cosine Similarity is a metric that allows you to measure the similarity of the documents.

2. In order to demonstrate cosine similarity function we need vectors. Here vectors are numpy array.

3. Finally, Once we have vectors, We can call cosine_similarity() by passing both vectors. It will calculate the cosine similarity between these two.

4. It will be a value between [0,1]. If it is 0 then both vectors are complete different. But in the place of that if it is 1, It will be completely similar.

### Steps to run:
1. Clone the repository
   ```
     https://github.com/Kyouma45/Movie_Recommendation_System
   ```
2. Create a conda environment after opening the repository
   make sure that you are using python>=3.7
   
   ```
   conda create -n movie python=3.7.10 -y
   ```
   ```
   conda activate movie
   ```

4. Install the requiremetnts
   ```
     pip install -r requirements.txt
   ```
5. Generate models
   ```
   #run this notebook file to generate models
   Movie_Recommender_System.ipynb
   ```
6. Now run
   ```
   streamlit run app.py
   ```
