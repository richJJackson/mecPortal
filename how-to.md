---
title: How-to
banner_title: Put PSCs to Work
order: 2
layout: landing
description: Workflows, software, and step-by-step guides from data to decision.
image: assets/images/learn-img.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<section id="when">
	<div class="inner">
		<header class="major">
			<h2>When Should You Use PSCs?</h2>
		</header>
		<p>PSCs are most valuable when you need a structured treatment comparison but a full randomised control arm is missing, impractical, or inefficient.</p>

		<div class="box-round">
			<header class="minor">
				<h3>Estimating Treatment Effects</h3>
			</header>

			<div class="box-round">
				<h4>Randomised Controlled Trials</h4>
				<p>When only experimental-arm data are available, PSCs can act as a modelled control — enabling the same structured comparison a trial would provide, without recruiting a full control cohort.</p>
				<span class="image fit"><img src="{% link assets/images/illustration-psc-comp.png %}" alt="PSC comparison illustration" /></span>
			</div>

			<div class="box-round">
				<h4>Observational Data</h4>
				<p>For registries or single-arm cohorts where clinicians chose who to treat, PSCs generate a counterfactual outcome under standard care for each patient. The gap between observed and predicted outcomes estimates the treatment effect.</p>
				<span class="image fit"><img src="{% link assets/images/observ-diag.jpg %}" alt="Observational data diagram" /></span>
			</div>
		</div>

		<div class="box-round">
			<header class="minor">
				<h3>Designing Clinical Trials</h3>
			</header>
			<p>In single-arm trial design, a PSC model can serve as an external control arm — reducing the number of randomised control patients needed while preserving a principled comparison.</p>
			<span class="image fit"><img src="{% link assets/images/exp_trial.jpg %}" alt="Trial design diagram" /></span>
		</div>

		<ul class="actions">
			<li><a href="methodology.html" class="button">Review the methodology</a></li>
		</ul>
	</div>
</section>

<section id="workflow">
	{% include section_header.html title="Your Analysis Workflow" lead="A step-by-step path from defining treated patients to interpreting results." %}

	<div class="inner grid-cards">
		<a href="learn/howto_land.html" class="image">
			<img src="{% link assets/images/how-to.jpg %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>End-to-End Workflow</h3>
				</header>
				<p>Define treated units, select a counterfactual model, run estimation, and review diagnostics.</p>
				<ul class="actions">
					<li><a href="learn/howto_land.html" class="button">Start the workflow</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<section id="by-outcome">
	{% include section_header.html title="Guides by Outcome Type" lead="Practical tutorials for preparing data and running analyses." %}

	<section class="flex-cards">
		<section>
			<a href="learn/howto_formatData.html" class="image">
				<img src="{% link assets/images/format-data.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Format Your Data</h3>
					</header>
					<p>Structure cohorts and covariates so they align with your counterfactual model.</p>
					<ul class="actions">
						<li><a href="learn/howto_formatData.html" class="button">Learn more</a></li>
					</ul>
				</div>
			</div>
		</section>

		<section>
			<a href="learn/howto_surv.html" class="image">
				<img src="{% link assets/images/survival-outcomes.jpg %}" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Survival Outcomes</h3>
					</header>
					<p>Apply PSCs when your endpoint is time-to-event.</p>
					<ul class="actions">
						<li><a href="learn/howto_surv.html" class="button">Learn more</a></li>
					</ul>
				</div>
			</div>
		</section>

		<section>
			<a href="learn/howto_glm.html" class="image">
				<img src="{% link assets/images/outcomes-bin-con.jpg %}" alt="" data-position="top center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Binary &amp; Continuous Outcomes</h3>
					</header>
					<p>Apply PSCs for non-survival endpoints.</p>
					<ul class="actions">
						<li><a href="learn/howto_glm.html" class="button">Learn more</a></li>
					</ul>
				</div>
			</div>
		</section>
	</section>
</section>

<section id="software">
	{% include section_header.html title="Software &amp; Tools" lead="R packages and utilities for fitting PSCs and designing trials." %}

	<div class="inner grid-cards">
		<a href="learn/software_land.html" class="image">
			<img src="{% link assets/images/software.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>psc &amp; pscDesign Packages</h3>
				</header>
				<p>Install, configure, and run Personalised Synthetic Controls in R.</p>
				<ul class="actions">
					<li><a href="learn/software_land.html" class="button">View software</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<section id="checklist">
	<div class="inner box-round">
		<header class="major">
			<h2>Pre-Analysis Checklist</h2>
		</header>
		<p><em>Template section — add a checklist covering data completeness, covariate alignment, model validation, and assumption review before running a PSC analysis.</em></p>
	</div>
</section>

<section id="reporting">
	<div class="inner box-round">
		<header class="major">
			<h2>Reporting Your Results</h2>
		</header>
		<p><em>Template section — add guidance on what to report: estimands, uncertainty, diagnostics, and limitations.</em></p>
	</div>
</section>

<section id="contact">
	<div class="inner">
		<header class="major">
			<h2>Get in Touch</h2>
		</header>
		<p>Used PSCs in your research? We would like to hear from you.</p>
		<ul class="actions">
			<li><a href="resources/getting_started_guide.html" class="button special">Getting started guide</a></li>
			<li><a href="mailto:{{ site.email }}" class="button">Contact us</a></li>
		</ul>
	</div>
</section>

</div>
