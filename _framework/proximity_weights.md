---
layout: post
title: PSCs and Proximity Weights
description: Further development — weighting patient contributions by proximity to the counterfactual model support.
image: assets/images/flowchart.jpg
---

<div id="main">

<section id="one">
<div class="inner">
	<header class="major">
		<h2>Proximity weights</h2>
	</header>
	<p>
		An area of ongoing development is the use of <strong>proximity weights</strong> when applying PSCs — down-weighting (or excluding) patients whose covariate profiles lie far from the region in which the counterfactual model was developed or validated.
	</p>
	<p>
		This relates closely to assumptions of <strong>overlap</strong> and <strong>transportability</strong>: patients should have non-zero probability of receiving control, and the CFM should be applicable to the comparison cohort without extrapolation beyond supported covariate ranges.
	</p>
</div>
</section>

<section id="development">
<div class="inner box-round">
	<header class="major">
		<h2>Further development</h2>
	</header>
	<p><em>Template — describe the proximity-weighting scheme, estimation procedure, and planned validation (simulation and case studies).</em></p>
	<ul>
		<li>Definition of proximity metric relative to CFM training data.</li>
		<li>Integration with Bayesian PSC estimation.</li>
		<li>Diagnostics for extrapolation and effective sample size.</li>
		<li>Comparison with unweighted PSC estimates.</li>
	</ul>
</div>
</section>

<section id="links">
<div class="inner">
	<ul class="actions">
		<li><a href="../methodology.html#assumptions" class="button">PSC assumptions</a></li>
		<li><a href="../learn/causal_psc.html" class="button">Causal inference framework</a></li>
	</ul>
</div>
</section>

</div>
