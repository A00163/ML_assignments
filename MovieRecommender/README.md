### README: Movie Recommendation System

---

#### **Overview**
This project is a **movie recommendation system** built using the **MovieLens 100k dataset**. The system uses collaborative filtering techniques with deep learning to predict user ratings for movies and recommend top-k movies for each user. It leverages TensorFlow and Keras for building the recommendation model.

---

#### **Features**
- Trains a recommendation model using **user and movie embeddings**.
- Computes **Recall@10** to evaluate the quality of recommendations.
- Visualizes the **distribution of predicted ratings** and actual ratings.
- Provides functionality to recommend movies for specific users.

---

#### **Requirements**
Install the required libraries using the following command:
```bash
pip install tensorflow pandas matplotlib scikit-learn
```

---

#### **Dataset**
The project uses the **MovieLens 100k dataset**, which contains 100,000 movie ratings from 943 users on 1,682 movies. The dataset is publicly available at [MovieLens](https://grouplens.org/datasets/movielens/).

---

#### **How to Use**
1. **Download and Extract Dataset**  
   Download the dataset and extract the files. Ensure the `u.data` file is in the same directory as the script.

2. **Run the Code**  
   Execute the script in a Python environment (e.g., Jupyter Notebook, Google Colab).

3. **Train the Model**  
   The model is trained on the MovieLens dataset, splitting the data into training and testing sets.

4. **Evaluate the Model**  
   - The model computes **Recall@10** to evaluate recommendation performance.
   - Visualizations of predicted and actual ratings are generated.

5. **Recommend Movies**  
   Use the `recommend_movies()` function to get movie recommendations for a specific user.

---

#### **Key Functions**
1. **`recall(model, test_data, train_data, k=10)`**  
   Computes Recall@10 to evaluate how well the model recommends relevant movies.

2. **`recommend_movies(model, user_id, k=10)`**  
   Recommends top-k movies for a given user based on predicted ratings.

3. **`debug_predictions(model, user_id, train_data, test_data, movie_ids, k=10)`**  
   Debugs predictions for a specific user by comparing recommended movies with ground truth.

---

#### **File Structure**
- **`ml-100k/`**: Contains the MovieLens 100k dataset.
  - `u.data`: The main dataset file with user, movie, and rating information.
- **`Recommender.ipynb`**: Jupyter Notebook containing the implementation.
- **`recommender.py`**: Python script with the same implementation.

---

#### **Model Details**
1. **Inputs**:
   - `user_id`: Encoded user IDs.
   - `item_id`: Encoded movie IDs.

2. **Embedding Layers**:
   - User and movie embeddings with a size of 64.

3. **Interaction**:
   - A dot product between user and movie embeddings to compute their interaction score.

4. **Loss Function**:
   - Mean Squared Error (MSE) is used as the loss function.

5. **Optimizer**:
   - Adam optimizer with a learning rate of 0.001.

---

#### **Evaluation**
The model's performance is evaluated using **Recall@10**. For example:
- **Mean Recall@10**: 0.2438 (This indicates that, on average, ~24.38% of the relevant movies are present in the top-10 recommendations for each user).

---

#### **Example Usage**
To get movie recommendations for a specific user:
```python
user_id = 4
recommended_movies = recommend_movies(model, user_id, k=10)
print(f'Recommended movies for user {user_id}: {recommended_movies}')
```

To debug predictions for a specific user:
```python
debug_predictions(model, user_id, train_data, test_data, movie_ids, k=10)
```

---

#### **Visualization**
The script generates the following visualizations:
1. **Distribution of Predicted Ratings**: Displays the range and frequency of predicted ratings.
2. **Distribution of Actual Ratings**: Shows the frequency of actual ratings in the training data.

---

#### **Future Improvements**
- Implement **Neural Collaborative Filtering (NCF)** for better accuracy.
- Use additional features (e.g., movie genres, timestamps) for richer recommendations.
- Add support for **hybrid recommendation systems** (collaborative + content-based filtering).
- Improve hyperparameter tuning and embedding size optimization.



#### **License**
This project is licensed under the MIT License. Feel free to use or modify the code for personal or commercial purposes.