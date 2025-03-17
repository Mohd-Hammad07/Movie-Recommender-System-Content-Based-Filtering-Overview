# **Movie Recommender System (Content-Based Filtering)**  

## **Overview**  
This project is a **Content-Based Movie Recommender System** that suggests similar movies based on their descriptions using **Natural Language Processing (NLP)** techniques.  

## **Features**  
- **Movie Recommendations**: Suggests similar movies based on content.  
- **Content-Based Filtering** using metadata (title, genres, overview).  
- **Feature Engineering**: Stopword removal, vectorization (TF-IDF, Bag of Words).  
- **Cosine Similarity** for measuring movie similarity.  
- **Streamlit Web App** for easy user interaction.  

## **Dataset**  
- **Source**: [TMDB Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)  
- **Key Features**:  
  - **Title**: Movie name  
  - **Overview**: Short description  
  - **Genres**: Movie categories (Action, Drama, Comedy, etc.)  
  - **Keywords & Cast**: Important for similarity calculation  

## **Data Preprocessing**  
- **Handling Missing Values**: Dropped incomplete rows.  
- **Text Preprocessing**:  
  - Lowercasing  
  - Removing punctuation & stopwords  
  - Tokenization  
- **Vectorization Techniques**:  
  - **TF-IDF (Term Frequency - Inverse Document Frequency)**  
  - **Bag of Words (BoW)**  

## **Recommendation Algorithm**  
1. **Input**: User enters a movie (e.g., *Avengers*).  
2. **Feature Extraction**: Converts text into vectors using **TF-IDF**.  
3. **Cosine Similarity**: Measures similarity between movies.  
4. **Movie Suggestions**: Returns top similar movies.  

**Example:**  
For *Avengers*, recommendations may include:  
1. Iron Man  
2. Thor  
3. Guardians of the Galaxy  
4. Captain America  

## **Technologies Used**  
- **Python**: Pandas, NumPy, Scikit-learn, NLTK  
- **Vectorization**: TF-IDF, CountVectorizer, Cosine Similarity  
- **Deployment**: Streamlit  

## **Project Structure**  
```
📂 movie-recommender
│── app.py              # Streamlit web app
│── data/               # TMDB dataset
│── models/             # Saved models (TF-IDF, similarity matrix)
│── notebooks/          # Data exploration & model training
│── requirements.txt    # Dependencies
│── README.md           # Documentation
```


4. **Enter a Movie Name** to get recommendations.  

## **Challenges & Future Improvements**  
- **Cold Start Problem**: Address new user/movie challenges.  
- **Performance Optimization**: Improve computational efficiency.  
- **Deep Learning Models**: Consider Word2Vec or BERT for better recommendations.  
- **User Feedback**: Implement rating-based filtering for better accuracy.  

## **Business Impact & Applications**  
- **Netflix, Amazon Prime, YouTube**: Increase user engagement, retention, and revenue.  
- **E-commerce**: Product recommendations based on user preferences.  
- **Finance**: Personalized investment recommendations.  

## **References**  
- [TMDB Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)  
- [Scikit-Learn](https://scikit-learn.org/)  
- [NLTK](https://www.nltk.org/)  
- [Streamlit](https://streamlit.io/)  

