---
layout: post
title: Estimation for Survival Outcomes
description: Likelihood formulation and Bayesian estimation when PSCs use parametric survival counterfactual models.
image: assets/images/survival.jpg
---

<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<div id="main">

<section id="one">
<div class="inner">
	<header class="major">
		<h2>Survival outcomes</h2>
	</header>
	<p>
		When the outcome is time-to-event, the data cohort provides an event time \(t_i\) and censoring indicator \(c_i\) for each patient, together with covariates \(\vec{x}_i\) aligned with the counterfactual model (CFM).
	</p>
	<p>
		For a fully parametric CFM, baseline hazard parameters \(\Lambda\) (e.g. spline coefficients for a flexible parametric model) and covariate effects \(\gamma\) define the control-arm prediction. The efficacy parameter \(\beta\) enters as a <strong>log hazard ratio</strong>, extending the linear predictor:
	</p>
	<p>\[ \Gamma_i = \vec{\gamma}\vec{x}_i + \beta \]</p>
	<p>
		From \(\Lambda\) and \(\Gamma_i\), cumulative hazard \(H(t_i \mid \Lambda, \Gamma_i)\) and hazard \(h(t_i \mid \Lambda, \Gamma_i)\) are obtained. Survival and density follow as \(S(t_i) = \exp\{-H(t_i)\}\) and \(f(t_i) = -S(t_i)\,h(t_i)\).
	</p>
</div>
</section>

<section id="likelihood">
<div class="inner box-round">
	<header class="major">
		<h2>Likelihood</h2>
	</header>
	<p>The contribution for patient \(i\) is:</p>
	<p>\[ L(D \mid \Lambda, \Gamma_i) = \prod_{i=1}^{N} f(t_i \mid \Lambda, \Gamma_i)^{c_i}\, S(t_i \mid \Lambda, \Gamma_i)^{(1-c_i)} \]</p>
	<p>
		This compares the observed survival of the experimental cohort against CFM-implied control survival, with \(\beta\) measuring the distance between them. Flexible parametric models (e.g. Royston–Parmar splines) are commonly used for the baseline hazard.
	</p>
</div>
</section>

<section id="bayesian">
<div class="inner box-round">
	<header class="major">
		<h2>Bayesian estimation</h2>
	</header>
	<p>
		CFM parameters are not fixed: draw \(b \sim \pi(B)\) from the model posterior (typically multivariate normal), then estimate \(\beta\) conditional on each draw. Two approaches are used:
	</p>
	<ul>
		<li><strong>Simulated RCT</strong> — simulate counterfactual control outcomes from \(\Phi(b)\) for each patient and compare arms directly.</li>
		<li><strong>Likelihood / MCMC</strong> — define \(P(\beta \mid b, D) \propto L(D \mid \gamma_i, \beta)\,\pi(\beta)\) and resample over \(b\) to obtain marginal inference for \(\beta\).</li>
	</ul>
	<p>
		Resampling propagates uncertainty from the CFM into the treatment-effect estimate. Ignoring CFM uncertainty produces confidence intervals with poor coverage.
	</p>
	<ul class="actions">
		<li><a href="../learn/howto_surv.html" class="button special">Survival how-to guide</a></li>
		<li><a href="../learn/methods_surv.html" class="button">Methods detail</a></li>
	</ul>
</div>
</section>

</div>
