# PIC16B-Project
```
X . .
. X .
. O O
```

# Project Proposal

## Abstract

Often times, people don't like the soundtrack selections in movies. Well we have a solution for that! We want to create a website that looks at scenes of a movie or play and creates a customized soundtrack for that scene based on your own Spotify music tastes.

Intitally, we will offer a select few famous scenes from movies that we conduct sentiment analysis on. From there we will cross reference our results to a user's own music preferences on their Spotify account to generate a unique song for the scence customized to the users preferences. 

## Planned Deliverables

For a "fully successful" project, we would like to have a nice looking web app that a user can easily interface with, with a place for a user to log-in to their Spotify account, select a scene for matching, and outputs a song corresponding to the mood of the scene and the user's music taste. 

As "reach" goals, we would like to add additional scenes for the user to choose from or provide a space for a user to input their own scene from a movie for sentiment analysis and song matching. In addition, some sort of mechanism to overlay the user's song choice over the movie scene of their choosing (probably one of our predefined scenes) so they can see their custom soundtrack in action.

A "partially successful" project should still hold the original intent of the project intact: to generate a custom song choice for a movie scence. However, it may not have a full web-app, front-end deployment and may just run as a python script.

It is also important to note that our sentiment analysis might not provide fruitful results, thus requiring us to pivot our project objectives. Luckily, the Spotify API has many potential applications and uses that we can exploit to successfully pivot our projects focus

## Resources Required

- Access to Spotify API
- Access to movie scripts through IMDBs API

Access to Genius API (for song)

## Tools/Skills Required

We will need access to multiple web APIs-Spotify music data and movie scripts. We will need to manipulate large data sets and perform sentiment analysis to characterize the overall mood of the scene. We will also need to conduct sentiment analysis on Spotify songs in order to determine their 'mood'. As Spotify already collects song features based on their "Acousticness" and "danceability", We would use these features, along with NLP on the song lyrics, to characterize a song's mood.

We will then match the mood score of the song to the scene in the movie to determine if it is consistent. Finally, we will create a stylized webpage to display our findings.

## Risks

What are two things that could potentially stop you from achieving the full deliverable above? Maybe it turns out that the data doesn't exist and you need change plan? Or maybe your idea requires more computational power than is available to you? What particular risks might be applicable for your project?

With any machine learning pipeline, there's always the risk that whatever model we try to implement will just end up not being very effective at trying to predict what we want. In particular, we need to make sure that we have the flexibility to re-evaluate after our exploratory data analysis where we attempt to analyze sentiment of movie scripts and put that together with the Spotify songs.

We 

## Ethics

All projects we undertake involve decisions about whose interests matter; which problems are important; and which tradeoffs are considered acceptable. Take some time to reflect on the potential impacts of your product on its users and the broader world. If you can see potential biases or harms from your work, describe some of the ways in which you will work to mitigate them. Remember that even relatively simple ideas can have unexpected and impactful biases. Here's a nice introductory video for thinking about these questions, and here's one that goes into somewhat more detail. Here are some relevant examples:

Will your recipe recommender app privilege the cuisines of some cultures above others? For example, peanut butter and tomato might seem an odd combination in the context of European cuisine, but is common in many traditional dishes of the African diaspora. A similar set of questions applies to recommendation systems related to style or beauty.

What data set will your sentiment analysis be trained on? What languages will be included? Will diverse dialects be included, or only the "standard" version of the target language? Who would be excluded by such a choice, and how will you communicate about your limitations?

Will your facial recognition system work well well on all faces, or will it systematically underperform on certain marginalized subgroups? (see the videos above for examples of this.)

## Tentative Timeline

Week 2: Data acquisition and prepping pipeline

Week 4: Data analysis: Spotify Sentiment Analysis, Movie Script Sentiment Analysis. Work within a local Jupyter notebook as a proof-of-concept/exploratory data analysis. See how effective a model can be for our idea, and evaluate 

Week 6: Full pipeline set up

Week 8: How to mesh the results from the machine learning pipeline with user input in the frontend?