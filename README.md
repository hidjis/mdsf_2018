# Meilleur Data Scientist de France 2018

This is my code for the Top 10 solution in the competition ["Meilleur Data Scientist de France 2018"](https://www.meilleurdatascientistdefrance.com/) (Best data scientist of France 2018).

I used a single [lightgbm model](https://github.com/Microsoft/LightGBM/tree/master/python-package) to achieve a logloss ~0.92. The model runs in less than 40 seconds on a laptop with an i5 CPU and 8G of RAM. The environement is a python docker image from Kaggle:

```
python : 3.6.4 |Anaconda custom (64-bit)| (default, Jan 16 2018, 18:10:19) 
[GCC 7.2.0]
pandas : 0.20.3
numpy : 1.13.3
sklearn : 0.19.1
lightgbm : 2.1.0
```

# Context

[Label Emmaüs](https://www.label-emmaus.co/fr/) offers for sale objects renovated or created by the movement
Emmaüs. The purpose of this challenge is to estimate the time to sale of each object.

The task is a **Multiclass classification**, with 3 classes:

* 0 : between 0 et 10 days
* 1 : between 10 et 60 days
* 2 : more than 60 days

The evaluation metric is **logloss** 
