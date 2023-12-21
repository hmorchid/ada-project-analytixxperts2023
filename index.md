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

## Now let's do a first naive analysis of the data

#### What's really Diversity ?

First, to best perform analysis we will need to define how we will measure diversity. We already said that we will focus on the ethnicity and the gender of the films actors but we need a quantitative tool to treat the data well. We chose to use the Simpson Diversity Index, which is calculated by assessing the likelihood that two randomly chosen individuals from a sample will not belong to the same species. A key strength of this index is that it considers not just the variety of species present but also the relative abundance of each species. 

This means that if we compare two scenarios:

- Movie 1: 20% representation for each of 5 ethnicities.
- Movie 2: 99% representation of one ethnicity, with 100 different ethnicities comprising the remaining 1%.

We find that **D1 = 0.8** is significantly greater than **D2 = 0.02**. This result is coherent as Movie 1 appears to have a more diverse cast, even though Movie 2 includes a greater number of ethnicities.

* INSERER PIE CHARTS AVEC LA PART DES DIFFERENTS NIVEAU DE DIVERSITE ETHNIQUE ET GENDER DANS LE DATASET *

#### Diversity as a sign of progress in the film industry ?

In our modern society, the principles of diversity and inclusion have emerged as central pillars, reflecting our collective aspiration for a more equitable and representative world. This shift in values, while widely acknowledged and embraced today, marks a stark contrast to the landscape merely two decades ago, where such topics were often sidelined. This evolution of societal norms prompts us to examine various sectors, including the industry of cinema, to understand how they have adapted to these changing tides. The pertinent question we face is whether the film industry, known for its power to shape culture and perception, has mirrored this broader societal progress in embracing diversity. The accompanying graph offers a visual narrative of this journey, charting the course of diversity within the film industry over the years. 

<iframe src="assets/diversity_over_time.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

Upon examining the data, we notice a particular trend regarding gender diversity. The curve, representing the evolution of gender representation, unfortunately, does not indicate significant progress. This stagnation suggests that while conversations around gender equality have become more mainstream, the translation of these discussions into tangible change within the film industry has been limited.
On the other hand, a more hopeful narrative emerges when we consider ethnic diversity. Here, the graph depicts an upward trajectory, indicating a gradual but apparent increase in the representation of various ethnicities on screen. This trend reflects a growing acknowledgment within the industry of the importance of racial and cultural representation, and while there's still much ground to cover, it suggests a positive direction towards inclusivity.

##### Naive interpretation of The Box Offfce evolution (PAS SUR DE CA)

In our introductory segment, we established a dual framework to quantify the performance of films, encompassing both their financial success through box office earnings and their reception via average public votes. This comprehensive approach allows us to paint a more nuanced picture of a film's impact and appeal. To set the stage for our analysis, let's begin by delving into the financial aspect of this equation.
We present to you a graph that traces the trajectory of box office earnings over an extended period. This visualization serves as a foundational piece of our investigation, offering a historical perspective on the financial ebbs and flows of the film industry.

INSEREZ BOX OFFICE OVER TIME 

Upon inspecting the graph, we're immediately struck by a clear and undeniable trend: the box office earnings have undergone a significant evolution over time. This growth curve may be influenced by a multitude of factors, from inflation and market expansion to the increasing global reach of cinematic works. However, what captures our interest is the parallel upward trend in ethnic diversity within films, a topic we've previously touched upon.
This observed synchrony between the rise in box office earnings and the increase in ethnic diversity leads us to a compelling line of inquiry: might there be a correlation between these two variables? The possibility that a more diverse cast could resonate with a broader audience and thereby enhance box office performance is an intriguing hypothesis.
To probe this relationship further, we must venture beyond mere visual comparison and engage in a statistical examination. By employing correlation analysis, we aim to uncover any statistical significance that might exist between the growing diversity in film and the ascending box office earnings. This method will allow us to understand not just the existence but also the strength of any potential correlation, providing us with a more grounded understanding of the interplay between these two facets of the cinematic world.

#### What do the statistics say?

We've been looking into whether there's a link between the variety of ethnic backgrounds in a movie's cast and how much money the movie makes. To do this, we first checked out the movie's box office receipts, which tell us how well it did financially.

We did some math and found a Pearson correlation of about 0.217 between the ethnic mix of a movie's cast and the money it made at the box office. This positive link is important because it's strong enough (the p-value is less than 0.05) to suggest that movies tend to earn more when they have a more ethnically diverse cast.

To dig deeper into how the ethnic mix of the cast affects a movie's earnings, we're going to do a regression analysis next. This will help us see just how much of an impact diversity has on the money movies make and get a clearer picture of how these two things are connected.

Our findings do show a real link between a film’s cast ethnic diversity and its box office success. But it's important to remember that the coefficient of determination (R²) is pretty low. This means that while ethnic diversity is part of the story, it doesn't tell us everything about why some movies make more money than others. There are likely other factors at play too.

To make this easier to understand, we'll create a regression graph. This graph will show us a visual story of the link between cast diversity and earnings. It'll have a bunch of dots showing individual movies and a line that shows the general trend. This line's upward slope means that in general, more diversity in the cast is associated with higher box office revenue. But remember, this graph just shows a connection, not that one thing directly causes the other. So, while it's clear that there's a link between diversity and earnings, we'd need to look even closer to say for sure that more diversity is what's making movies earn more.

<iframe src="assets/diversity_ethnicity_corr_boxoffice.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

We also took a look at gender diversity in movie casts to see if it has anything to do with how much money the movies make. We found that there's basically no straight-line relationship between the two. Having a more balanced mix of genders in the cast doesn't seem to have a clear link with the movie's financial success.
Next, we're going to do a regression analysis to confirm what we found. After doing this deeper dive, the results tell us that gender diversity isn't really predicting how well a movie does at the box office. It looks like the model we used to test this isn't a great fit for the data, either. This suggests that there are probably other things, maybe like the ethnic diversity we talked about before, that are better at explaining why some movies earn more than others.

To make this clearer, we'll create a regression graph like we did for the ethnic diversity.
After looking at the scatter plot, it's clear that the numbers back up what we found in our analysis: the mix of genders in a movie's cast doesn't really have a noticeable link with how much money the movie makes. So, while gender diversity is important for many reasons, it doesn't seem to have a big impact on a movie's box office revenue based on this data.

<iframe src="assets/gender_corr_boxoffice.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

Ethnic Diversity compared to ratings :

<iframe src="assets/diversity_ethnicity_corr_rating.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

Gender Diversity compared to ratings :

<iframe src="assets/gender_corr_rating.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

<iframe src="assets/ethnicity_boxoffice_timeperiods.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>

<iframe src="assets/gender_boxoffice_timeperiods.html" width="750px" height="500px" frameborder="0" position="relative">Genre plot</iframe>
