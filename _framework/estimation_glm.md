---
layout: post
title: Estimation for GLM Outcomes
description: Likelihood formulation for binary and continuous outcomes using generalised linear counterfactual models.
image: assets/images/outcomes-bin-con.jpg
---

<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<div id="main">

<section id="one">
<div class="inner">
	<header class="major">
		<h2>GLM outcomes</h2>
	</header>
	<p>
		When the CFM is a generalised linear model, outcomes from the exponential family are handled within a unified likelihood framework. For each patient \(i\) in the experimental cohort, observed outcome \(y_i\) and covariates \(\vec{x}_i\) are combined with CFM parameters \(\Lambda\) (common parameters such as intercept) and \(\gamma\) (covariate effects).
	</p>
	<p>
		The extended linear predictor includes the efficacy parameter \(\beta\):
	</p>
	<p>\[ \Gamma_i = \vec{\gamma}\vec{x}_i + \beta \]</p>
	<p>
		A link function \(G(\cdot)\) relates \(\Gamma_i\) to the scale on which data are measured. For a binomial outcome with logistic link, \(\theta_i = G^{-1}(\Gamma_i)\) and the likelihood takes the standard GLM form.
	</p>
</div>
</section>

<section id="likelihood">
<div class="inner box-round">
	<header class="major">
		<h2>Likelihood</h2>
	</header>
	<p>For exponential-family outcomes:</p>
	<p>\[ L(y_i \mid \Gamma_i) = \prod_{i=1}^{N} \exp\bigl[y_i\theta - b(\theta) - c(y_i)\bigr] \]</p>
	<p>
		For logistic regression, with \(\theta_i = \text{logit}^{-1}(\Gamma_i)\):
	</p>
	<p>\[ L(y_i \mid \Gamma_i) = \prod_{i=1}^{N} \exp\Bigl\{ y_i G^{-1}(\Gamma_i) - n \log\bigl[1 + \exp(G^{-1}(\Gamma_i))\bigr] \Bigr\} \]</p>
	<p>
		The parameter \(\beta\) measures the distance between observed experimental responses and CFM-predicted control responses — for example as a log odds ratio for binary outcomes.
	</p>
</div>
</section>

<section id="motivating">
<div class="inner box-round">
	<header class="major">
		<h2>Motivating example</h2>
	</header>
	<p>
		In a single-arm early-phase study with binary outcome, each patient's observed \(Y_i(1)\) is compared to the CFM prediction \(\psi(0 \mid W_i)\) under control. Individual contrasts \(\delta_i = Y_i(1) - \psi(0 \mid W_i)\) motivate the efficacy parameter; extending the linear predictor with \(\beta\) and accounting for CFM uncertainty via Bayesian resampling generalises this to full inference.
	</p>
	<ul class="actions">
		<li><a href="../learn/howto_glm.html" class="button special">GLM how-to guide</a></li>
		<li><a href="../learn/methods_glm.html" class="button">Methods detail</a></li>
	</ul>
</div>
</section>

</div>
