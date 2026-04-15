---
layout: page
title: Mathematical framework
layout: landing
description: Find out about how to measure the difference between a data cohort and a CFM in a causal inference and bayesian framework
---

<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>


<div id="main">
<section id="one">


<div class="inner">

  <header class="major">
    <h1> PSCs in a Causal Inference Framework </h1>
  </header>
  
  <p>
  Within a cohort of patients (i=1,...,N), each patient can receive one of two 
  treatment: Z &isin; (0,1). Each patient has two possible outcomes 
  Y<sub>i</sub>(0) and Y<sub>i</sub>(1)and only one outcome is 
  observed.
  Since only one possible treatment outcome is observed, each patient has 
  an individual treatment effect, and inferences are
  made as the Average Treatment Effect (ATE) across the whole population.
  
  The Conditional Average Treatment Effect (CATE) is defined as
  within a set of prognostic covariates X: <br>
  
  $$ \tau_i(x) = E[Y_i(1) - Y_i(0) \mid X = x_i] $$

  The difference between two conditional estimates is expressed as: <br>
  $$  \tau_i(x) = m_{1_i}(x) - m_{0_i}(x)  $$
  
  where: 
  $$  m_{1_i}(x) = E[Y_i(1)\mid X = x_i]  $$
  
  We assume that the potential outcomes are independent of the treatment 
  approach conditional on X, which allows us to define:
  $$  m_{1_i} = E[Y_i(1) \mid X=x_i,Z=1]  $$
  
  
  In PSCs, the observed data consists entirely of patients on some 
  experimental arm. \( m_{1_i}(x)\) is defined directly from the data.
  Counterfactual evidence for each patient is generated from a 
  parametric model to define: 
  $$ m_{0_i} =E[Y_i(0) \mid X=x_i,Z=1] = f(x_i, Z=1) $$
  where  f is some function of the data x. 
  This allows for an estimand to be defined as:
  $$  tau_i(x)= m{1_i}(x) - f(x_i, Z=1)  $$
  
  The individual treatment effect can directly estimated for each individual
  as the predicted and observed outcomes are available. The reliability of 
  these estimates depends on the strength of the assumptions made.
  
  </p>

</div>

</section>




<section id="two">


<div class="inner">

  <header class="major">
    <h1> Estimation in a Bayesian Framework </h1>
  </header>
  
  <p>
  The bayesian estimation used is about propagating uncertainty from
  the CFM into the treatment effect estimate. The bayesian approach used 
  avoids overly narrow confidence intervals.
  
  A CFM for outcomes under control with parameters \( B \) 
  (which includes baseline hazard parameters available to all patients 
  \(&Lambda;\), and \(&gamma;\) for patient covariates) is defined. <br>
  <br>
  <b>
  1) A posterior distribution is put on the CFM parameters \( B \) <br>
  </b>
  The CFM parameter uncertainty is approximated as:
  $$  B &tilde; MVN (&mu;, &Sigma;)  $$ 
  where \(&mu;\) is the vector of estimated CFM coefficients and
  \( &Sigma;\) is the CFM variance-covariance matrix <br>
  \(b \) is a single draw from this distribution. <br>
  <br>
  
  <b>
  2) An efficacy parameter (\(&beta;\) ) is defined conditional on a draw \(b\): <br>
  </b>
  $$ &Gamma;_i = &gamma;^{T}x_i + &beta; $$
  
  <b>
  3) The marginal posterior for &beta; is obtained by resampling  \(b\) <br>
  Each posterior for (\(&beta;\) ) is conditional on one CFM draw \(b\). <br>
  The marginal effects (\(&beta;\) ) is obtained by resampling from 
  \(B &tilde; MVN (&mu;, &Sigma;)\).
  </b>
  
 <ul>
  <li>The two estimation procedures:
    <ul>
      <li>Simulated RCT approach:
        <ul>
          <li>Draw \(b\)</li>
          <li>Generate random counterfactual outcomes for each treated patient from the model \( &#934; b \)</li>
          <li>For each patient, a counterfactual control observation is generated resulting in observations which can be directly compared as part of simulated RCT</li>
          <li>This is repeated across draws of \(b\)</li>
        </ul>
      </li>
      <li>Likelihood based approach:
        <ul>
          <li>Draw \(b\)</li>
          <li>Evaluate likelihood with \(&beta;\) shifting the linear predictor</li>
          <li>Estimate the posterior for \(&beta;\) using prior \(&pi;(&beta;)\)</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>
  
  </p>

</div>

</section>


</div>
