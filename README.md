# About the project
#### This project aims to build a model to predict whether it will rain the next day given weather information about the current day

# Key Achievements
* Trained and optimized a model to have an accuracy of 85% and an F2 score of 58% in predicting whether it will rain the next day. So the decrease in the accuracy is caused of false negatives overwhelmingly, as the data is unbalanced for the nature of having more days off rain
* Shrank the dataset to only the top eight distinguishing features and fit it to the model to have an accuracy of 84.4% and an F2 score of 55%
* Built three models for the same problem with different prediction tendencies (increasing in recall for positives) through modifying the class distribution in the training sets for each, using the shrunk dataset
* Considered the model with the lowest recall to be informing about high rain probability, considered the model with the highest recall to be informing about low rain probability, and considered the last model to be in-between
* Assigned a digit  to each of the three models to give a 3-digit binary number that the model that can inform about low probability is assigned the digit representing the lowest power of 2, and so on, and with that, the models are assigned 2^0, 2^1, and 2^2 with respect to the probability each can inform about, in order to combine their information to obtain a range of 0 to 7 indicating the degree of rain probability
* Found out that if the degree of 7 only is said to be indicating "positive rain" (i.e., the three models agree on "positive rain"), then the accuracy will reach up to 88% beating the curse of the false negatives to some degree

# Requirements
`Python` `NumPy`
`Pandas`
`matplotlib`
`scikit-learn`

# Execution
#### Locate `will_it_rain_tomorrow.ipynb` and run the following command:
```
jupyter notebook will_it_rain_tomorrow.ipynb
```

# Demonstration

#### [Google drive link](https://drive.google.com/file/d/1TQSPZYRlYxPVGmBk8n_qeH7sMHErnzCm/view?usp=share_link)


