# Movie Recommendation System

### About This Project:
This is a **Streamlit web application** that provides personalized movie recommendations based on user interests. The system employs a **content-based filtering algorithm**, which suggests movies with similar attributes to the ones the user has shown interest in. Below are some screenshots showcasing the app's interface:

![Screenshot 1](https://github.com/Kyouma45/Movie_Recommendation_System/assets/67496078/a9638c40-56db-44f4-a99a-360325c64e3a)
![Screenshot 2](https://github.com/Kyouma45/Movie_Recommendation_System/assets/67496078/498d35c6-c8c0-444b-afaa-c461ba7a87c8)
![Screenshot 3](https://github.com/Kyouma45/Movie_Recommendation_System/assets/67496078/d724272b-58bb-4b47-acb2-e8ede2f14bda)

### Features:
This model uses a **content-based filtering algorithm**.

**Content-Based Filtering**:
- Content-based systems use item attributes (such as movie genres, cast, director, etc.) to make recommendations.
- Systems like Twitter and YouTube use similar algorithms to suggest content based on user preferences.
- The system forms embeddings (vectors) based on features, such as the movies you watch or the music you listen to.
- **Recommendation Approach**: It creates a vector of item features and compares them with the user’s preferences to recommend similar items.
- **Advantages**: Personalized suggestions based on past user behavior.
- **Limitations**: This may lead to excessive specialization (i.e., the system might only recommend items from the same categories, missing out on other potentially interesting items).

### Data:
Data is sourced from the [TMDb Movie Metadata Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/data).

### Model Overview:
The model uses **Cosine Similarity** to compare movies:
1. **Cosine Similarity** is a metric that measures the similarity between two vectors.
2. Vectors are generated from movie features using a **NumPy array**.
3. The `cosine_similarity()` function calculates the similarity between two vectors, with values ranging from [0,1].
   - **0**: Completely dissimilar.
   - **1**: Completely similar.

### Steps to Run the Project:

1. Clone the repository:
   ```bash
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

4. Install the requirements
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
