# Drifting Upstream

This project explores a regression problem for the hypothetical record label, Regression Records, in which we seek to predict a song's popularity based on its music features. We examine 2 datasets (as indicated by 'Phase 1' and 'Phase 2') in which song popularity is conveyed respectively as either the target variable of total Spotify streams, or a popularity score (1-100). Music features in Phase 1 include tempo, danceability, valence, energy, acousticness, instrumentalness, liveness, speechiness, and mode. Music features in Phase 2 are the same, minus mode, plus duration and loudness. Phase 1's best model is a Random Forest Regressor with a mean absolute error score on the test set of ~268 million streams. Phase 2's best model is an Extra Trees Regressor with a mean absolute error score on the test set of ~15.30. While these models enable Regression Records to make informed business decisions from benchmark predictions regarding which of its songs are most likely to become popular, there is ample room for expansion in future work to explore additional features and observations, and more specifically quantify a success metric. Details on the process and further implications are indicated in the following files.

## Data

**Phase 1**
- spotify_2023.csv (original dataframe of 953 rows and 24 columns)
- spotify_2023_cleaned.csv (phase 1a modeling dataframe of 945 rows and 36 columns)
- spotify_2023_streams_and_features.csv (phase 1b modeling dataframe of 945 rows and 10 columns)
- spotify_additional_data.csv (experimental phase 1 data wrangling additional dataframe of 20,594 rows and 24 columns)

**Phase 2**
- spotify_30k.csv (second dataframe of 32,833 rows and 23 columns)
- spotify_30k_cleaned.csv (phase 2 modeling dataframe of 32,833 rows and 54 columns)

## Notebooks

**Phase 1**
- data_wrangling_1.ipynb (phase 1 data wrangling)
- eda_1.ipynb (phase 1 exploratory data analysis)
- preprocess_and_train_1.ipynb (phase 1 preprocessing, training, and modeling)

**Phase 2**
- tsa_2.ipynb (phase 2 time series analysis)
- dw_and_eda_2.ipynb (phase 2 data wrangling and exploratory data analysis)
- modeling_2.ipynb (phase 2 preprocessing, training, and modeling)

### Hyperparameter Tuning
- hp_et.ipynb (Extra Trees Regressor hyperparameter tuning and feature scaling)
- hp_gb.ipynb (Gradient Boosting Regressor hyperparameter tuning and feature scaling)
- hp_hgb.ipynb (Hist Gradient Boosting Regressor hyperparameter tuning and feature scaling)
- hp_rf.ipynb (Random Forest Regressor hyperparameter tuning and feature scaling)
- hp_xgb.ipynb (XGBoost Regressor hyperparameter tuning and feature scaling)

## Reports

- Best_Model_Metrics.pdf (feature importance, hyperparameters, and mean absolute error scores for phase 2 best model: Extra Trees Regressor)
- Project_Presentation.pdf (PDF of 20-slide PowerPoint presentation of project summary and key findings)
- Project_Presentation.pptx (20-slide PowerPoint presentation of project summary and key findings)
- Project_Proposal.pdf (original phase 1 project proposal)
- Project_Report.pdf (18-page written report of project summary and key findings)
