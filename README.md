# Real-time Sentiment Analysis of Business Reviews using Kafka and PySpark

## Overview

In this project, we simulated streaming business reviews in real-time and performed ML prediction, namely sentiment analysis on the streamed data using PySpark/PyTorch. We simulated data streaming using Apache Kafka and received the streaming data using PySpark, where we performed sentiment analysis on the review and stored this information. In the system architecture, we considered both, the non-distributed setup and distributed setup in storing our streaming data at the producer(Kafka) and reflect on any performance improvements. 

Sentiment analysis is the process of identifying and classifying the opinions and emotions expressed in a piece of text. It has numerous applications in areas such as marketing, customer service, and political analysis. We built a simple Logistic Regression Model pipeline in PySpark, and finetuned BERT in PyTorch to classify whether the reviews are positive, negative or neutral. And finally, we developed a dashboard that displays a real-time analysis of customer reviews, sentiment analysis results and other relevant metrics using Streamlit.

## Objectives achieved

#### Producer:

1. Setup kafka to store data in a distributed setup for efficient parallel processing.

#### Consumer:

1. Perform sentiment analysis on the stream of reviews.
2. Populate data in a database for further analysis and visualization.
3. Setup multiple consumers to process data in parallel. 

#### Overall:

1. Compare performance differences between distributed setup vs non-distributed setup.
2. Develop the user-friendly dashboard to display the sentiment analysis results in real-time.

## Methodology

The project will be implemented using the following methodology:
1. **Streaming Pipeline:** 

Simulate streaming of business reviews in real-time using native Python / Apache Spark.

2. **Model Building:**

    * Build a Logistic Regression Model pipeline to classify whether the reviews as negative or positive using PySpark's Machine Learning (ML) library.

    * Here, our focus is not to build a very accurate classification model but to see how to use any model and return results on streaming data.

    * Use PySpark to clean and preprocess the reviews, which may involve tasks such as tokenization, stop word removal, and stemming, as well as train the model.

3. **Workflow:**

    * Receive a stream of reviews.

    * Clean the reviews, and preprocess them to perform prediction.

    * Perform sentiment analysis on these reviews using PySpark's ML library.

    * Store the analyzed data in a database for further analysis and visualization.

4. **User-Interface:**

    * Develop a user-friendly dashboard to display the sentiment analysis results in real-time using Streamlit.

    * Streamlit is a Python library that can be used to create interactive web-based dashboards.

5. **Dataset source:**

    * https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset


## TOOLS AND TECHNOLOGIES

The following tools and technologies will be used in this project:

1. **PySpark:** for distributed processing of data
2. **Apache Kafka:** to simulate real-time streaming of data
3. **Python:** for programming the project
4. **Streamlit:** for developing the dashboard
5. **CSV / MySQL:** for storing the analyzed data
