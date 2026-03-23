---
layout: post
title:  "Personalised Synthetic Controls - Conception and Estimation"
date: 2025-03-12
description: How do Personalised Synthetic Controls work?
image: 
---















<section id="concept" class="spotlights">


  <section class="image">
	  <img src="{% link assets/images/methods_land_fig1.png %}" alt="" data-position="center center" />
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Models as the base for counter-factual evidence </h3>
				</header>
				<p> The premis for Model Estimated Control is that a model can be used 
  				to estimate a patient's outcome and that this estimate can be compared 
  				against their observed outcome
  			</p>
			</div>
		</div>
	</section>
  

  <section>
  		<a class="image">
  			<img src="{% link assets/images/methods_land_fig2.png %}" alt="" data-position="top center" />
  		</a>
  		<div class="content">
  			<div class="inner">
  				<header class="major">
  					<h3> Average Treatment Effects obtained by averaging across individual effect </h3>
  				</header>
  				<p> To estimate the average treatment effect over a group of patients, we can average over all individual effects. </p>
  			</div>
  		</div>
  </section>

</section>





<section id="Estimation" class="spotlights">


  <h2> Estimation </h2> 

    <h5> Two procedures exist for estimating treatment effects using MEC - a simulation and a likelihood approach </h5>

<section>
	<a class="image">
		<img src="{% link assets/images/methods_land_fig3.png %}" alt="" data-position="center center" />
	</a>
	<div class="content">
		<div class="inner">
			<header class="major">
				<h3> Simulation </h3>
			</header>
			<p> Use the model to directly simulate 'synthetic' patients. For each 
			observed patient we can then use basic analytical methods to compare the 
			observed and the expected outcomes </p>
		</div>
	</div>
</section>

<section>
	<a class="image">
		<img src="{% link assets/images/methods_land_fig4.png %}" alt="" data-position="top center" />
	</a>
	<div class="content">
		<div class="inner">
			<header class="major">
				<h3> Likelihood based approach </h3>
			</header>
			<p> Define a likelihood where a term is added to measure the direct 
			difference between the counter factual model and the new cohort of 
			observations </p>
		</div>
	</div>
</section>


</section>