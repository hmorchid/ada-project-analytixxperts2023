---
layout: page
title: Diversity in Cinema
subtitle: The Influence of Diversity on Role Dynamics and Film Performance
cover-img: /assets/img/red-movie-theater-seats-with-curtains-background_1017-38388.jpg
thumbnail-img: /assets/img/red-movie-theater-seats-with-curtains-background_1017-38388.jpg
share-img: /assets/img/red-movie-theater-seats-with-curtains-background_1017-38388.jpg
use-site-title: true
---

The topic of diversity is gaining increasing attention nowadays. Many studies, like [this McKinsey & Company report](https://www.mckinsey.com/capabilities/people-and-organizational-performance/our-insights/why-diversity-matters), affirms that diversity is not just a buzzword but a pivotal aspect of business success. We would like to assess whether this phenomenon is also applicable to the movie industry.
Consider the groundbreaking success of movies like Black Panther and Barbie. These films not only shattered box office records but also marked a significant cultural moment by celebrating diversity in ethnicity and gender, respectively. Their success prompts a deeper reflexion: Is there a tangible link between a film's performance, i.e its box office earnings and public ratings, and its cast's diversity ?

## Introduction
Join us on this cinematic journey as we unravel the data story behind diversity in films. We will dissect this relationship by analyzing a variety of films across genres, from blockbuster hits to indie gems, our research will shed light on whether films with diverse casts resonate more profoundly with audiences and critics alike. 

By navigating in the data we will uncover the patterns, understand the impacts, and discover whether the movies we love are a reflection of the diverse world we live in. Are diverse casts just a trend, or are they a key ingredient to a film's success and legacy? Let the data respond !

## Let's take a first look to the Data

#### What's really Diversity ?

First, to best perform analysis we will need to define how we will measure diversity. We already said that we will focus on the ethnicity and the gender of the films actors but we need a quantitative tool to treat the data well. We chose to use the Simpson Diversity Index, which is calculated by assessing the likelihood that two randomly chosen individuals from a sample will not belong to the same species. A key strength of this index is that it considers not just the variety of species present but also the relative abundance of each species. 

This means that if we compare two scenarios:

- Movie 1: 20% representation for each of 5 ethnicities.
- Movie 2: 99% representation of one ethnicity, with 100 different ethnicities comprising the remaining 1%.

We find that **D1 = 0.8** is significantly greater than **D2 = 0.02**. This result is coherent as Movie 1 appears to have a more diverse cast, even though Movie 2 includes a greater number of ethnicities.

##### Diversity as a sign of progress in the film industry ?

While we can all agree that diversity and inclusion in the broadest sense of the term have become a key issue in today's society, this was not the case even twenty years ago. The question is whether this progress can also be observed in the film industry, and the following graph shows how diversity has evolved over the years in the film industry.

<iframe src="assets/diversity_over_time.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

Well, the curve for gender diversity doesn't really show any evolution over time. There is, however, an upward trend in ethnic diversity. 

##### Naive analysis of the correlation between Diversity and Performance

As it been said in the introduction we will define performance by two componenets, the bof office earnings and the average public vote.
To give you an initial comparison, here's a graph showing the evolution of box office earnings over time.

INSEREZ BOX OFFICE OVER TIME (INFLATION?)

We observe a net evolution of the box office earnings over time. Since ethnic diversity also has an upward trend, can we conclude that the two are correlated? Let's see if we can simply determine their correlation statistically. 
The following graph shows the relationship between correlation and ethnic diversity :

<iframe src="assets/diversity_ethnicity_corr_boxoffice.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

The chart provides a visual representation that complements statistical findings that indicate ethnic diversity is a significant predictor of box office revenue.
Gender diversity compared to box office revenue :

<iframe src="assets/gender_corr_boxoffice.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

Ethnic Diversity compared to ratings :

<iframe src="assets/diversity_ethnicity_corr_rating.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

Gender Diversity compared to ratings :

<iframe src="assets/gender_corr_rating.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>



