# Mobile-Price-Range-Prediction
Machine learning classification project
Mobile-Price-Range-Prediction
 
# Problem Statement
There are many things we consider before buying a mobile as we used our mobile for various purpose like connecting with our family & Office Colleagues, playing games, taking a photo’s to keep our memory alive. So this such specifications such as RAM, internal memory, Wi-Fi, 3G/4G connectivity etc. plays important role to buy a mobile. To analysis of this important factor from time to time and come up with the best setoff specifications and price ranges so that people will buy the mobile. Hence through the various ML modules we will help the company to estimate the price of mobiles according to feature so the maximum amount of sell will be possible.

# Data Description
We have been provided with the dataset containing the 2000 rows and 21 features
• Battery power - Total energy a battery can store in one time measured in mAh
• Blue - Has Bluetooth or not
• Clock_speed -speed at which microprocessor executes instructions
• Dual_sim - Has dual sim support or not
• Fc - Front Camera mega pixels
• Four_g - Has 4G or not
• Int_memory - Internal Memory in Gigabytes
• M_dep - Mobile Depth in cm
• Mobile_wt - Weight of mobile phone
• N_cores - Number of cores of processor
• Pc - Primary Camera mega pixels
• Px_height - Pixel Resolution Height
• Px_width - Pixel Resolution Width
• Ram - Random Access Memory in Mega Bytes
• Sc_h - Screen Height of mobile in cm
• Sc_w - Screen Width of mobile in cm
• Talk_time - longest time that a single battery charge will last when you are
• Three_g - Has 3G or not
• Touch_screen - Has touch screen or not
• Wifi - Has wifi or not
• Price_range - This is the target variable with value of 0(low cost), 1(medium cost),2(high cost) and 3(very high cost).



# Data Processing
Understanding and cleaning the data

# Data Exploration
Analyze the data through visualization

# Model Performed
• Decision Tree Classifier
• Random Forest Classifier
• K Nearest Neighbor
• Gradient Boosting Classifier
• XGB Classifier
• Support Vector Machine


## **<u>Conclusion:</u>**

#### We have reached the end of our mobile price range prediction project and have achieved a fairly good result for all the models implemented. We have discovered a lot of insights from the data through EDA which helps in determining which features will have a strong influence on the price range prediction. 

#### This kind of prediction is very important for businesses to understand which factors drive the price of a mobile phone and estimate the price of mobile phones accurately to give good competition to other manufacturers.

#### Let us summarize the whole work in few points below:

* The dataset contains 2000 records of mobile phone information with 21 features. There are 6 categorical features and 14 numerical features with price range as the target variable.

* The dataset was almost a cleaned one with no null values present or duplicate records found. Few features like pixel resolution height and screen width had zero values in few records which had to be removed before proceeding further.

* EDA was used to generate insights or to get all sorts of information of the features in the dataset. With the help of EDA, we got to know that

  * The target class data was mostly balanced with not much difference between each class.

  * Most of the categorical features had a similar distribution or count except the feature 'three_g'. There were very few records for mobile phones which doesn't support 3G. We can infer that almost all phones had 3G network access if not 4G.

  * Most of the numerical features follow an uniform distribution except few features like front camera, pixel resolution height and screen width which had a right skewed distribution.

  * The boxplots suggested us that there are few outliers in two features but we know that these values are very natural in real life, thus we didn't treat them as outliers.

  * Almost all categorical features had a similar distribution across all price ranges except 'three_g' where there were very few records of mobile phones not having 3G network access across all price ranges.

  * There is a slight increase in count for each feature in the very high cost category except the feature touch screen.

  * We can infer that the more we pay, more choices we get for mobile phones with all the features.

  * Battery power and RAM increases with the increase in price range and thus these two features will be an influential factor for predicting the price range.

  * Most of the other numerical features doesn't show a significant change with the price range.

* Through correlation analysis we got to know that,

  * RAM is the only feature which is strongly correlated with the target variable.

  * Most of the other independent variables were not strongly correlated to each other and hence we didn't need to remove or combine any feature.

  * Through correlation plots we have observed that except RAM, battery power, px_height and px_width are slightly correlated with the target variable and can be important features to determine the price ranges.

  * No categorical feature is strongly correlated with the target variable and interestingly touch screen had a low negative correlation with the target variable.

* We have implemented 6 classification models and have achieved a fairly good result for all the algorithms.

  * Logistic Regression
  * Random Forest
  * Gradient Boosting
  * XG Boost
  * K Nearest Neighbors
  * Support Vector Machines

* All the models have achieved an approx accuracy of 90% which shows that the data were properly classified.

* Logistic Regression and SVM has performed better than any other model by achieving an accuracy of 96% which is the highest among the 6 models implemented.

* Through the tree based methods we found out that RAM, battery power, px_height and px_width are the most important features for the prediction of price ranges.

* The tree based methods have performed poorly in comparison to the other classification methods.
