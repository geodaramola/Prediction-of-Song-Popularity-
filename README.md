Predicting Song Popularity with Engineered Audio Features
📌 Project Overview

Bassline.io is exploring whether its existing engineered audio features can effectively predict the popularity of a song. This project evaluates the usefulness of those features by building and interpreting a machine learning model to predict song popularity.

The goal is not to deploy a production-ready model, but rather to assess:

Whether the current feature set has predictive value

Which features contribute most to song popularity

What limitations exist in the current feature engineering approach

🧠 Business Problem

The data science team at Bassline.io has previously engineered several audio-related features, including:

Danceability

Energy

Acousticness

Before investing further effort into feature development, the team wants to understand:

Are these features actually useful for predicting song popularity?

To answer this, we frame the task as a supervised regression problem where song popularity is predicted using the existing engineered features.

🎯 Objectives

Build a machine learning model to predict song popularity

Evaluate model performance using Mean Squared Error (MSE)

Interpret model results to determine feature usefulness

Identify limitations of the current feature set

Provide insights to guide future feature engineering efforts

📊 Dataset

~20,000 songs

Each row represents a song

Includes:

Engineered audio features (e.g. danceability, energy, acousticness)

Target variable: song_popularity

🧪 Methodology

Exploratory Data Analysis

Distribution of song popularity

Feature correlations

Detection of outliers and skewness

Baseline Modeling

Simple regression model to establish a performance benchmark

Model Development

Train regression models using engineered features

Compare performance across different modeling approaches

Evaluation

Primary metric: Mean Squared Error (MSE)

Residual and error analysis to understand model behavior

Interpretation

Feature importance analysis

Examination of which features drive predictions

Identification of weak or redundant features

Exploration of Alternatives

Feature selection techniques

Dimensionality reduction (e.g. PCA)

Discussion of trade-offs between interpretability and performance

📈 Evaluation Metric

Mean Squared Error (MSE) is used to assess predictive performance:

Penalizes larger errors more heavily

Appropriate for continuous popularity scores

Interpreted alongside qualitative error analysis rather than optimized blindly

🔍 Key Insights (Example)

(Replace with your actual findings)

Danceability and energy showed stronger predictive power than acousticness

Overall model performance suggests limited explanatory power from the current feature set alone

Prediction errors indicate difficulty modeling extremely popular or unpopular songs

Feature set likely lacks contextual or behavioral data needed for stronger predictions

⚠️ Limitations

Model is trained only on pre-engineered audio features

No listener behavior, genre context, or temporal effects included

Popularity is influenced by many non-audio factors not captured here

Model is not intended for production use

🚀 Future Work

Engineer additional features (e.g. tempo dynamics, lyrical sentiment)

Incorporate user engagement or playlist data

Explore nonlinear models with stronger interpretability tools

Revisit target definition (e.g. popularity buckets vs continuous score)

🛠️ Tech Stack

Python

pandas, numpy

scikit-learn

matplotlib / seaborn

