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

## Let's dive into the Data

First, to best perform analysis we will need to define how we will measure diversity. We already said that we will focus on the ethnicity and the gender of the films actors but we need a quantitative tool to treat the data well. We chose to use the Simpson Diversity Index, which is calculated by assessing the likelihood that two randomly chosen individuals from a sample will not belong to the same species. A key strength of this index is that it considers not just the variety of species present but also the relative abundance of each species. 

This means that if we compare two scenarios:

- Movie 1: 20% representation for each of 5 ethnicities.
- Movie 2: 99% representation of one ethnicity, with 100 different ethnicities comprising the remaining 1%.

We find that **D1 = 0.8** is significantly greater than **D2 = 0.02**. This result is coherent as Movie 1 appears to have a more diverse cast, even though Movie 2 includes a greater number of ethnicities.
