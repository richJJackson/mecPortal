---
layout: post
title: PSCs for Trial Design
description: Using counterfactual models as external controls in single-arm and hybrid trial design.
image: assets/images/design_trials.png
---

<div id="main">

<section id="one">
<div class="inner">
	<header class="major">
		<h2>External controls in trial design</h2>
	</header>
	<p>
		In single-arm clinical trial design, a validated PSC model can act as an <strong>external control arm</strong> — providing a structured comparison without recruiting a full concurrent control cohort.
	</p>
	<p>
		This supports efficiency: fewer randomised control patients may be required while still enabling a principled comparison that accounts for uncertainty in the counterfactual model. Sample size and power calculations can incorporate both experimental-arm data and variability propagated from the CFM.
	</p>
</div>
</section>

<section id="applications">
<div class="inner box-round">
	<header class="major">
		<h2>Intended uses</h2>
	</header>
	<ul>
		<li>Design of single-arm phase II trials with model-based external controls.</li>
		<li>Hybrid designs where a PSC supplements a reduced randomised control arm.</li>
		<li>Retrospective evaluation of completed single-arm studies to inform phase III planning.</li>
		<li>Posterior predictive assessment of whether a phase II signal is consistent with phase III success.</li>
	</ul>
	<p><em>Template — expand with worked examples, operating characteristics, and regulatory context.</em></p>
</div>
</section>

<section id="software">
<div class="inner box-round">
	<header class="major">
		<h2>pscDesign</h2>
	</header>
	<p>
		The <code>pscDesign</code> R package supports trial design using Personalised Synthetic Controls. Documentation and examples will be added here.
	</p>
	<ul class="actions">
		<li><a href="../learn/software_pscExtra.html" class="button">pscDesign overview</a></li>
		<li><a href="../how-to.html#when" class="button">When to use PSCs</a></li>
	</ul>
</div>
</section>

</div>
