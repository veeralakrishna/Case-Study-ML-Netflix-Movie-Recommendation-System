# Case-Study-ML-Netflix-Movie-Recommendation-System
---
A Machine Learning Case Study for Recommendation System of movies based on collaborative filtering and content based filtering.

### Business Problem 
Netflix is all about connecting people to the movies they love. To help customers find those movies, they developed world-class movie recommendation system: CinematchSM. Its job is to predict whether someone will enjoy a movie based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes. And while Cinematch is doing pretty well, it can always be made better. Now there are a lot of interesting alternative approaches to how Cinematch works that netflix haven’t tried. Some are described in the literature, some aren’t. We’re curious whether any of these can beat Cinematch by making better predictions. Because, frankly, if there is a much better approach it could make a big difference to our customers and our business. Credits: https://www.netflixprize.com/rules.html

### Problem Statement 
Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on the same training data set. (Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.)

### Sources 
* https://www.netflixprize.com/rules.html
* https://www.kaggle.com/netflix-inc/netflix-prize-data
* Netflix blog: https://medium.com/netflix-techblog/netflix-recommendations-beyond-the-5-stars-part-1-55838468f429
* surprise library: http://surpriselib.com/ (we use many models from this library)
* surprise library doc: http://surprise.readthedocs.io/en/stable/getting_started.html (we use many models from this library)
* installing surprise: https://github.com/NicolasHug/Surprise#installation
* Research paper: http://courses.ischool.berkeley.edu/i290-dm/s11/SECURE/a1-koren.pdf (most of our work was inspired by this paper)
* SVD Decomposition : https://www.youtube.com/watch?v=P5mlg91as1c
### Real world/Business Objectives and constraints 
#### Objectives:
* Predict the rating that a user would give to a movie that he has not yet rated.
* Minimize the difference between predicted and actual rating (RMSE and MAPE) 
#### Constraints:
* Some form of interpretability.
* There is no low latency requirement as the recommended movies can be precomputed earlier.
### Type of Data:
* There are 17770 unique movie IDs.
* There are 480189 unique user IDs.
* There are ratings. Ratings are on a five star (integral) scale from 1 to 5.
* There is a date on which the movie is watched by the user in the format YYYY-MM-DD.
### Getting Started
Start by downloading the project and run "NetflixMoviesRecommendation.ipynb" file in ipython-notebook.

### Prerequisites
You need to have installed following softwares and libraries in your machine before running this project.

* Python 3
* Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, scipy.
* XGBoost
* Surprise
#### Installing
* Python 3: https://www.python.org/downloads/
* Anaconda: https://www.anaconda.com/download/
* XGBoost: conda install -c conda-forge xgboost
* Surprise: pip install surprise
#### Built With
* ipython-notebook - Python Text Editor
* sklearn - Machine learning library
* seaborn, matplotlib.pyplot, - Visualization libraries
* numpy, scipy- number python library
* pandas - data handling library
* XGBoost - Used for making regression models
* Surprise - used for making recommendation system models
### Authors
Veerala Hari Krishna - Complete work
### Acknowledgments
Applied AI Course
