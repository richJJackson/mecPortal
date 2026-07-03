---
title: Methodology
banner_title: The Ideas Behind PSCs
order: 1
layout: landing
description: Concepts, assumptions, and causal foundations — plus the guides to understand them.
image: assets/images/mathematical.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<section id="one">
	<div class="inner">
		<header class="major">
			<h2>What Are Personalised Synthetic Controls?</h2>
		</header>
		<p>Personalised synthetic controls (PSCs) are statistical models used to assess treatment efficacy when a conventional control arm is unavailable or impractical.</p>
		<p>They generate counterfactual evidence — answering <em>what would have happened if this patient had received standard care?</em> — by predicting individual outcomes from a validated counterfactual model.</p>
	</div>

	<div class="inner">
		<header class="major">
			<h2>How PSCs Differ From Classical Synthetic Controls</h2>
		</header>
		<p>The only similarity is that counterfactual evidence is synthetically generated in both approaches. The differences matter for interpretation:</p>

		<div class="table-wrapper">
			<table>
				<thead>
					<tr>
						<th style="text-align:left;">Feature</th>
						<th style="text-align:center;">Personalised Synthetic Controls</th>
						<th style="text-align:center;">Classical Synthetic Controls</th>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td style="text-align:left;">Compares observed experimental response against a counterfactually constructed control response</td>
						<td style="text-align:center;">&#10003;</td>
						<td style="text-align:center;">&#10003;</td>
					</tr>
					<tr>
						<td style="text-align:left;">Patient-level (personalised) treatment comparison</td>
						<td style="text-align:center;">&#10003;</td>
						<td style="text-align:center;">&#10007;</td>
					</tr>
					<tr>
						<td style="text-align:left;">How counterfactual evidence is generated</td>
						<td style="text-align:center;">Predicted from the counterfactual model</td>
						<td style="text-align:center;">Weighted average of donor units</td>
					</tr>
					<tr>
						<td style="text-align:left;">Treatment effect</td>
						<td style="text-align:center;">Observed response minus model-estimated response</td>
						<td style="text-align:center;">Observed response minus weighted combination of controls</td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>

	<div class="inner">
		<header class="major">
			<h3 id="assumptions">Assumptions of PSCs</h3>
		</header>
		<ul>
			<li>Counterfactual model parameters are shared across patients, and the data cohort contains the outcome and covariates required by the model.</li>
			<li>Strong ignorability — potential outcomes are independent of treatment given observed covariates.</li>
			<li>No unmeasured confounders affect the outcome.</li>
			<li>Stable unit treatment value assumption — a patient's potential outcome is not affected by how or where treatment was observed.</li>
			<li>The model is correctly specified and its posterior can be approximated by a multivariate normal distribution.</li>
			<li>Transportability — CFM results apply to the setting in which the comparison cohort was collected.</li>
			<li>Overlap — each treated patient had non-zero probability of receiving control.</li>
		</ul>
	</div>

	<div class="inner">
		<header class="major">
			<h2>Limitations</h2>
		</header>
		<p>PSCs rely on the <a href="#assumptions">assumptions above</a>. When these are not met, treatment-effect estimates may be biased. Sensitivity analysis and diagnostic review are essential before drawing conclusions.</p>
	</div>
</section>

<section id="estimation">
	{% include section_header.html title="Estimation by Outcome Type" lead="How the PSC likelihood and Bayesian procedures differ for survival and GLM endpoints." %}

	<div class="inner grid-cards">
		<a href="framework/estimation_survival.html" class="image">
			<img src="{% link assets/images/survival-outcomes.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Survival Outcomes</h3>
				</header>
				<p>Parametric survival CFMs, log hazard ratio efficacy, censoring, and MCMC estimation with uncertainty propagation.</p>
				<ul class="actions">
					<li><a href="framework/estimation_survival.html" class="button">Read more</a></li>
				</ul>
			</div>
		</div>
	</div>

	<div class="inner grid-cards">
		<a href="framework/estimation_glm.html" class="image">
			<img src="{% link assets/images/outcomes-bin-con.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Binary &amp; Continuous Outcomes (GLM)</h3>
				</header>
				<p>Exponential-family likelihoods, link functions, and efficacy parameters for non-survival endpoints.</p>
				<ul class="actions">
					<li><a href="framework/estimation_glm.html" class="button">Read more</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<section id="further-development">
	{% include section_header.html title="Further Development" lead="Ongoing methodological work extending PSCs to trial design and weighted estimation." %}

	<div class="inner flex-cards">
		<section>
			<a href="framework/psc_trial_design.html" class="image">
				<img src="{% link assets/images/exp_trial.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>PSCs for Trial Design</h3>
					</header>
					<p>Using counterfactual models as external controls in single-arm and hybrid trial design with <code>pscDesign</code>.</p>
					<ul class="actions">
						<li><a href="framework/psc_trial_design.html" class="button">Read more</a></li>
					</ul>
				</div>
			</div>
		</section>

		<section>
			<a href="framework/proximity_weights.html" class="image">
				<img src="{% link assets/images/flowchart.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>PSCs and Proximity Weights</h3>
					</header>
					<p>Weighting patient contributions by proximity to the CFM support — addressing overlap and transportability.</p>
					<ul class="actions">
						<li><a href="framework/proximity_weights.html" class="button">Read more</a></li>
					</ul>
				</div>
			</div>
		</section>
	</div>
</section>

<section id="foundations">
	{% include section_header.html title="Statistical Foundations" lead="Go deeper into estimation, causal inference, and the mathematics behind PSCs." %}

	<div class="inner grid-cards">
		<section>
			<a href="learn/methods_land.html" class="image">
				<img src="{% link assets/images/math_board.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Methods</h3>
					</header>
					<p>Likelihood definitions, Bayesian estimation, and how counterfactual models are built.</p>
					<ul class="actions">
						<li><a href="learn/methods_land.html" class="button">Explore methods</a></li>
					</ul>
				</div>
			</div>
		</section>

		<section>
			<a href="learn/causal_land.html" class="image">
				<img src="{% link assets/images/concept-estim.jpg %}" alt="" data-position="25% 25%" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Causal Inference</h3>
					</header>
					<p>What makes PSCs a causal tool, how they relate to RCTs, and how they compare to other approaches.</p>
					<ul class="actions">
						<li><a href="learn/causal_land.html" class="button">Explore causality</a></li>
					</ul>
				</div>
			</div>
		</section>
	</div>
</section>

<section id="deep-dive">
	{% include section_header.html title="Concept &amp; Theory" lead="Formal treatments of the PSC framework, from intuition to equations." %}

	<div class="inner">
		<div class="grid-cards">
			<a href="framework/concept_estimation.html" class="image">
				<img src="{% link assets/images/concept-estim.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Concept and Estimation</h3>
					</header>
					<p>How model-estimated controls are conceived, fitted, and interpreted.</p>
					<ul class="actions">
						<li><a href="framework/concept_estimation.html" class="button">Read more</a></li>
					</ul>
				</div>
			</div>
		</div>

		<div class="grid-cards">
			<a href="framework/mathematical_fwk.html" class="image">
				<img src="{% link assets/images/math_board.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Mathematical Framework</h3>
					</header>
					<p>The causal-inference and Bayesian framework underpinning PSC treatment effects.</p>
					<ul class="actions">
						<li><a href="framework/mathematical_fwk.html" class="button">Read more</a></li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</section>

<section id="publication">
	<div class="inner box-round">
		<header class="major">
			<h2>Published Manuscript</h2>
		</header>
		<p>The methodology is described in full in our peer-reviewed paper in <em>BMC Medical Research Methodology</em>.</p>
		<ul class="actions">
			<li><a href="https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-025-02540-2" target="_blank" rel="noopener noreferrer" class="button special">Read the paper</a></li>
			<li><a href="how-to.html" class="button">Ready to apply PSCs?</a></li>
		</ul>
	</div>
</section>

{% include resources_tiles.html %}

<section id="research-context">
	<div class="inner box-round">
		<header class="major">
			<h2>Research Context</h2>
		</header>
		<p><em>Template section — add narrative on how PSCs developed, ongoing research, or links to related work.</em></p>
	</div>
</section>

<section id="key-terms">
	<div class="inner box-round">
		<header class="major">
			<h2>Key Terminology</h2>
		</header>
		<p><em>Template section — add a glossary of terms such as CFM, counterfactual, estimand, and transportability.</em></p>
	</div>
</section>

</div>
