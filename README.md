
# Predicting Video Engagement for Educational Content

## Introduction

Engagement is pivotal in educational videos, directly impacting the learning experience. Engaging content captivates the viewer, leading to prolonged viewing durations crucial for effective learning. This project delves into the understanding of factors that influence engagement in educational content. Through supervised machine learning, we predict a video's engagement level using various features extracted from transcripts, audio tracks, and hosting platforms.

## Dataset Overview

The project dataset comprises two files: `train.csv` and `test.csv`. Each file row represents an individual educational video, with multiple features describing the content. The target variable, `engagement`, is binary, indicating whether the median watch percentage across viewers is at least 30% (True) or below (False).

-   `train.csv`: Utilized for model training, it contains both features and the target variable.
-   `test.csv`: Used for model testing, it contains only features.

## Features Description

-   `title_word_count`: Word count in the video title.
-   `document_entropy`: Score reflecting the diversity of video topics based on the transcript. A lower score suggests a more cohesive video.
-   `freshness`: Days since the video's publication (calculated from 01/01/1970). Recent videos have higher values.
-   `easiness`: Text difficulty score from the transcript, with lower scores hinting at complex language.
-   `fraction_stopword_presence`: Percentage of stopwords in the video transcript.
-   `speaker_speed`: Presenter's average speaking rate (words/minute). ... (other features as listed in the notebook)

## Installation and Setup

1.  Clone this repository.
2.  Install required Python packages:

Copy code

`pip install -r requirements.txt` 

3.  Open and run the Jupyter notebook: `Predicting_Video_Engagement_for_Educational_Content.ipynb`.

## Usage

To predict video engagement:

1.  Load your data into the notebook.
2.  Follow the data preprocessing steps.
3.  Train the model using the training dataset.
4.  Evaluate the model and make predictions using the test dataset.

## Exploratory Data Analysis (EDA) Highlights

-   Distribution of target variable.
-   Correlation between features.
-   other EDA highlights as detailed in the notebook

## Modeling and Results

The project employs various machine learning models, including:

-   Logistic Regression
-   Random Forest Classifier
-   Gradient Boosting ... (other models as mentioned in the notebook)

Model performances are evaluated based on accuracy, ROC-AUC, and other relevant metrics.

## Conclusion

Insights and findings derived from the analysis are presented, highlighting the significance of certain features in predicting video engagement.

## License

MIT License