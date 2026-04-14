---
layout: post
title:  "How To Use Peronaslised Synthetic Controls"
date: 2025-03-12
categories: [methods]
description: How do Personalised Synthetic Controls work?
image: assets/images/how.jpg
---

<section id="one">

<div class="box-round">

  <header class="major">
    <h2> Typical user workflow </h2>
  </header>
  
  <p>
  <b>Below is a simple step-by-step guide to applying PSCs:</b><br>
  </p>
  <div class="row uniform 50%" style="text-align: center;">
    <div class="6u 12u$(medium)" style="display: inline-block; float: none;">
    
      <div class="box-round" style="background-color: #f7f8fa;">
      <b>Define treated unit(s)</b> <br>
        Treated dataset should have baseline covariates and
        observed outcomes.
     
      </div>
      
    </div>
  </div>
  
  <div style="text-align: center;">
  <span style="font-weight:1000; font-size:1.8em;">&darr;</span>
  </div>
  
  
  <div class="row uniform 50%" style="text-align: center;">
    <div class="8u 12u$(medium)" style="display: inline-block; float: none;">
    
      <div class="box-round" style="background-color:#f7faf8;">
      <b>Define donor pool</b> <br>
          Choose where the control comes from: <br>
          A dataset: historical trial arm/registry that 
          can be used to build a CFM, or <br>
          An existing validated CFM
      </div>
    
    </div>
  </div>
  
  <div style="text-align: center;">
  <span style="font-weight:1000; font-size:1.8em;">&darr;</span>
  </div>
  
  
    <div class="row uniform 50%" style="text-align: center;">
    <div class="6u 12u$(medium)" style="display: inline-block; float: none;">
    
      <div class="box-round" style="background-color: #f7f8fa;">
      <b>Select covariates</b> <br>
        Select all covariates that were used to build the CFM
  
      </div>
    
    </div>
  </div>
  
  
  <div style="text-align: center;">
  <span style="font-weight:1000; font-size:1.8em;">&darr;</span>
  </div>
  
  
    <div class="row uniform 50%" style="text-align: center;">
    <div class="6u 12u$(medium)" style="display: inline-block; float: none;">
    
      <div class="box-round" style="background-color: #f7faf8;">
      <b> Choose personalisation parameters</b> <br>
         
          Decide how individual predictions are made:

      </div>
    
    </div>
  </div>
  
  
  <div style="text-align: center;">
  <span style="font-weight:1000; font-size:1.8em;">&darr;</span>
  </div>
  
    
  
    <div class="row uniform 50%" style="text-align: center;">
    <div class="8u 12u$(medium)" style="display: inline-block; float: none;">
    
      <div class="box-round" style="background-color: #f7f8fa;">
      <b>Run estimation</b> <br>
          
      Apply the CFM to the extract the predicted outcome for each treated patient.
      Estimate effect by chosen estimand <br>
      Propagate uncertainty by repeating over model-parameter draws and aggregating.

      </div>
    
    </div>
  </div>
  
  
  
    <div style="text-align: center;">
  <span style="font-weight:1000; font-size:1.8em;">&darr;</span>
  </div>
  
  
    <div class="row uniform 50%" style="text-align: center;">
    <div class="8u 12u$(medium)" style="display: inline-block; float: none;">
    
      <div class="box-round" style="background-color: #f7faf8;">
      <b>View diagnostics</b> <br>
      
      Assess model performance- calibration/discrimination <br>
      Influence: which patients drive the estimate <br>
      Stability: sensitivity to covariate set <br>
      Assumptions: document unmeasured confounding risks and do sensitivity analysis<br>
 
      </div>
    
    </div>
  </div>
  
  

  

  

  

</div>

</section>



<b>Details on Model Estimated Controls as a tool for Causal Inference</b> <br>


<!-- Two -->
<section id="two" class="flex-cards">

  	<section>
		<a href="howto_formatData.html" class="image">
			<img src="{% link assets/images/format-data.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Format Data for PSCs </h3>
				</header>
				<p> Learn how to format your data when using Model Estimated Controls </p>
				<ul class="actions">
					<li><a href="howto_formatData.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	
	<section>
		<a href="howto_surv.html" class="image">
			<img src="{% link assets/images/survival-outcomes.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> PSCs for Survival Outcomes </h3>
				</header>
				<p> Learn how to use Model Estimated Controls when you have a survival outcome </p>
				<ul class="actions">
					<li><a href="howto_surv.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	
	<section>
		<a href="howto_glm.html" class="image">
			<img src="{% link assets/images/outcomes-bin-con.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> PSCs for Binary/Continuous Outcomes </h3>
				</header>
				<p> Learn how to use Model Estimated Controls when you have a binary/continuous outcome </p>
				<ul class="actions">
					<li><a href="howto_glm.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	

</section>
