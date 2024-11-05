# 🏨 Hotel Reviews Sentiment Analysis

This project focused on analyzing hotel reviews using Natural Language Processing (NLP) techniques to classify sentiments effectively. We employed **Word2Vec** embeddings to transform text data into numerical vectors, enabling the application of machine learning models to detect patterns in review sentiments.

## 🗂️ Overview of the Process

- **Goal**: Classify hotel review sentiments using supervised learning models.
- **Techniques Used**:
  - **Word Embedding**: Word2Vec
  - **Classification Models**: Logistic Regression, Random Forest, Decision Tree

## 🧹 Data Preprocessing

Extensive data preprocessing was essential to prepare the reviews for analysis:

- **Handling Missing Values**: Ensured no gaps in data could skew model accuracy.
- **Data Cleaning**: Removed irrelevant characters and symbols for clarity.
- **Tokenization and Stop Words Removal**: Tokenized each review and eliminated common, uninformative words to focus on meaningful terms.
  
These steps prepared the text data for the Word2Vec model, enhancing feature quality by focusing on informative content.

## 🔠 Word2Vec Embedding

- **Purpose**: Transform text into numerical vectors while preserving semantic relationships between words.
- **Process**:
  - **Word2Vec Training**: Trained a Word2Vec model on the preprocessed review text, capturing word associations and context.
  - **Review Vectorization**: Each review was then represented as an aggregated vector of its word embeddings, providing a meaningful numerical format for sentiment classification.

## 🧑‍🏫 Classification Models

After vectorizing the reviews, we applied supervised machine learning models to classify sentiment:

1. **Logistic Regression** (Best Performing Model)
   - 🌟 **Accuracy**: High accuracy and well-balanced classification report.
   - **Why It Worked**: The linear approach of logistic regression matched well with the Word2Vec vector representation, effectively capturing sentiment patterns.

2. **Random Forest Classifier**
   - 🌲 Ensemble model offering robust classification.
   - **Performance**: Good accuracy, though slightly lower than logistic regression in this context.

3. **Decision Tree Classifier**
   - 🌳 Captured decision boundaries in the data but showed more variance compared to logistic regression.
   - **Performance**: Moderate accuracy, with a tendency to overfit.

### 📈 Model Evaluation

Each model was evaluated using a classification report to assess accuracy, precision, recall, and F1-score.

- **Result**: Logistic regression emerged as the best-fit model, offering the highest accuracy and balanced performance metrics, making it optimal for this sentiment analysis task.

## 📊 Key Insights from Word Cloud Analysis

A **word cloud** visualization of the hotel reviews highlighted prominent themes that indicate what aspects matter most to guests:

- **Main Themes**:
  - 🛏️ **Room Quality** and 🏨 **Overall Hotel Experience**: Words like "room," "hotel," "resort," and "day" indicate a strong focus on these aspects.
  - **Amenities**: Frequent mentions of "restaurant," "pool," "beach," and "food" show the importance of these amenities in guest experiences.
  - **Customer Service**: Words such as "staff," "nice," and "friendly" reflect the value of positive, friendly interactions in guest satisfaction.
  - **Areas for Improvement**: Terms like "problem" and "check" suggest common pain points related to service efficiency and check-in processes.

- **Implication**: Enhancing **room quality**, improving **service efficiency**, and investing in **amenities** could significantly boost guest satisfaction and improve overall ratings.

## ✅ Conclusion: Word2Vec + Logistic Regression as the Optimal Combination

- **Word2Vec Embeddings**: Provided a strong feature set by embedding semantic relationships into numerical form.
- **Logistic Regression**: Effectively leveraged these embeddings, resulting in a straightforward yet accurate classification of review sentiments.
- **Actionable Insight**: Enhancing key aspects identified in the word cloud (room quality, service, amenities) can lead to higher guest satisfaction.

> 📌 **Tip**: For future analysis, consider experimenting with alternative embeddings (e.g., GloVe, FastText) or deep learning approaches (e.g., LSTM or BERT) for potentially improved performance.

This combination of **Word2Vec** embeddings with **logistic regression** proved to be a reliable method for analyzing hotel review sentiments, capturing trends in customer feedback that provide actionable insights for service improvement.

