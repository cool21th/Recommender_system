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
          User attributes: age, locations,..
          Product attributes: screen resolution, weight, RAM, etc...
      Target Y
          buy the product or not
          rating the product
          

Markov Models


Page Ranks


Hacker News Formula

reference: [How Hacker News ranking really works: scoring, controversy, and penalties](https://www.righto.com/2013/11/how-hacker-news-ranking-really-works.html)

    score = (((ups - downs - 1)^0.8)/(age+2)^gravity) * penalty
    gravity = 1.8
    penalty = multiploer to implement "business rules"
