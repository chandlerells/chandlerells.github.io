# Third Blog Post

## Prompt: 

When building regression models, it often takes a lot of experience and knowledge about your data in order to determine the variables and transformation of variables that you want to include in the model
building process.  There are many variable selection techniques (or feature selection) but it can be a confusing practice when you are first learning.  
Read through these articles (and others if you'd like to find your own):

`For your blog post, write up a brief discussion of how you would plan to determine variables to use in a regression model.  What variable selection techniques do you prefer and why?.` 

## Response:

I think the first thing I would do to approach variables in a regression model is come up with a global set of variables based on background knowledge. This could be sought by a variety of ways such as expert opinion, 
industry knowledge, common sense, or intuition. I would then spend time with the global set of variables, looking to see if I could reduce any from the set by looking at their relationships with one another in the 
context of the response.

While challenging to rule variables in or out of model estimation based on individual statistical tests, I might try and standardize each predictor, run a simple linear regression model using each predictor,
and look at the corresponding t-tests and p-values provided. This could be an initial way to compare the importance of certain variables in the global set since they were standardized. I would also run some 
metric that attempts to calculate each variable's overall importance to be used for comparison. Having a global set of predictors to start I believe can be very helpful, especially in the instance of high dimensionality.

Based on the third article provided in the prompt, I would also spend a considerable amount of time doing EDA to help select the appropriate variables. I really liked the author's point that often we try to fit 
the data to our model instead of the opposite way around. The author layed out numerous issues with each of the common variable selection methods, while providing a general framework of variable selection by
conducting a proper EDA, spending a lot of time understanding the data and the various components that could make for a model that better optimizes bias-variance tradeoff. EDA can be useful here to understand
the global set of variables and how to further refine them or apply the proper transformation that leads to the best predive power.

While supplementing my EDA, as well as since modeling is fairly new to me, I would use many of the popular variables selection methods for my regression model for comparison. If I have the computational capacity, 
and the number of predictors is reasonable, I would conduct best subset selection. I like this because it seems to be fairly intuitive, and searches all possible model combinations, selecting the best one based on 
performance error. It also doesn't suffer from some of the same issues as stepwise, where a particular combination of predictors may be very powerful at prediction together, instead of selecting this by adding or
taking away one variable at a time. 
 
I would also do backwards stepwise, as this seems to be recommended more in practice, and starts with the most unbiased model. Lastly, I would perform some shrinkage method, such as LASSO, since it automatically
performs variable selection for me, by shrinking coefficient estimates to zero for the variables with the least predictive power. This would also be something that is helpful in the instance I am working with data
I am unfamiliar with. One thing I thought was interesting from the first article, which I may attempt to practice, is only doing variable selection on the predictors I am least confident about. While the article 
was in relation to IV's, I thought many of the ideas were transferable. It might be of value to not include variables I am confident in having a strong association with the response.


