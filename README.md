# SNR-prediction
Predicting signal to noise ratio in vehicle to vehicle connection in two scenarios(urban, highway) using 10 features.
most of the code is data cleaning and feature engineering.
dataset is scaled using standard scaler. three different models are used for both scenarios.
## KNN(K nearest neighbor)
### Pros
* no training phase(low cost)
* simple algorithm 
* first choice on supervised porblems
### Cons
* unable to learn complex datasets
* hyperparameter setting(K value)
#### link
https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html
## MLP(multi layer perceptron)
### Pros
* can learn multiple complexities
* suitable for both regression and classification 
* have various agorithms to prevent overfitting
### Cons
* learning time
* hyperparameter setting(layers and neurons)
#### link
https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html
## RF(random forrest)
### Pros
* can learn multiple complexities
* performs well on classification tasks 
* features with discrete nature can increase performance in random forrest
### Cons
* suitable for only classification
* hyperparameter setting(number of trees)
#### link
https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
## Performance
all models performed around a certain score
* KNN: 96.22% (urban), 90.28% (highway)
* MLP: 96.78% (urban), 90.33% (highway)
* RF: 96.38% (urban), 89.35(highway)
### Urban
![3](https://user-images.githubusercontent.com/95940606/197838871-56303e3d-1e5f-4278-9120-0be2de19857b.png)
### Highway
![4](https://user-images.githubusercontent.com/95940606/197839215-8a348448-b0c4-4a86-845d-4e2200f23c74.png)
## Conclusion
data distribution can vary final score alot as it have in our two scenarios. but data cleaning and model selection can improve final result. but if we want to summerize these three models we would have this
* KNN: fast and free
* MLP: reliable and powerful
* RF: discriminative and classifier
