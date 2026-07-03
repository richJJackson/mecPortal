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
				<p> The premis for Personalised Synthetic Controls is that a model can be used 
  				to estimate a patient's outcome and that this estimate can be compared 
  				against their observed outcome.
  				
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
  			    <p>
              For patient <i>i</i>, let <i>Y<sub>i</sub><sup>(1)</sup></i>
              be the actual observed treated outcome and 
              <i>Y<sub>i</sub><sup>(0)</sup></i> be the predicted counterfactual
              outcome. The individual effect (&tau;<sub>i</sub>) is:
            </p>
            
            <p>
              <b>&tau;<sub>i</sub> = Y<sub>i</sub><sup>(1)</sup> - Y<sub>i</sub><sup>(0)</sup></b>
            </p>
            
            
            <p>
              To estimate the average treatment effect (ATE) over a group of patients (n),
              we can average over all individual effects:
              <b>ATE = (1/n) &sum; &tau;<sub>i</sub></b>.
            </p>
  				
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
			<p> Use the model to directly simulate 'synthetic' outcomes for treated patients. For each 
			observed patient we can then use basic analytical methods to compare the 
			observed and the expected counterfactual outcomes.


			</p>
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
			difference between the counterfactual model and the new cohort of 
			observations </p>
		</div>
	</div>
</section>







<!-- Two -->
<div class="collapsible-section">
<div class="section-header">
<h2> Further Details </h2> 
</div>

<!-- LINKS -->
<div class="section-content">
<section id="links" class="spotlights">
  <div class="inner">
      <header class="major">
  	    <h2>
        <a href="../learn/methods_glm.html"> MECs for Binary/Continuous Outcomes </a>
        </h2>
      </header>
	    <p>Understand how Model Estimated Controls work with MEC based on Generalised Linear Models </p>
  </div>
  
  <div class="inner">
      <header class="major">
  	    <h2>
        <a href="../learn/methods_surv.html"> MECs for Survival Outcomes </a>
        </h2>
      </header>
	    <p> Understand how Model Estimated Controls work with MEC based on Parametric Survival Models </p>
  </div>
  
  <div class="inner">
      <header class="major">
  	    <h2>
        <a href="../learn/methods_surv.html"> Bayesian Estimation of MECs </a>
        </h2>
      </header>
	    <p> Get more details on the Bayesian estimation procedures along with MCMC algorithms </p>
  </div>
    
</section>
</div>



</section>