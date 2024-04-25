# Enhancing Restaurant Serviced with Customer Reviews - BERTopic Modeling

## Project Overview
Leveraging data from Yelp, the project consolidates reviews to rate each aspect of a restaurant's service, such as food, service, ambiance, and more. A distinct feature of the code is its capability to generate comments automatically if the ratings are exceptionally low or high, summarizing the majority's sentiments. This innovative approach is poised to establish market trends based on available customer data, guiding restaurants in tailoring their services to current customer preferences.

## Objective
The project's primary goal is to dissect and evaluate multi-dimensional aspects of restaurant reviews, utilizing these insights to provide actionable recommendations for service enhancement and to foster an environment of customer satisfaction.

## Data Sources and Selection Criteria:
Utilizing the yelp_academic_dataset_business.json and yelp_academic_dataset_review.json files, the team applies rigorous filtering criteria to focus on operational restaurants in Arizona with substantial review histories post-2019.

## Methodology:
1. **Data Preparation** - The project uses Pandas for data manipulation, focusing on reviews and businesses in Arizona. Data is cleaned and preprocessed, with textual reviews undergoing natural language processing to facilitate further analysis.
2. **Topic Modeling** - Latent Dirichlet Allocation (LDA) is employed to categorize the review content into distinct operational aspects of the restaurant industry, such as food quality, service, and ambiance.
3. **Sentiment Analysis** - The sentiment of each review is quantified using the VaderSentiment library, which evaluates the tone and assigns a sentiment score.
4. **Topic Modeling** - Latent Dirichlet Allocation (LDA) and TF-IDF vectorization are utilized to identify and extract common themes within the reviews.
5. **Machine Learning** - Using supervised learning algorithms, the project aims to predict ratings for various restaurant aspects. Tools such as Scikit-learn's MultinomialNB and SVC are employed for classification tasks.
6. **Business Analysis** - The project investigates the number of reviews, unique customer count, and the distribution of star ratings to understand the data's breadth and depth.


## Final Selection Criteria:
- Restaurants located in Arizona.
- Restaurants that are still in operation.
- Restaurants with more than 200 reviews.
- Reviews from the year 2019 onwards.

## Sentiment Analysis:
> Sentiment analysis algorithms are used to evaluate the tone of the reviews, generating sentiment scores that range from highly negative to highly positive.
> Natural Language Processing (NLP) techniques, such as tokenization, stop-word filtering, and lemmatization, are applied to process the review text for analysis.
> A polarity score is assigned to each review using TextBlob, contributing to the aggregate sentiment score for each thematic category.

## Data Analysis:
> For each topic, reviews are aggregated to calculate the average sentiment score, reflecting public opinion and identifying areas needing improvement.
> Statistical methods are applied to ensure the robustness of the analysis, accounting for potential biases such as geographical skew or temporal changes.

## Sentiment Scores Calculation:
> A systematic approach is taken to calculate sentiment scores for various operational aspects of restaurants, with the sentiment analysis results fed into a predictive model.
> The model predicts ratings for individual aspects based on the sentiment scores derived from the review text, providing a comprehensive assessment.

## Application Development:
> A Streamlit application is developed to enable interactive analysis, allowing users to enter a restaurant's name and receive a detailed sentiment breakdown for different aspects.
> This application is designed to serve as a tool for potential customers to make informed decisions and restaurant owners to gain insights into public perception.

## Insights and Implications:
> The analysis offers insights into customer preferences, service quality, and potential market trends in Arizona's restaurant industry.
> The project outputs can inform business decisions related to market entry, expansion strategies, and customer experience improvements.

## Findings
1. **Identified Themes:** Topics such as "Italian Cuisine Experience" and "Japanese Food Dining Experience" highlighted specific cuisines' popularity. Other themes like "Service and Dining Out" and "Breakfast and Coffee Shops" indicated that customers often focused on particular aspects of their dining experience, such as service quality or the breakfast offerings.
2. **Sentiment Association:** By associating sentiment scores with each theme, the analysis provided a granular view of customer satisfaction levels. For example, topics like "Ambiance and Enjoyment" and "Customer Service During COVID" showcased how certain aspects significantly influenced overall satisfaction.
3. **Negative Feedback Insight:** Although the initial topic modeling focused on positive aspects, it was noted that further analysis specifically on negative reviews could reveal crucial areas for improvement.
