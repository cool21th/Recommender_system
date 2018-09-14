# Recommender_system

Popularity

    A business wants to make money
    More buying makes more money


## Non-personalized

Your individual likes and dislikes aren't used for custom suggestions to you

    News feed
    E-commerce's products list
    


Personalized 



ex) Making supervised learning for recommendations
    
      Input X
          User attributes: age, locations, gender, race, occupation, education level, ..
          Product attributes: screen resolution, weight, RAM, etc...
      Target Y
          buy the product or not
          rating the product
          click on the article
          sign up for the newsletter
          
      Model
          Logistic Regression
          Random Forestakfm
            
          

Markov Models


Page Ranks


#### Hacker News Formula

reference: [How Hacker News ranking really works: scoring, controversy, and penalties](https://www.righto.com/2013/11/how-hacker-news-ranking-really-works.html)

    score = (((ups - downs - 1)^0.8)/(age+2)^gravity) * penalty
    gravity = 1.8
    penalty = multiploer to implement "business rules"
    
#### Reddit Formula

reference: [reddit’s new comment sorting system](https://redditblog.com/2009/10/15/reddits-new-comment-sorting-system/)

    score = sign(ups-downs) * log{max(1, |ups-downs|)} + age/45000
    log -> sublinear
    the more downvotes gets, the further scores goes down
    
    
#### Smoothing

    1000 4 star ratings  -> 3.999
    5 4 star ratings -> 3.83
    one 4 star rating -> 3.5
    
