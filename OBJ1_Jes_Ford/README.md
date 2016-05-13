# OBJ1: Random Forest Regressor for the win

A simplified version of my notebook from Objective 1 is in `code/VisionZero.ipynb`.

It reads in the data, selects only the rows that have values for **adt** 
(the target value), and filters out columns that have strings in them (anything 
that couldn't be interpreted as a number). This is 77 features for training. 
I would have liked to code some of the other 15 variables into numbers but we 
ran out of time. There are more detailed notes in the notebook.

I tried several different models, but the Random Forest Regressor was the most 
successful, getting an r^2 score of about ~82%.

A plot of feature importance is given in `images/feature_importance.png`.

Applying the (best) trained model to the rows of data for which **adt** is unknown 
yields the predictions given in `output/predictions.csv`.

**contact:** jesford.data@gmail.com
