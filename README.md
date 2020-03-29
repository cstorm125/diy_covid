# (Do Not) Do-It-Yourself COVID-19 "Data Scientist" Kit 

This notebook offers a drag-and-drop interface for polynomial and exponential curve fitting that will allow you to predict COVID-19 cases in Thailand like a "data scientist" with just some hyperparameter tuning, and why you should or should not do it.

Clearly, polynomial curves with one coefficient (aka a flat line) or two coefficients (aka a straight line) are reliably bad with MAPE of over 50% over all number of days used to trained. But more importantly, even if you look at models which do reasonably well such as polynomial with 4, 5 and 6 coefficients, and the exponential curve, you can see that these models have quite large variance in their performance with range from 10% up to 40% MAPE.

At no point in time is one model "the best" for this prediction. This is to be expected since:
1. We have very few training data points
2. What we are trying to predict has a very dynamic nature
3. We do not have any means to obtain the features that might describe that dynamic nature

Now then, if you are now asking yourself:

> Why are we trying to apply statistical modeling (machine learning) to the ONE situation where we are taught in every single textbook that it is not suitable for? 

Then I have accomplished my goal with this notebook.