---
title: The PSC framework
order: 1
layout: landing
description: What are Personalised Synthetic Controls and how do they work?
image: assets/images/blackboard.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	
	<div class="inner">
		<header class="major">
			<h1>What are Personalised Synthetic Controls?</h1>
		</header>
		<p> Personalised synthetic controls (PSCs) are statistical models that can be used 
		to assess the efficacy of new therapies without needing to use clinical trials.
    </p>
    <p>
    PSCs can act as counterfactual evidence (a way to predict ‘what if?’)- 
    i.e., how would patients respond if they had received a different treatment?
    </p>
	</div>

	<div class="inner">
	
		<header class="major">
			<h1>How do PSCs differ to classical synthetic controls? </h1>
		</header>
		<p> 
		The only similarity of PSCs with classical synthetic
			controls is tht the counterfactual evidence is synthetically generated
			in both concepts, however there are more differences between the two as 
			shown in the table below:
    </p>
        
      <div class="table-wrapper">
    <table>
     <thead>
      <tr>
       <th style="text-align:left;">  Feature </th>
       <th style="text-align:center;"> Personalised Synthetic Controls </th>
       <th style="text-align:center;"> Classical Synthetic Controls </th>
      </tr>
     </thead>
    <tbody>
      <tr>
       <td 
       style="text-align:left;"> Compares the observed response of 
       an experimental group against a counterfactually <br>
       constructed response of the control group
       </td>
       <td style="text-align:center;">&#10003;  </td>
       <td style="text-align:center;">  &#10003;</td>
      </tr>
      <tr>
      <td style="text-align:left;">Can make a comparison 
      on individual patient level <br> (personalised treatment comparison)</td>
      <td style="text-align:center;">&#10003;  </td>
       <td style="text-align:center;">&#10007;</td>
      </tr>
      <td style="text-align:left;"> How counterfactual evidence is generated </td>
      <td style="text-align:center;"> Predicted from the counterfactual model </td>
      <td style="text-align:center;"> The weighted average of controls</td>
      <tr>
      <td style="text-align:left;"> Treatment effect</td>
      <td style="text-align:center;">Difference between the observed experimental response and 
      the model estimated response</td>
      <td style="text-align:center;">Difference between the observed 
      experimental response and the weighted combination
      of controls</td>
      </tr>
    </tbody>
    </table>
    </div>

    <header class="major">
    <h3> Assumptions of PSCs: </h3>
    </header>
    
    <li>the parameters of the counterfactual model (CFM)
    are common to all patients (e.g., model intercept), and the data cohort contain outcome 
    data and CFM covariates are present in the data cohort </li>
    
    <li>Strong ignorability- the potential outcomes are independent
    of the treatment approach conditional on the observed covariates. </li>
    
    <li> There are no unmeasured confounders (i.e., there are no 
    unaccounted variables that affect the outcome). </li>
    
    <li> Stable Unit Treatment Variability Assumption - a patients's potential outcome is not affected by 
    the setting in which it was observed</li>
    
    <li> The model is correctly specified and the posterior distribution
    of the model can be approximated by a multivariable normal distribution</li>
    
    <li> Transportability - first the results of the CFM should be applied
    to the setting in which the data cohort were collected </li>
    
    <li> overlap- for each patient who received the experimental treatment,
    there exists some non-zero probability that they may have received the control treatment </li>
    
  </div>

  <div class="inner">
  	<header class="major">
  		<h1> When should PSCs be used? </h1>
  	</header>
  	<p> 
  	
    </p>
  </div>
   
</section>


<div class="inner">



  <div id="two" class="grid-cards">
		<a href="framework/concept_estimation.html" class="image">
			<img src="{% link assets/images/paper.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Concept and Estimation </h3>
				</header>
				<p>Learn more about the concept behind model estimated controls, including
				likelihood definitions and Bayesian Estimation procedures</p>
				<ul class="actions">
					<li><a href="framework/concept_estimation.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</div>
	
	
	<div id="two" class="grid-cards">
		<a href="framework/concept_estimation.html" class="image">
			<img src="{% link assets/images/math_board.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Mathematical Framework </h3>
				</header>
				<p>Learn more about the mathematical framework of PSCs </p>
				<ul class="actions">
					<li><a href="framework/mathematical_fwk.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</div>
	
	
		<div id="two" class="grid-cards">
		<a href="framework/concept_estimation.html" class="image">
			<img src="{% link assets/images/paper.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> Manuscript and publications </h3>
				</header>
				<p>Access the published manuscript about Personalised Synthetic Controls </p>
				<ul class="actions">
					<li><a href="https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-025-02540-2" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</div>
	
	
	
</div>

</div>




	
