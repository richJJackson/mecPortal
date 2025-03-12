---
layout: post
title:  "A (possible) solution."
date: 2025-03-12
categories: [introduction]
description: How to cope with a modelled control treatment??
image: assets/images/post_solution.png
---

For a long time out solution was to do nothing.  After all we had plenty to do 
and a problem without a solution was, well, inconvenient.  Especially with an 
inspection on the horizon.

But you do keep coming back to these things.  It was the model that was most 
interesting and the fact that we couldn't deny that it was a good model.  Not 
only based on good data but validated in a real world setting and with a 
reasonable degree of precision.

Furthermore, it was a model created for prediction.  This model was meant to 
predict patients outcomes.  It only seemed reasonable to use it for just this 
purpose.

So we did. Alot. For every patient in fact.

This was reasonably straight forward, we had the baseline hazard parameters which 
allowed us to estimate a survival function.  For each patient we could then use 
the parameters from the model to create a linear predictor for each patient in 
our dataset.  

Three exampels are below:

<span class="image fit"><img src="{% link assets/images/post_solution.png %}" alt="" /></span>

Our first impression what that the model estimates themselves had a large amount 
of variability with median survival ranging from around 3 months to beyond 20 
months.  This was then a heterogensous population.  

The second point was that, more often than not the observed time was beyond the 
median.  

We did think briefly around some form of sign-rank test based on the ability of 
patietns to out-live the median but what we would do with censored patients 
wasn't clear.  Also, it felt a bit of a *blunt* approach.

We would have to keep thinking.  But we had made a start, and that felt like something.



