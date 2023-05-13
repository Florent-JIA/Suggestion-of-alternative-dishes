# 5.Suggestion-of-alternative-dishes
## Introduction
This project aims to provide restaurants with alternative menus to reduce the environmental impact of catering consumption.

For several years now, the environmental impact of products and services has been increasingly taken into account by individuals. This is also true for the food market: consuming locally to reduce CO2 emissions due to transport, consuming foods that in their production have a lower environmental impact...

We want to offer a solution for school/company canteens that offer large quantities of certain pre-determined meals. Our project focuses on the impact of the extraction, agriculture and product processing phases, so we are targeting organizations that source locally or wish to move towards this mode of supply. We want to offer them alternatives to the dishes they offer while respecting the following criteria: the dishes will try to be nutritionally similar and will have a better impact on the environment.

The solution we propose aims to enable the organizations concerned to reconcile their activity and their ethics while adapting to the environmental requirements that our economy and our organizations must face.

Thus our model will have to take a dish as a starter, determine which dishes at our disposal are nutritionally similar to this dish, in order, within these similar dishes, to recommend to the user more ecological substitutes than the starting dish.

## Data set
Firstly, we found a data set with 1,000,000 dishes and their ingredients. Due to the limitation of computer computing power, we randomly selected 3000 dishes.

Then, we found another dataset that recorded the energy, fat, sugar, fiber, protein, salt and nutrition score of each ingredient so that we could calculate the values of these variables for each dish.

Then, we calculated the ecoscore for each dish.

Finally, we got a [data set](https://github.com/Weizhe-JIA/5.Suggestion-of-alternative-dishes/blob/main/Recipe_ingredients_Variables.xls/) with 3000 dishes and values for 8 variables: energy, fat, sugar, fiber, protein, salt, nutrition score and ecoscore.

## Clustering
In order to find out the alternative dishes of the target dish, we cluster the 3000 dishes in the dataset according to those 7 variables: energy, fat, sugar, fiber, protein, salt and nutrition score, in order to find the dishes similar to the target dish.

![similarity](https://github.com/Weizhe-JIA/5.Suggestion-of-alternative-dishes/blob/main/imgs/similarity.png)
<br>(a) exemple of picking 10 similar dishes for a given dish

## Recommadation
By sorting the dishes found based on similarity according to the ecological score, we can get those dishes that are similar to the original dishes and have high ecological scores.
![ecoscore](https://github.com/Weizhe-JIA/5.Suggestion-of-alternative-dishes/blob/main/imgs/ecoscore.png)
<br>(b) sort the similar dishes based on the ecoscore

