---
title: Getting started
order: 2
layout: landing
description: When and how should PSCs be used?
image: assets/images/blackboard.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>When Should PSCs be used?</h1>
		</header>
		
		<div class="box-round">
		  <header class="minor">
		  <h2> Estimating Treatment Effects </h2>
		  </header>
		  
		  
		    
		    <div class="box-round">
		      <h3> Randomised Controlled Trials (RCTs) </h3>
		      <p>
	          PSCs can be used to essentially produce the same information
	          that a RCT produces (to estimate treatment efficacy). 
	          The downside of RCTs is that they are costly, time consuming and 
	          require large numbers of patients. 
	          
	          <br>
	          When only data from an experimental arm are available, PSCs
	          can act as a control group to be compared against the performance of the 
	          experimental group. This allows for the comparison of the two treatment 
	          groups (as is done in a RCT).
	          
	          <div>
    
              <span class="image fit"><img src="{% link assets/images/illustration-psc-comp.png %}" alt="" /></span>
            </div>
		      </p>
		    </div>
		    
		    
		    <div class="box-round">
		      <h3> Observational Data </h3>
		      The PSC methodology is also useful for estimating treatment effects 
		      using observational data on experimental treatments
		    </div>
		    
		  </div>
		  
		  
		  <div class="box-round">
		  <header class="minor">
		  <h2> Designing Clinical Trials Using Personalised Synthetic Controls </h2>
		  </header>
		  
		  
		  <div class="box-round">
		  In the design of a single-arm clinical trial, the PSC model can act as 
		  the external control arm:
		  
		  
		    <div>
          <span class="image fit"><img src="{% link assets/images/exp_trial.jpg %}" alt="" /></span>
        </div>
		  
		  This supports efficiency because fewer randomised control patients
		  can be used while still achieving a structured comparison that accounts for 
		  uncertainty in the PSC. This allows for choosing an experimental 
		  sample size that achieves an efficient clinical trial.

		  </div>
		  
		</div>
		
	
</section>
</div>

<!-- Two -->
<section id="two" class="grid-cards">



	<section>
		<a href="learn/methods_land.html" class="image">
			<img src="{% link assets/images/model-of-city.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Methods </h3>
				</header>
				<p>Get Details on Personalised Synthetic Controls.  Learn how they are developed and how they work, including likelihood definitions and Bayesian Estimation procedures</p>
				<ul class="actions">
					<li><a href="learn/methods_land.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	
	<section>
		<a href="learn/software_land.html" class="image">
			<img src="{% link assets/images/code.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Software </h3>
				</header>
				<p> Explore the packages developed to use Personalised Synthetic Controls and learn how they are used</p>
				<ul class="actions">
					<li><a href="learn/software_land.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	
	<section>
		<a href="learn/howto_land.html" class="image">
			<img src="{% link assets/images/maze.jpg %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> How To... </h3>
				</header>
				<p> Details and user guides on how to use Synthetic Controls in practice </p>
				<ul class="actions">
					<li><a href="learn/howto_land.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>

	<section>
		<a href="learn/causal_land.html" class="image">
			<img src="{% link assets/images/domino-white.jpg %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Causal Inference </h3>
				</header>
				<p> Personalised Synthetic Controls can be a tools for causal inference - find out what makes them causal and what assumptions are required!</p>
				<ul class="actions">
					<li><a href="learn/causal_land.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	
</section>


<!-- Three -->
<section id="three">
	<div class="inner">
		<header class="major">
			<h2>Contact</h2>
		</header>
		<p>  Have you used Personalised Synthetic Controls in your research? </p>
		<ul class="actions">
			<li><a href="generic.html" class="button next">Get Started</a></li>
		</ul>
	</div>
</section>

</div>
